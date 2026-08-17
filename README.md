<div align="center">

# 김다연 · Dayeon Kim

**추론 알고리즘을 직접 구현하고, 그 모델로 센서 · 텍스트 · 교통 데이터를 분석합니다**

고려대학교 세종캠퍼스 빅데이터사이언스학과 석사과정 · 졸업예정 2027.02

<br>

### [📂 포트폴리오 보기 → kim-da-yeon.github.io](https://kim-da-yeon.github.io/)

[![포트폴리오](https://img.shields.io/badge/포트폴리오-kim--da--yeon.github.io-5A2B47?style=for-the-badge)](https://kim-da-yeon.github.io/)
[![이력서](https://img.shields.io/badge/이력서-PDF-14706A?style=for-the-badge)](https://kim-da-yeon.github.io/resume.pdf)
[![Email](https://img.shields.io/badge/Email-dayun0405@korea.ac.kr-16211E?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dayun0405@korea.ac.kr)

</div>

---

## 무엇을 하는 사람인지

베이지안 계산과 텍스트 모델링 사이에서 일합니다. 어려운 사후분포의 모드에 **실제로
도달하는 표집기**를 설계하고, **데이터가 생성된 방식을 반영하는 구조**의 모델을 만듭니다.

- **Stochastic-gradient MCMC** — SGLD · SGHMC와 적응적 가중 변형. 미니배치 gradient 표집이 적응적 최적화기를 언제 이기고 언제 못 이기는지를 통제된 환경과 실데이터 양쪽에서 확인해 왔습니다.
- **순차적 토픽 모델** — 문서를 교환 가능한 토픽 주머니가 아니라 문장 간 전이 네트워크로 모델링합니다. 이상반응 보고서나 사고 서술문처럼 문서 자체가 인과 사슬로 읽히는 데이터에서 의미가 있습니다.
- **LLM 데이터를 정직하게 평가하기** — LLM 생성 데이터가 실제로 무엇에 쓸 만한지에 관심이 있습니다. 표준 정규화가 상호운용성은 크게 올리지만 추천 정확도에는 유의한 변화를 주지 않았다는 결과를, 양쪽 다 보고했습니다.

## 논문

전부 제1저자. 동일 모델(TNTM)의 제약을 단계적으로 해제한 연속 연구입니다.

| 논문 | 게재 |
|---|---|
| AWSGLD를 이용한 전이 네트워크 토픽 모델 추론 | 한국자료분석학회지 28(1) 109–121 · 2026 |
| 자율주행 도메인에서 LoRA 기반 sLLM 파인튜닝 | 한국자료분석학회지 27(3) 769–780 · 2025 |
| Fixed-K Shrinkage BNTM with AWSGLD Inference | 한국자료분석학회 하계학술발표대회 포스터논문 **장려상** · 2026 |
| Fixed-K Shrinkage BNTM with AWSGHMC Inference | SCI급 학술지 투고 중 · 석사 학위논문 |

## 참여 연구

| 과제 | 역할 |
|---|---|
| TNTM을 활용한 임베디드 시스템 기술 문서의 주제 흐름 분석 (한국연구재단 석사과정생연구장려금, RS-2025-25437035) | **연구책임자** |
| 베이지안 추론을 위한 적응적 가중 SGMCMC 알고리즘 (한국연구재단, RS-2024-00352792) | 참여연구원 |
| 초격차산업기반 표준전문인력양성 (KIAT, RS-2025-02215617) | 참여연구원 |

## 코드

| 저장소 | 한 줄 |
|---|---|
| [**llmrec-metadata-standard**](https://github.com/Kim-Da-yeon/llmrec-metadata-standard) | LLM 생성 메타데이터의 ISO 3166-1 / BCP 47 정규화. 한 국가가 1,166개 표면형으로 흩어진 것을 57개 표준 코드로 통합해 상호운용성 0 → **80.3%**. 추천 정확도에는 유의한 변화 없음도 함께 보고 |
| [**GCIoU-SGMCMC-3D-Detection**](https://github.com/Kim-Da-yeon/GCIoU-SGMCMC-3D-Detection) | SGLD·SGHMC·SGNHT를 Adam과 동일한 GCIoU 손실 아래 비교. 학습 손실이 가장 낮은 표집기가 검출 성능은 최고가 아니었고, 모멘텀 유무가 성능을 갈랐습니다 |
| [**SONY_Chatbot**](https://github.com/Kim-Da-yeon/SONY_Chatbot) | 제품 설명서 대상 한국어 RAG. bge-m3 + Chroma 검색에 **페이지 단위 출처**를 붙여 답변 근거를 특정 페이지까지 되짚습니다 |
| [**mcmc-r-packages**](https://github.com/Kim-Da-yeon/mcmc-r-packages) | 확률적 근사 몬테카를로를 순수 R · C/Rcpp · Python/reticulate 세 백엔드로 각각 R 패키지화 |
| [**Pykachu-Volleyball**](https://github.com/Kim-Da-yeon/Pykachu-Volleyball) | gymnasium 환경 표 기반 Q-learning. 희소 보상을 밀집 보상으로 재설계 |
| `bntm-topic-model` | 석사 학위논문 코드 — 심사 중 비공개, 게재 후 공개 예정 |

## 도구

![Python](https://img.shields.io/badge/Python-16211E?style=flat-square&logo=python&logoColor=white)
![R](https://img.shields.io/badge/R-16211E?style=flat-square&logo=r&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-16211E?style=flat-square&logo=pytorch&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-16211E?style=flat-square&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-16211E?style=flat-square&logo=scikitlearn&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-16211E?style=flat-square&logo=mysql&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-16211E?style=flat-square)
![Rcpp](https://img.shields.io/badge/Rcpp-16211E?style=flat-square)
![QGIS](https://img.shields.io/badge/QGIS-16211E?style=flat-square&logo=qgis&logoColor=white)

---

<div align="center">
<sub>저장소 대부분에 <b>Limitations</b> 절이 있습니다. 장식이 아니라, 재현되지 않은 결과는 그렇다고 적어둔 것입니다.</sub>
</div>
