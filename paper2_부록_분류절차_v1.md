# 부록: LLM 프레임 분류 절차와 프롬프트 (논문 2)

## A. 분류 환경

| 항목 | 내용 | 비고 |
|---|---|---|
| 분류 수행 | Anthropic의 대규모 언어모델을 코딩 에이전트 환경(Claude Code, 클라우드 세션)에서 사용 | |
| 세션 모델 설정 | 세션 생성 시 설정 `claude-opus-5-5`, 이후 사용자가 `claude-sonnet-5-5`로 전환. 현재 서비스 모델 `claude-sonnet-5-5` | 세션 메타데이터 기준 |
| 1차 분류(176편) 시점의 모델 | **기록 불충분** | 전환 시점과 해당 분류 시점의 대응 기록이 없다. 투고 전 세션 기록으로 확인하거나, 확인이 불가능하면 "모델 전환이 있었으며 시점별 모델은 확정하지 못했다"고 한계에 쓴다 |
| 반복·변형 분류(재분류) 모델 | 하위 에이전트로 호출. 별도 지정 없이 세션 기본 모델을 상속한 것으로 보이나 호출별 모델 식별자는 기록하지 않았다 | 확인 필요 |
| 호출 일자 | 1차 분류: 2026-10 중순(세션 2026-10-12 이후), 재분류: 2026-10-13 | 세션 생성일 2026-10-12 |
| 온도 등 샘플링 설정 | 사용자 지정 불가 환경, 기본값 | 재현성의 한계로 서술 |

## B. 입력 형식

각 논문은 한 줄 `TID | 논문명 | 키워드 | 초록`으로 제공하였다. 1차 분류와 반복 분류, 정의문 변경 분류는 초록 앞 450자, 초록 전체 제공 설정은 잘라내지 않은 초록을 입력하였다. 응답은 `TID|프레임|확신(상/중/하)` 한 줄로 받았다. 하위 에이전트에게는 이전 라벨, 토픽 번호, 분야 정보, 결과 파일을 보지 말도록 지시하였다(블라인드).

## C. 코드북

코드북 v3(`frame_coding_criteria.md`)를 제공하였다. 프레임 정의는 다음과 같다.

| 프레임 | 핵심 논거 |
|---|---|
| 현실 | 국가(또는 국가 주도 기업)의 힘·경쟁력·안보·자립·상대적 이익 (수출통제, 제재, 군사 활용, 기술 패권, 산업 육성, AI 주권, 공급망) |
| 자유 | 규칙과 제도의 설계·정합·조화·협력·표준 (규제 체계 설계, 입법 비교, 규제 조화, 표준화, 다자 협의체) |
| 구성 | 권리·윤리·책임·가치·정당성 (기본권, 인간 존엄, 책임 귀속, 투명성·설명가능성 원칙, 규범 확산) |
| 해당없음 | 논거·처방이 없는 현황 소개, 또는 거버넌스와 무관한 이슈 |
| U | 정보가 부족해 판단 불가 |

판단 순서: (1) 처방이 무엇으로 정당화되는가, (2) 처방이 없으면 문제 정의, (3) 단순 법리 해석은 가장 가까운 논거로 배정하되 확신 '하', (4) 혼합이면 주 프레임 하나. 경계 사례 10개 규칙은 코드북 원문을 따른다. 법리·정책 문서도 논거의 종류로 프레임을 배정하며 해당없음을 기본값으로 쓰지 않는다.

## D. 재분류 지시문 원문

### D-1. 독립 반복 및 초록 전체 제공 (코드북 사용; 입력 파일만 다름)

> Classify academic papers by IR-theory frame. Read the codebook /home/user/test-git/frame_coding_criteria.md (use sections defining the frame categories; ignore any procedure sections about pilots/reviews). Then read the input file (tab-separated: TID, title, keywords, abstract start). Do NOT read any other files in that scratchpad or the repo (no prior labels, xlsx, pkl, or results files) — this is an independent blind repeat. For each paper assign one frame: 현실, 자유, 구성, 해당없음, or U, plus a confidence 상/중/하, following the codebook's core-argument rule. Write output to [출력 파일], one line per paper: TID|frame|confidence. Cover every TID. Reply only 'done' and the count.

초록 전체 제공 설정은 같은 지시문에 "(…, full abstract)"만 달랐다. 입력은 4개 파일(독립 반복) 또는 2개 파일(변형)로 나누어 병렬 수행하였다.

### D-2. 정의문 변경 (코드북 미제공)

> Classify academic papers by which international-relations perspective their central argument takes. Do NOT read any repo files or other scratchpad files. Read only [입력 파일] (tab-separated: TID, title, keywords, abstract start; all about AI governance/strategy). Categories: 현실 = AI treated as an object of power, national interest, technological competition, military/security advantage, or great-power rivalry; the argument is about states winning or staying safe. 자유 = the argument is about building or reforming rules, institutions, regulation, standards, international cooperation or legal harmonization to manage AI. 구성 = the argument is about norms, ethics, rights, responsibility, identity, values or social meaning of AI. 해당없음 = none of these is the core argument (e.g., purely technical or business application). U = cannot judge. Judge by the core argument, not by mere mention of keywords. Give confidence 상/중/하. Write [출력 파일], lines TID|frame|confidence, every TID. Reply only 'done' and count.

## E. 1차 분류(분석 기준값)의 지시문

176편의 1차 분류는 별도 하위 에이전트가 아니라 코딩 세션 안에서 코드북 v3와 위 입력 형식으로 수행하였고, 그 시점의 지시문을 파일로 보존하지 않았다. 따라서 재현은 코드북 v3와 위 입력 형식에 의존한다. **이 점은 재현성의 한계로 논문에 명시해야 한다.** 186편 중 10편은 연구자 확정 라벨이다.

## F. 코드북과 실제 입력의 차이 (정리 필요)

1. 코드북 §1은 논문 입력을 "논문명 + 국문 초록, 키워드 필드는 판단 근거로 쓰지 않는다"고 규정하나, 논문 2의 분류 입력에는 키워드가 포함되었고 초록은 앞 450자로 잘렸다. 원고 Ⅲ-2는 실제 입력("제목, 키워드, 초록 앞 450자")을 기술하고 있다. 코드북 §1과 어긋난 점을 부록에 명시하는 것이 정직하다.
2. 코드북의 국제맥락·경쟁대립 플래그는 본 분류에서 사용하지 않았다(본 코딩 절차 §10).
3. 코드북 v3의 신뢰도 서술(§7)은 논문 1의 두 코더 파일럿에 관한 것이며, 본 논문의 타당화는 별도 50편 연구자 독립 코딩이다.
