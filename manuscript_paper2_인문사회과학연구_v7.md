---
title: "같은 소재, 다른 문제틀: 국가 전략·미중 경쟁 토픽에 대한 학문분야별 AI 거버넌스 프레임 비교"
---

**원고 매수: 200자 원고지 약 85매 (글자 수 기준 어림값, 한글 2005에서 다시 계산)**

**영문 제목: Same Subject, Different Frames: Comparing AI Governance Frames across Academic Disciplines on the National Strategy and US–China Competition Topic**

**저자: [심사본에서는 삭제]**

# 초록

본 연구는 한국 학계의 AI 거버넌스 논의 중 ‘국가 전략·미중 경쟁’ 토픽에 속한 KCI 학술논문 186편을 전수 대상으로, 학문분야에 따라 국제정치이론 프레임(현실주의·자유주의·구성주의)이 어떻게 달라지는지 비교하였다. 프레임 판정에는 대규모 언어모델(LLM)을 분류 도구로 쓰고, 반복 분류와 프롬프트 변형, 연구자의 독립 코딩 50편으로 안정성과 타당성을 점검하였다. 정치외교학(73%)·지역학(74%)·군사학(86%)·정책학(92%)은 현실주의 프레임이 우세했고, 법학은 제도·규범을 강조하는 자유주의 프레임이 가장 많았으며(46%), 교육학은 대부분(90%) 어느 프레임에도 해당하지 않았다(Cramér’s V=0.40). 이 큰 방향은 분류 설정과 무관하게 유지되었으나 세부 비율, 특히 구성주의 비중은 설정에 민감하였다. 연구자와의 일치도는 κ=0.67이었다. 본 연구는 AI 거버넌스 담론이 분야별로 다른 문제틀 위에서 전개됨을 보이고, LLM 기반 프레임 분류의 가능성과 한계를 함께 제시한다.

**주제어**: AI 거버넌스, 프레임 분석, 학문분야, 국제정치이론, LLM 기반 내용분석

# Abstract

Using all 186 Korean journal articles (KCI) on the national strategy and US–China competition topic of AI governance, this study compares how academic disciplines frame the same issue from realist, liberal, and constructivist perspectives. A large language model (LLM) coded the frames; stability was checked with a blind repeat and two prompt variations, and validity against the researcher’s independent coding of 50 papers. Realism dominated political science/diplomacy (73%), area studies (74%), military studies (86%), and policy studies (92%), whereas law favored a liberal, rules-and-institutions frame (46%), and most education papers (90%) fit none of the frames (Cramér’s V = 0.40). The broad pattern held across all settings, but disciplinary percentages, particularly for constructivism, were sensitive to prompt wording. Agreement with the researcher was substantial (κ = 0.67). AI governance discourse rests on different problem frames across disciplines, and LLM-based frame classification is promising but setting-dependent.

**Keywords**: AI governance, framing, academic disciplines, international relations theory, LLM-assisted content analysis

# Ⅰ. 서론

## 1. 연구 배경과 목적

인공지능(AI)의 국제 거버넌스는 한국에서도 여러 학문분야가 함께 다루는 주제가 되었다(박선형 2024; 김지상 2026). 정치외교학과 군사학은 미중 기술 경쟁과 안보를(윤정현 2026; 이상훈·권혁진 2025), 법학은 각국의 규제 입법과 국제 규범을(안준철 2024; 김태훈·이성엽 2025), 경영학과 교육학은 산업 경쟁력과 인재 문제를 논의한다(김성준·이중학 2026; 이현주 2025). 그러나 이 분야들이 같은 문제를 같은 방식으로 규정하는지는 확인된 바가 많지 않다. 같은 ‘국가 전략과 미중 경쟁’이라는 소재를 두고도 어떤 분야는 힘과 안보의 문제로, 어떤 분야는 규칙과 제도의 문제로 풀 수 있다.

동일한 코퍼스와 토픽모형을 사용한 별도의 연구(익명 처리, 투고 준비 중, 이하 별도 연구)는 2019년 5월부터 2026년 9월까지 한국 언론과 학계의 AI 글로벌 거버넌스 담론을 토픽모형과 국제정치이론 프레임으로 비교하였다. 그 연구에서 국가 전략·미중 경쟁 토픽은 뉴스의 대부분을 차지했고, 학술논문에서도 가장 큰 토픽 가운데 하나였다. 별도 연구는 아직 공개되지 않았으므로 본 연구는 그 결과에 의존하지 않고, 같은 코퍼스에서 도출한 T1 논문 186편을 새로운 질문(분야 간 비교)과 새로운 방법(LLM 분류의 안정성·타당화)으로 분석한다. 본 연구는 이 토픽에 속한 학술논문 186편 전체를 대상으로, 같은 소재 안에서 학문분야에 따라 프레임이 어떻게 달라지는지를 비교한다. 소재를 고정함으로써 분야 간 차이가 주제 선택이 아닌 문제 규정 방식의 차이임을 드러내려는 것이다.

연구 문제는 다음과 같다. 같은 ‘국가 전략·미중 경쟁’ 토픽 안에서 학문분야별 국제정치이론 프레임(현실주의, 자유주의, 구성주의)의 분포는 어떻게 다른가. 또한 프레임 분류에 대규모 언어모델(LLM: large language model)을 도구로 쓸 때 그 분포 차이는 분류 설정에 얼마나 안정적인가.

## 2. 논문의 구성

Ⅱ장에서 이론적 배경을, Ⅲ장에서 자료와 LLM 기반 분류 방법을, Ⅳ장에서 결과를, Ⅴ장에서 논의와 결론을 제시한다.

# Ⅱ. 이론적 배경

## 1. AI 거버넌스와 세 이론 전통

AI를 규율하는 국제 규범은 하나의 조약이나 기구가 아니라 여러 기구와 문서가 겹친 분절된 형태로 발전해 왔다(Cihon et al. 2020; Schmitt 2022; Stix 2022). 이 지형은 협력만으로 구성되지 않고 여러 행위자가 서로 다른 제도를 통해 규칙의 주도권을 다투는 경합적 다자주의(contested multilateralism)의 성격도 지닌다(Morse and Keohane 2014; 하윤빈 2026). 따라서 같은 사건이 어떤 행위자에게는 제도 설계의 문제로, 다른 행위자에게는 경쟁과 안보의 문제로 해석될 수 있다(Evans and Singh 2026). 국제정치학의 세 이론 전통은 이 해석의 차이를 구분하는 틀이 된다(Hay 2016). 본 연구는 세 전통을 담론이 문제를 규정하고 처방을 정당화하는 논거의 유형으로 조작화한다. 이는 프레임을 문제 규정과 처방의 정당화로 보는 엔트먼(Entman 1993)의 개념과 통합적 프레임 분석(Dan 2017)에 따른 것이다.

현실주의(realism)는 국가 간 힘의 분포, 안보, 경쟁에 주목한다. AI를 군사력과 국제정치에 영향을 주는 촉진 기술로 보는 연구(Horowitz 2018)와, AI 반도체 공급망과 수출통제(유인태 2025), 미중 AI 패권경쟁(김상배 2025), AI 군사력 경쟁(차정미 2022), 자율무기와 세력 전이(이재준 2022), AI 안보화 담론(윤정현 2026), 무기기술과 AI 윤리(이상훈·권혁진 2025)에 관한 국내 연구가 이 계열이다. 자유주의(liberalism)는 규칙과 제도의 설계, 조화, 협력에 주목하며, 국제기구와 다자 협의체를 AI 정책의 조율 장치로 본다(Schmitt 2022; Cihon et al. 2020; 윤혜선 2024; Sayles 2024). 구성주의(constructivism)는 규범과 가치, 정체성이 무엇을 정당한 행동으로 만드는지에 주목한다(Finnemore and Sikkink 1998; Erskine 2024). AI 윤리 지침이 투명성, 공정성, 책임 등으로 수렴하되 이행은 갈린다는 연구(Jobin et al. 2019; Hagendorff 2020; 안소영 2025)와 중국의 AI 규범 분석(Roberts et al. 2021; 이재숭 2022; 구오단양 2024; Carvalho 2026), 롤스적 관점에서 AI 거버넌스를 논의한 연구(서요련 2026)가 여기에 해당한다.

## 2. 연구 공백

선행 연구는 AI 거버넌스를 이론별로 설명하거나, 뉴스 프레이밍(framing)을 가치 프레임 중심으로 분석해 왔다(최믿음·조은수 2024; 이겨레·임철민 2026). 그러나 한국 학계 안에서 학문분야에 따라 같은 소재가 어떤 이론 프레임으로 다루어지는지를 전수 자료로 비교한 연구는 확인하지 못했다 [확인: 학술DB 직접 검색 필요]. 한편 LLM을 텍스트 주석 도구로 쓰는 연구는 프레임 탐지를 포함한 과제에서 인간 주석자와 견줄 만한 정확도와 일치도를 보고해 왔고(Gilardi et al. 2023; Ziems et al. 2024), 보건·언론·사회 분야 등에서 LLM을 활용한 내용분석이 확산되고 있다(Li et al. 2026; Wang and Poenaru 2026). 다른 한편으로는 프롬프트 문구를 조금 바꾸거나 같은 입력을 반복해도 출력이 달라질 수 있으므로 인간 라벨에 의한 검증이 필요하다는 경고도 있다(Reiss 2023; Demirbaş 2026). 다만 이 연구들은 주로 영어 텍스트를 대상으로 하며(Sazzed 2026; Sulaiman et al. 2025), 한국어 학술논문에서 이론 기반 프레임을 분류하면서 그 결과가 분류 설정과 사람 코딩에 얼마나 견고한지를 함께 보고한 연구는 확인하지 못했다 [확인: 학술DB 직접 검색 필요]. 본 연구는 이 두 공백을 다룬다. 학문분야는 문제를 보는 훈련과 규범이 다르므로 같은 소재라도 다른 프레임을 택할 것이라는 기대가 있으나(Dan 2017), 이를 검증한 근거는 확인되지 않았으므로 본 연구는 탐색적 비교로 수행한다. 따라서 가설 검정 대신 분야별 분포와 그 안정성을 기술한다.

# Ⅲ. 연구 방법

## 1. 분석 대상

분석 대상은 KCI 등재지·등재후보지 논문 669편에 LDA(latent Dirichlet allocation) 토픽모형(K=7)을 추정하여 ‘국가 전략·미중 경쟁’(T1) 토픽에 가장 높은 비중으로 배정된 논문 186편 전체이다. 표집 없이 전수를 분석하므로 보고하는 비율은 표본추정치가 아니라 이 코퍼스의 모수이다. 다만 코퍼스는 검색·수집 범위와 토픽 배정 규칙에 의존하므로 일반화 범위는 이 코퍼스로 한정한다. 코퍼스와 토픽모형은 별도 연구(투고 준비 중)와 같은 것이며, 별도 연구의 프레임 코딩 표본 가운데 T1에 속한 10편의 연구자 라벨이 본 연구의 1차 분류값에 포함되어 있다. 두 연구는 연구 질문(뉴스·학계 비교 대 학계 내 분야 비교)과 분석 단위, 방법(표집·가중 추정 대 전수·LLM 분류)이 다르다. 학문분야는 KCI가 논문별로 부여한 단일 연구분야 경로(대분류 > 중분류 > 소분류)의 중분류(두 번째 단계)를 사용하였다. 186편 모두 하나의 경로만 갖고 있어 복수 분야 논문은 없었다. 경로가 중분류 한 단계로만 기재된 3편(정책학 1, 지역학 2)은 그 이름을 중분류로 보았다. 10편 미만 분야는 ‘기타’로 묶었다.

## 2. 프레임 분류

분류 단위는 논문 1편(제목, 키워드, 초록 앞 450자)이다. 분류 기준은 핵심 논거를 기준으로 현실(권력·경쟁·안보), 자유(규칙·제도 설계·조화), 구성(권리·윤리·책임·가치), 해당없음 중 하나를 배정하는 코드북이며, 판정이 어려우면 판정불가(U)로 둔다(Dan 2017). 분류는 사람 코더가 아니라 LLM이 코드북에 따라 논문별로 프레임과 확신도를 출력하는 방식으로 수행하였다. 사용 모델의 식별자와 호출 일자, 프롬프트 전문은 부록에 제시한다 [확인: 1차 분류 시점의 모델 식별자 기록 불충분, 부록 A 참조]. 코드북은 입력으로 논문명과 초록만 규정하나 본 분류에서는 키워드를 함께 제공하였다(부록 F). 186편 중 10편은 별도 연구 과정에서 연구자가 직접 확정한 라벨이 있어 1차 분류값에 연구자 라벨을 그대로 사용하였고(나머지 176편은 LLM 분류), 반복·변형 분류는 186편 전체를 LLM이 분류하였다. 이 10편과 LLM 재분류의 일치는 타당화 참고로도 보고한다.

## 3. 타당화와 안정성 점검

사람 코딩을 하지 않으므로 다음 세 가지로 분류의 신뢰성을 점검하였다(Reiss 2023; Demirbaş 2026). 첫째, 이전 라벨을 보지 않은 독립 LLM 인스턴스로 같은 코드북과 입력으로 재분류하였다(독립 반복). 둘째, 초록을 잘라내지 않고 전체를 제공하였다. 셋째, 코드북 없이 새로 작성한 짧은 정의문만 제공하였다. 일치도는 일치율과 코헨의 카파(Cohen 1960)로 보고하며 해석은 랜디스와 코크(Landis and Koch 1977)의 구간을 참고한다. 이 점검은 같은 계열 모델 간의 안정성(신뢰도)을 보여줄 뿐 타당도를 보증하지 않는다. 타당도의 외부 기준으로, 연구자가 LLM 분류를 보지 않은 채 독립적으로 코딩한 50편(LLM 1차 분류별 층화 추출: 현실 20, 자유 10, 구성 10, 해당없음 10)과 비교하였다. 50편은 연구자 확정 10편과 겹치지 않으며 표본이 작다. 층화가 LLM 라벨 기준이므로 전체 일치율은 층 크기(176편 중 현실 98, 자유 27, 구성 27, 해당없음 23)로 가중해 추정하고, 신뢰구간은 부트스트랩(2,000회)으로 구하였다.

## 4. 분석

분야 × 프레임 교차표로 분야별 비율을 제시하고, 연관 강도는 크라메르의 V(Cramér’s V)로 나타낸다. 전수 자료이므로 유의성 검정 대신 분야 라벨을 무작위로 섞은 5,000회 참조분포를 비교 지표로 제시한다. 주 분석은 초록 앞 450자를 입력한 1차 분류 값이며, 초록 전체 제공은 강건성 분석의 한 설정으로 다룬다. 분야별 비율은 1차 분류 값과 1차 분류를 포함한 네 가지 설정(1차, 독립 반복, 초록 전체 제공, 정의문 변경)의 최소–최대 범위를 함께 보고한다. 주 분석 입력을 450자로 둔 것은 분석 설계 단계의 결정이며, 사람 대조 이후에도 바꾸지 않았다.

## 5. 인공지능 활용 고지

프레임 분류의 분석 도구로 대규모 언어모델(LLM)을 사용하였다. 1차 분류값 186편 중 176편은 연구자의 재검토를 거치지 않은 자동 분류값이고 10편은 연구자 확정 라벨이다. LLM 분류의 타당화는 연구자가 LLM 라벨을 보지 않고 독립 코딩한 50편으로 수행하였다. 또한 원고 작성에 LLM의 도움을 받았다. [확인: 학술지 규정의 AI 활용 고지 문구]

# Ⅳ. 연구 결과

## 1. 전체 분포

1차 분류 기준으로 T1 186편의 프레임은 현실 102편(54.8%), 자유 29편(15.6%), 구성 28편(15.1%), 해당없음 26편(14.0%), 판정불가 1편(0.5%)이다. 같은 토픽 안에서도 현실주의 프레임이 절반을 넘지만, 그 외 프레임이 합쳐 45%에 이른다.

## 2. 학문분야별 프레임 분포

<표 1>은 중분류 분야별 프레임 비율(1차 분류, %)과 네 가지 설정에서의 범위이다. 10편 미만 분야는 ‘기타’로 묶었다(n=31).

**<표 1> 학문분야별 프레임 비율(%): 1차 분류(네 설정의 최소–최대)**

| 분야 | n | 현실 | 자유 | 구성 | 해당없음 |
|---|---|---|---|---|---|
| 정치외교학 | 30 | 73 (73–77) | 10 (7–10) | 17 (17–20) | 0 (0–0) |
| 지역학 | 27 | 74 (67–78) | 15 (11–15) | 11 (7–11) | 0 (0–11) |
| 법학 | 24 | 29 (29–33) | 46 (33–62) | 17 (0–29) | 4 (4–4) |
| 경영학 | 15 | 27 (27–47) | 27 (20–27) | 13 (0–13) | 33 (27–47) |
| 군사학 | 14 | 86 (57–86) | 0 (0–7) | 14 (7–21) | 0 (0–29) |
| 학제간연구 | 13 | 54 (54–62) | 8 (8–8) | 31 (15–31) | 8 (8–23) |
| 정책학 | 12 | 92 (67–92) | 0 (0–0) | 8 (0–8) | 0 (0–25) |
| 사회과학일반 | 10 | 60 (40–60) | 0 (0–10) | 10 (0–20) | 30 (30–50) |
| 교육학 | 10 | 0 (0–0) | 0 (0–0) | 10 (10–30) | 90 (70–90) |
| 기타 | 31 | 42 (42–55) | 19 (19–19) | 16 (13–16) | 23 (13–26) |

출처: 저자 분석.

분야와 프레임의 연관 강도는 Cramér’s V = 0.40(네 설정에서 0.38–0.40)로 중간 이상이다. 분야 라벨을 무작위로 섞은 5,000회 참조분포에서 관측값 이상이 나온 경우는 없었다(p<0.001). 전수 자료이므로 이 값은 추론적 검정이 아니라 ‘분야 구분 없이 프레임이 배정되었다고 가정할 때 이 정도 차이가 나올 가능성’을 보여주는 참조 지표로만 해석한다.

## 3. 주요 발견

**1) 안보·국제정치 계열은 현실 프레임이 지배적이다.** 정치외교학(73%), 지역학(74%), 군사학(86%), 정책학(92%)에서 현실 프레임이 70% 안팎 이상이다. 이 가운데 정치외교·군사·지역 세 분야를 합친 계열(n=71)에서는 현실 76%(68–79), 자유 10%(7–10), 구성 14%(13–15)이다.

**2) 법학은 같은 토픽을 자유(제도·규범) 프레임으로 다룬다.** 법학 24편 중 자유가 46%(33–62)로 가장 많고 현실은 29%(29–33)에 그친다. 같은 ‘국가 전략·미중 경쟁’ 토픽이라도 법학은 경쟁 자체보다 규제·제도 설계를 논거의 중심에 둔다(윤혜선 2024; 안준철 2024). 이 분야 차이의 방향(법학의 현실 비중이 정치외교·지역의 절반 이하)은 네 설정 모두에서 유지되었다.

**3) 경영학과 교육학은 프레임 바깥의 접근이 많다.** 교육학은 10편 중 9편이 해당없음(90%)이며 현실 프레임은 없다(0%). 경영학은 현실·자유·해당없음이 각각 27–33%로 분산한다. 이는 해당 분야가 이 토픽을 국제정치 프레임이 아닌 산업·인재·기술 응용 문제로 다룬다는 뜻으로 해석할 수 있다(김성준·이중학 2026; 이호찬·이상윤 2025).

**4) 구성주의 프레임은 학제간 연구에서 상대적으로 높다.** 학제간연구의 구성 비중은 31%(15–31)로 전체 평균(15%)의 두 배이나, n=13이고 정의문 변경 시 절반으로 줄어들므로 잠정적 관찰에 그친다.

## 4. 분류 설정에 대한 강건성(요약)

분야 간 차이의 큰 방향(정치외교·지역·군사·정책은 현실, 법학은 자유 비중이 가장 큼, 교육학은 해당없음)은 네 가지 분류 설정에서 모두 유지되었다.

반면 군사학(현실 86→57), 정책학(92→67), 경영학(현실 27→47), 법학의 자유(33–62), 구성 비율 전반은 설정에 따라 크게 움직인다. 이들의 절대 수치는 점추정이 아니라 범위로 해석해야 한다.

분야별 반복 분류 일치율은 정치외교 0.93, 군사 0.93, 지역 0.89, 법학 0.83, 경영 0.67로, 일치율이 낮은 분야일수록 위 범위가 넓다.

## 5. 분류의 안정성

<표 2>는 1차 분류와 세 가지 재분류(독립 반복, 초록 전체 제공, 정의문 변경)의 일치도이다. 재분류는 모두 이전 라벨을 보지 않은 독립 인스턴스가 수행하였다.

**<표 2> 분류 설정 간 일치도**

| 비교 | 일치율 | κ |
|---|---|---|
| 1차 분류 vs 독립 반복 | 0.882 | 0.811 |
| 1차 분류 vs 초록 전체 제공 | 0.876 | 0.799 |
| 1차 분류 vs 정의문 변경 | 0.817 | 0.719 |
| 초록 전체 제공 vs 정의문 변경 | – | 0.696 |

출처: 저자 분석.

코드북이 같으면 κ가 0.80 안팎으로 안정적이었으나, 정의문을 바꾸면 ‘구성’ 논문 10편이 ‘자유’로, ‘현실’ 논문 11편이 ‘해당없음’으로 옮겨 가 구성 비중이 15%에서 9%로 줄었다. 확신도별 일치율은 ‘상’ 97.6%, ‘중’ 88.7%, ‘하’ 65.2%였다. 사람 기준과의 대조에서는, 연구자가 독립 코딩한 50편과 LLM 1차 분류의 일치율이 76.0%, κ = 0.67(95% 부트스트랩 구간 0.50–0.82)이었다. LLM 라벨의 층 크기로 가중한 일치율은 77.1%(0.65–0.89)였다. 같은 50편에서 다른 설정의 일치는 독립 반복 0.82(κ 0.75), 초록 전체 제공 0.90(κ 0.86; 강건성 설정이며 주 분석값은 아님), 정의문 변경 0.70(κ 0.60)이었다. 불일치 12편 가운데 연구자가 ‘구성’으로 판정했으나 LLM이 다른 프레임(자유 1, 해당없음 2, 현실 2)으로 분류한 경우가 5편, 반대로 LLM이 ‘구성’으로 분류했으나 연구자는 다르게 판정한 경우가 2편이었다. 분야별로는 정치외교 12편 중 11편(92%)이 일치한 반면 법학은 7편 중 4편(57%), 정책학은 4편 중 2편(50%)이었고, 분야별 표본이 작아 참고용이다. 연구자 확정 10편과의 일치는 별도로 독립 반복 6편, 초록 전체 제공 7편, 정의문 변경 6편이었다.

## 6. 이 결과가 말하지 못하는 것

주 분석 입력(450자)보다 초록 전체를 줄 때 연구자와의 일치가 더 높았으므로(표본 50편), 입력 텍스트의 길이와 구성이 분류 품질에 영향을 줄 수 있다(Sulaiman et al. 2025). 초록 전체 기준 분야별 비율은 <표 1>의 범위에 이미 포함되어 있다.

사람 기준과의 타당도는 단일 코더 50편에서 κ=0.67(구간 0.50–0.82)로 확인되었으나 표본이 작고 구간 하한이 낮다.

제목·초록 기반 분류이므로 본문 논거와 다를 수 있다.

분야 구분은 KCI가 학술지·논문에 부여한 중분류 기준이며, 논문의 실제 내용 분야와 다를 수 있다.

# Ⅴ. 논의 및 결론

## 1. 발견의 의미

같은 ‘국가 전략·미중 경쟁’ 토픽 안에서도 학문분야가 논거의 중심을 다르게 설정한다는 점이 확인되었다. 안보·국제정치 계열은 AI를 국가 간 경쟁과 안보의 대상으로 다루는 현실주의 문제틀을 따르고(윤정현 2026), 법학은 같은 경쟁 상황을 규제와 제도 설계의 문제로 옮겨 다룬다(김태훈·이성엽 2025; 김유정 2026). 이는 AI 거버넌스 담론이 하나의 공통 논의가 아니라 분야별 문제 정의 위에서 병렬로 전개되고 있음을 시사한다(박선형 2024). 별도 연구(투고 준비 중)에서 확인한 뉴스와 학계의 프레임 차이는 학계 내부의 이질성이 부분적 원인일 수 있다는 해석의 단서도 제공하나, 두 연구의 대상과 방법이 다르므로 직접 비교는 하지 않았다 [확인: 별도 연구가 공개되기 전에는 이 문장 삭제 또는 일반화 검토].

## 2. 정책·학술적 함의

정책적으로 안보 중심 논의와 제도·규범 중심 논의가 서로 다른 분야에서 생산되므로, 국가 전략을 수립할 때 두 계열의 지식이 연결되는 경로가 필요하다(김지상 2026).

학술적으로 학제간연구에서 구성주의 프레임이 상대적으로 높게 나타난 점은 후속 연구에서 본문 수준 분석으로 확인할 만하다.

## 3. 방법론적 시사점과 한계

LLM 분류는 같은 코드북에서 안정적이었으나(κ≈0.80) 정의문이 바뀌면 구성주의 경계가 크게 움직였다. 따라서 LLM 기반 프레임 분석은 수치 하나가 아니라 설정별 범위로 보고해야 한다(Reiss 2023; Demirbaş 2026).

연구자의 독립 코딩 50편과의 일치는 κ=0.67(95% 구간 0.50–0.82)로, 사람 기준 타당도가 어느 정도 확인되었으나 단일 코더, 50편이라는 한계가 있고 구간 하한이 중등도 수준이다. 불일치에서 연구자가 ‘구성’으로 보고 LLM이 아니라고 본 경우(5편)가 반대(2편)보다 많아, 구성 비중이 LLM 분류에서 과소추정되었을 가능성이 있으나 표본이 작아 잠정적이다. 반복 분류는 신뢰도일 뿐 타당도를 보증하지 않으며 체계적 편향은 재현된다.

제목·초록 기반 분류이고, KCI 코퍼스와 LDA 배정에 의존하며, 소규모 분야(n<15)의 비율은 불안정하다. 결과는 이 코퍼스에 한정된 기술적 모수이다.

후속 연구는 사람 코더 다수와의 대조, 본문 수준 분석, 복수 모델 비교가 필요하다(Wang and Poenaru 2026).

## 4. 결론

한국 학계는 AI 거버넌스의 국가 전략 문제를 분야에 따라 현실주의적 경쟁 논리, 제도·규범 설계, 또는 프레임 바깥의 응용 문제로 서로 다르게 다루고 있다. 이 분야 간 차이는 분류 설정을 바꾸어도 큰 방향이 유지되는 반면, 세부 수치는 범위로 해석해야 한다.

# 참고문헌

구오단양. 2024. “Advancing AI Governance and Lawmaking in China: Insights and Strategies.” 『한중사회과학연구』 22(2), 279-298.

김상배. 2025. “미중 인공지능 패권경쟁과 한국: 국제정치의 전환과 중견국의 국가전략.” 『국가전략』 31(2), 101-132.

김성준·이중학. 2026. “AI Governance, 조직 및 인사 분야 시사점과 연구제언.” 『조직과 인사관리연구』 50(3), 29-85.

김유정. 2026. “일본 AI법(人工知能関連技術の研究開発及び活用の推進に関する法律) 제정 과정에 관한 연구.” 『일본학보』 146, 301-317.

김지상. 2026. “AI 기본법 너머의 정책 설계 과제: 한국 국가 AI 정책의 방향성과 거버넌스 구조 분석.” 『한국정책학회보』 35(3), 577-614.

김태훈·이성엽. 2025. “소버린 AI(Sovereign AI) 구축의 글로벌법제 동향에 관한 연구.” 『경영법률』 36(1), 195-223.

박선형. 2024. “AI 거버넌스의 정의와 쟁점 및 발전 과제: 비판적 관점.” 『교육정치학연구』 31(1), 89-117.

서요련. 2026. “무지의 베일을 쓴 AI: 롤스적 AI 거버넌스에 관한 비판적 고찰.” 『도덕윤리과교육』 92, 231-260.

안소영. 2025. “기업의 AI 윤리 실천: LG AI연구원의 사례 분석.” 『과학기술과 사회』 8, 63-99.

안준철. 2024. “유럽의 AI 거버넌스와 미디어 책임.” 『통합유럽연구』 15(3), 209-242.

유인태. 2025. “인공지능과 미·중 전략 경쟁의 국제정치: 글로벌 AI 반도체 공급망과 미국의 경제적 강압을 중심으로.” 『국제정치논총』 65(1), 103-140.

윤정현. 2026. “미국의 AI 안보화 담론과 AI 안보 거버넌스의 재구성.” 『대한정치학회보』 34(1), 79-108.

윤혜선. 2024. “AI 거버넌스의 새로운 축(軸): 영향평가제도에 관한 연구.” 『공법연구』 53(2), 377-424.

이겨레·임철민. 2026. “토픽모델링(BERTopic)을 활용한 국내 인공지능 정책 관련 언론보도 분석.” 『한국콘텐츠학회 논문지』 26(2), 86-100.

이상훈·권혁진. 2025. “다계층 AI 거버넌스를 통한 AI 윤리 확보 방안 연구: 무기기술 발전과 인간 존엄성을 중심으로.” 『시스템엔지니어링학술지』 21(2), 34-51.

이재숭. 2022. “중국의 인공지능(AI) 윤리 정책에 관한 연구.” 『중국학』 80, 69-87.

이재준. 2022. “미국과 중국의 군사 기술 경쟁과 세력 전이: 인공지능, 자율무기체계 군사 기술을 중심으로.” 『한국과 국제정치』 38(3), 1-35.

이현주. 2025. “AI 시대 화성시 문화예술교육의 현황과 혁신 가능성 제안.” 『브랜드디자인학연구』 23(4), 65-74.

이호찬·이상윤. 2025. “적소적재 채용 전략을 위한 AI 정책과 활용 동향 분석: 국내 사례와 글로벌 트렌드 비교 및 시사점 분석을 중심으로.” 『인적자원관리연구』 32(5), 221-239.

차정미. 2022. “미중 패권경쟁과 인공지능 군사력 경쟁.” 『국가전략』 28(3), 5-31.

최믿음·조은수. 2024. “AI 관련 뉴스기사의 보도 프레임 분석.” 『문화기술의 융합』 10(6), 339-346.

하윤빈. 2026. “AI 거버넌스와 글로벌 사우스: 배제의 권력 기제와 전략적 대응.” 『세계지역연구논총』 44(3), 55-105.

Carvalho, A. 2026. “China’s AI Governance Architecture: From State Control to Operational AI Governance.” SSRN. https://doi.org/10.2139/ssrn.6656118 [확인: 프리프린트, 게재본 여부]

Cihon, P., M. M. Maas, and L. Kemp. 2020. “Fragmentation and the Future: Investigating Architectures for International AI Governance.” Global Policy 11(5). [확인: 쪽수·DOI]

Cohen, J. 1960. “A Coefficient of Agreement for Nominal Scales.” Educational and Psychological Measurement 20(1): 37-46.

Dan, V. 2017. Integrative Framing Analysis: Framing Health through Words and Visuals. London: Routledge. https://doi.org/10.4324/9781315171456 [확인: 부제·출판지; 본문 인용은 서론장 및 ‘프레이밍 영향 요인’ 장을 포함해 단행본 하나로 통합함]

Demirbaş, D. 2026. “Revisiting Trust and Interpretive Authority in LLM-Assisted Qualitative Data Analysis.” Research Square (Preprint). https://doi.org/10.21203/rs.3.rs-9629061/v1

Entman, R. M. 1993. “Framing: Toward Clarification of a Fractured Paradigm.” Journal of Communication 43(4): 51-58.

Erskine, T. 2024. “Normative International Relations Theory.” In International Relations Theories, 264-291. Oxford: Oxford University Press. https://doi.org/10.1093/hepl/9780192866455.003.0015 [확인: 편집자·판차]

Evans, A., and A. Singh. 2026. “AI Governance Framework Models.” In AI Governance, 110-128. https://doi.org/10.4324/9781003682530-12 [확인: 편집자·출판사]

Finnemore, M., and K. Sikkink. 1998. “International Norm Dynamics and Political Change.” International Organization 52(4): 887-917.

Gilardi, F., M. Alizadeh, and M. Kubli. 2023. “ChatGPT Outperforms Crowd Workers for Text-Annotation Tasks.” Proceedings of the National Academy of Sciences 120(30): e2305016120. https://doi.org/10.1073/pnas.2305016120 [확인: 서지 원문 대조]

Hagendorff, T. 2020. “The Ethics of AI Ethics: An Evaluation of Guidelines.” Minds and Machines 30(1): 99-120. https://doi.org/10.1007/s11023-020-09517-8

Hay, C. 2016. “International Relations Theory and Globalization.” In International Relations Theories. Oxford: Oxford University Press. https://doi.org/10.1093/hepl/9780198707561.003.0016 [확인: 편집자·쪽수]

Horowitz, M. C. 2018. “Artificial Intelligence, International Competition, and the Balance of Power.” Texas National Security Review 1(3).

Jobin, A., M. Ienca, and E. Vayena. 2019. “The Global Landscape of AI Ethics Guidelines.” Nature Machine Intelligence 1: 389-399. https://doi.org/10.1038/s42256-019-0088-2

Landis, J. R., and G. G. Koch. 1977. “The Measurement of Observer Agreement for Categorical Data.” Biometrics 33(1): 159-174.

Li, W., J. Shanahan, and Y. Liu. 2026. “Psychological Distance and Efficacy: Analyzing the Framing of Climate Change on US Agricultural News Websites Using LLM-Assisted Content Analysis.” Frontiers in Communication 11. https://doi.org/10.3389/fcomm.2026.1759296

Morse, J. C., and R. O. Keohane. 2014. “Contested Multilateralism.” Review of International Organizations 9(4): 385-412.

Reiss, M. V. 2023. “Testing the Reliability of ChatGPT for Text Annotation and Classification: A Cautionary Remark.” arXiv:2304.11085. [확인: 프리프린트, 게재본 여부]

Roberts, H., J. Cowls, J. Morley, M. Taddeo, V. Wang, and L. Floridi. 2021. “The Chinese Approach to Artificial Intelligence: An Analysis of Policy, Ethics, and Regulation.” AI & Society 36(1): 59-77.

Sayles, J. 2024. “Aligning AI Governance with Other Internal Governance Models for Trustworthy AI: ‘The Convergence of Governance Frameworks.’” In Principles of AI Governance and Model Risk Management, 113-172. https://doi.org/10.1007/979-8-8688-0983-5_5

Sazzed, S. 2026. “Eating Disorder-Related Content in Reddit Suicidal Ideation Posts: An LLM-Assisted Analysis of Mental Health Comorbidities, Substance Use, and Demographic Patterns.” Social Network Analysis and Mining. https://doi.org/10.1007/s13278-026-01647-8

Schmitt, L. 2022. “Mapping Global AI Governance: A Nascent Regime in a Fragmented Landscape.” AI and Ethics 2(2): 303-314. https://doi.org/10.1007/s43681-021-00083-y

Stix, C. 2022. “The Ghost of AI Governance Past, Present, and Future.” In The Oxford Handbook of AI Governance, 937-958. https://doi.org/10.1093/oxfordhb/9780197579329.013.56

Sulaiman, M. H., N. Muda, and F. A. Razak. 2025. “Impact of Data Types on Machine Learning Performance in LLM-Assisted Content Analysis (LACA) of Hospital Online Reviews.” JMIR Preprints. https://doi.org/10.2196/preprints.73984

Wang, L., and D. Poenaru. 2026. “Evaluative Stance Toward Artificial Intelligence in High-Quartile Medical Journals (2021–2026): Large-Scale LLM-Assisted Computational Content Analysis.” medRxiv. https://doi.org/10.64898/2026.07.23.26358815 [확인: 프리프린트 서버]

Ziems, C., W. Held, O. Shaikh, J. Chen, Z. Zhang, and D. Yang. 2024. “Can Large Language Models Transform Computational Social Science?” Computational Linguistics 50(1): 237-291. https://doi.org/10.1162/coli_a_00502 [확인: 서지 원문 대조]
