# 논문 2 B2: LLM 기반 내용분석 선행 연구 후보

검색일 2026-10-14. 웹 검색 결과 요약만 확인했고 원문 전체는 읽지 않았다. 인용 전 원문과 서지를 직접 확인해야 한다(특히 쪽수·권호).

## 1순위 (원고 인용 권장, 서지 확인 가능)

| 문헌 | 쓸 곳 | 근거 |
|---|---|---|
| Gilardi, F., Alizadeh, M., & Kubli, M. (2023). ChatGPT outperforms crowd workers for text-annotation tasks. *PNAS*, 120(30). DOI 10.1073/pnas.2305016120 | Ⅱ-2, Ⅲ-3: LLM 주석이 인간 주석을 대체·보완할 수 있다는 근거(프레임 탐지 포함) | 트윗·뉴스 6,183건. 무샷 정확도가 크라우드워커보다 평균 약 25%p 높고 코더 간 일치도도 높았다고 보고 |
| Reiss, M. V. (2023). Testing the reliability of ChatGPT for text annotation and classification: A cautionary remark. arXiv:2304.11085 (프리프린트) | Ⅲ-3, Ⅴ-3: 프롬프트 문구·반복에 따라 결과가 달라진다는 근거. 본 연구의 변형·반복 분류 설계를 정당화 | 문구를 조금 바꾸거나 같은 입력을 반복해도 출력이 달라지며 신뢰도 기준에 못 미치는 경우가 많다고 보고. 인간 주석 검증을 권고 |
| Ziems, C., Held, W., Shaikh, O., Chen, J., Zhang, Z., & Yang, D. (2024). Can large language models transform computational social science? *Computational Linguistics*, 50(1), 237–291. DOI 10.1162/coli_a_00502 | Ⅱ-2: 분류 과제에서 LLM은 최고 수준의 지도학습 모델에는 못 미치나 인간 주석자와 상당한 일치, '인간과 함께 쓰는 주석자'로의 활용 | 25개 영어 CSS 벤치마크에서 13개 모델 평가 |

## 2순위 (선택)

| 문헌 | 비고 |
|---|---|
| Törnberg, P. (2023). ChatGPT-4 outperforms experts and crowd workers in annotating political Twitter messages with zero-shot learning. arXiv:2304.06588 | 정치 텍스트 주석. 후속 저널판은 *Social Science Computer Review*(2025, 43권)로 보이나 호수·쪽수 미확인. 프리프린트와 저널판 중 어느 것을 인용할지 결정 필요 |
| Pangakis, N., Wolken, S., & Fasching, N. (2023). Automated annotation with generative AI requires validation. arXiv:2306.00176 | 검색 결과에 제목만 나옴. "LLM 주석은 반드시 인간 라벨로 검증해야 한다"는 본 연구의 타당화 설계와 맞음. 내용 미확인 |
| Kristensen-McLachlan 외 (2025). Are chatbots reliable text annotators? Sometimes. *PNAS Nexus* | 이진 주석에서 챗봇이 지도학습 분류기보다 못한 경우가 있다고 보고. 서지 세부(저자 전체, 권호) 미확인 |

## 최근 프리프린트(2026), 인용 신중
- 프롬프트의 개념 정의가 주석을 바꾼다는 연구(NeurIPS 2026 관련 항목), 프롬프트 간 신뢰도를 측정 문제로 다룬 연구(arXiv 2604.16413), 정치 텍스트 주석 파이프라인 선택의 영향 연구(arXiv 2603.26898)가 검색되었다. 본 연구의 정의문 변경 결과(κ 0.72)와 직접 연결되는 주제이나, 동료 심사 여부와 서지가 불확실하므로 원문 확인 후에 인용 여부를 정한다.

## 원고 반영 안 (확인 후 적용)
- Ⅱ-2 연구 공백 문단에 추가: "LLM을 텍스트 주석 도구로 쓰는 연구는 인간 주석과 견줄 만한 정확도를 보고하는 한편(Gilardi et al., 2023; Ziems et al., 2024), 프롬프트 문구와 반복에 따라 결과가 달라지므로 인간 라벨 검증이 필요하다고 경고한다(Reiss, 2023)."
- 이 연구들은 영어 소셜미디어 텍스트가 중심이다. 한국어 학술논문 초록에 대한 프레임 분류를 다룬 연구는 이번 검색에서 확인하지 못했다. 이 점은 연구 공백으로 쓸 수 있으나 "없다"고 단정하지 말고 "확인하지 못했다"로 쓴다.
