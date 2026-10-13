# 토론·결론 및 초록 (논문 2 초안)

## 초록 (국문)

본 연구는 한국 학계의 AI 거버넌스 논의 중 '국가 전략·미중 경쟁' 토픽으로 분류된 KCI 학술논문 186편을 전수 대상으로, 학문분야에 따라 국제정치이론 프레임(현실주의·자유주의·구성주의)이 어떻게 달라지는지 비교하였다. 프레임 판정에는 사람 코더 대신 대규모 언어모델(LLM)을 분류 도구로 사용하는 자동 내용분석을 적용하고, 반복 분류와 두 가지 프롬프트 변형으로 안정성을 점검하였다. 분석 결과 같은 토픽이라도 분야에 따라 접근이 뚜렷이 달랐다. 정치외교학(73%)·지역학(72%)·군사학(86%)·정책학(91%)은 현실주의 프레임이 우세한 반면, 법학은 제도·규범을 강조하는 자유주의 프레임이 가장 많았고(46%) 현실주의는 29%에 그쳤다. 교육학은 대부분(90%) 어느 프레임에도 해당하지 않았다. 분야와 프레임의 연관 강도는 Cramér's V=0.39였다. 이러한 큰 방향은 분류 설정과 무관하게 유지되었으나 분야별 세부 비율, 특히 구성주의 비중은 설정에 민감하였다. 반복 분류의 일치도는 κ=0.81, 정의문 변경 시 κ=0.72였고 연구자 확정 라벨과의 일치는 제한적이었다. 본 연구는 AI 거버넌스 담론이 분야별로 다른 문제틀 위에서 전개됨을 보이고, LLM 기반 프레임 분류의 가능성과 한계를 함께 제시한다.

**주제어:** AI 거버넌스, 프레임 분석, 학문분야, 국제정치이론, LLM 기반 내용분석

## Abstract

Using all 186 Korean journal articles (KCI) assigned to the "national strategy and US–China competition" topic of AI governance, this study compares how academic disciplines frame the same issue through realist, liberal, and constructivist perspectives. Frames were coded by a large language model (LLM) as an automated content-analysis tool, and stability was checked by a blind repeat and two prompt variations. Disciplines differed markedly: realism dominated political science/diplomacy (73%), area studies (72%), military studies (86%), and policy studies (91%), while law favored a liberal, rules-and-institutions frame (46%) over realism (29%); most education papers (90%) fit none of the frames. Association between discipline and frame was moderate (Cramér's V = 0.39). The broad pattern held across all classification settings, but disciplinary percentages, particularly for constructivism, were sensitive to prompt wording (repeat κ = 0.81; reworded definitions κ = 0.72), and agreement with researcher-confirmed labels was limited. The study shows that AI governance discourse is built on different problem frames across disciplines and reports both the promise and limits of LLM-based frame classification.

**Keywords:** AI governance, framing, academic disciplines, international relations theory, LLM-assisted content analysis

## 논의 및 결론

### 1. 발견의 의미

같은 '국가 전략·미중 경쟁' 토픽 안에서도 학문분야가 논거의 중심을 다르게 설정한다는 점이 확인되었다. 안보·국제정치 계열은 AI를 국가 간 경쟁과 안보의 대상으로 다루는 현실주의 문제틀을 따르고, 법학은 같은 경쟁 상황을 규제와 제도 설계의 문제로 옮겨 다룬다. 이는 AI 거버넌스 담론이 하나의 공통 논의가 아니라 분야별 문제 정의 위에서 병렬로 전개되고 있음을 시사한다. 논문 1이 보인 뉴스와 학계의 프레임 차이(학계는 구성·자유 비중이 높다)는 학계 내부의 이질성이 부분적 원인일 수 있다는 해석의 단서도 제공한다. 다만 두 연구의 대상과 방법이 다르므로 직접 비교는 하지 않았다.

### 2. 정책·학술적 함의

- 정책적으로 안보 중심 논의와 제도·규범 중심 논의가 서로 다른 분야에서 생산되므로, 국가 전략을 수립할 때 두 계열의 지식이 연결되는 경로가 필요하다.
- 학술적으로 학제간연구에서 구성주의 프레임이 상대적으로 높게 나타난 점은 후속 연구에서 본문 수준 분석으로 확인할 만하다.

### 3. 방법론적 시사점과 한계

- LLM 분류는 같은 코드북에서 안정적이었으나(κ≈0.80) 정의문이 바뀌면 구성주의 경계가 크게 움직였다. 따라서 LLM 기반 프레임 분석은 수치 하나가 아니라 설정별 범위로 보고해야 한다.
- 연구자 확정 라벨 10편 중 6–7편만 일치하여 사람 기준 타당도는 충분히 입증되지 않았다. 반복 분류는 신뢰도일 뿐 타당도를 보증하지 않으며 체계적 편향은 재현된다.
- 제목·초록 기반 분류이고, KCI 코퍼스와 LDA 배정에 의존하며, 소규모 분야(n<15)의 비율은 불안정하다. 결과는 이 코퍼스에 한정된 기술적 모수이다.
- 후속 연구는 사람 코더 다수와의 대조, 본문 수준 분석, 복수 모델 비교가 필요하다.

### 4. 결론

한국 학계는 AI 거버넌스의 국가 전략 문제를 분야에 따라 현실주의적 경쟁 논리, 제도·규범 설계, 또는 프레임 바깥의 응용 문제로 서로 다르게 다루고 있다. 이 분야 간 차이는 분류 설정을 바꾸어도 큰 방향이 유지되는 반면, 세부 수치는 범위로 해석해야 한다.

---
**투고 전 확인할 사항:** (1) 논문 1과의 코퍼스 중복 및 관계 명시, (2) 학술지의 생성형 AI 사용 규정에 따른 방법 절·투고 양식 기재, (3) 모델 식별자와 프롬프트 전문의 부록 수록, (4) 사람 코더 대조 보강 여부.
