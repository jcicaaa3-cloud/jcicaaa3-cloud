# Wonseok Kim

**Cybersecurity · Malware Analysis · Ransomware Research**  
Computer Engineering Undergraduate @ Hankuk University of Foreign Studies (HUFS)

악성코드가 **무엇을 실행하고, 어떤 흔적을 남기며, 어떻게 탐지할 수 있는지**에 관심이 있습니다.
현재 컴퓨터보안(Computer Security)을 수강하고 있으며, 랜섬웨어의 정적 분석과 행위 기반 분석을 중심으로 개인 연구를 준비하고 있습니다.

이전에는 컴퓨터비전 및 머신러닝 프로젝트에서 모델 개발, 실험 검증, 추론 API 구현을 경험했습니다. 이제는 그 경험을 보안 분석과 위협 탐지에 연결하고자 합니다.

---

##  Current Focus — Cybersecurity

| 분야 | 현재 관심 및 학습 방향 |
| --- | --- |
| **Malware Analysis** | 실행 파일 구조, 문자열, 함수 흐름 및 악성 행위 이해 |
| **Ransomware Behavior** | 파일 변경·암호화 과정, 복구 방해 행위 및 IOC 분석 |
| **Computer Security** | AES·RSA 등 암호학 기초, 디지털 서명, 시스템 보안 |
| **Threat Detection** | 공개 분석 자료와 관찰 가능한 행위를 기반으로 탐지 근거 검토 |
| **AI for Security** | 기존 ML 개발·성능 평가 경험을 악성 행위 탐지 연구에 적용 |

> 현재 보안 분야는 학습 및 개인 연구 단계입니다. 분석을 완료하지 않은 샘플이나 검증하지 않은 결과를 연구 성과로 표기하지 않았습니다.

##  Research Notes — In Progress

### Calipso Ransomware (2026) — 공개 분석 자료 검토

- 공개적으로 보고된 Windows x64 샘플 정보 및 해시 조사
- 공개 샌드박스 보고서에서 프로세스 실행, 파일 변경, 복구 방해 행위 검토
- 분석 자료의 관찰 사실과 추정 사항을 구분해 기술 노트 작성 예정

**Reference:** [Hatching Triage public report](https://tria.ge/261006-nzbfjaay5m)

### Behavioral Ransomware Detection — 학습 및 프로젝트 방향

- 행위 데이터의 특성과 악성코드 탐지 연구 검토
- 공개 데이터셋 및 기존 모델의 재현성과 평가 방법 학습
- 참고 연구: [MLRan dataset and research code](https://github.com/faithfulco/mlran)

분석 결과는 확인 가능한 근거와 함께 공개할 예정입니다. 당연하지만 실행 가능한 악성코드 원본이나 피해자 데이터는 이 프로필 저장소에 게시하지 않습니다. 

---

##  Previous Work — AI / Machine Learning

AI 연구 경험은 보안 분야에서도 활용할 수 있는 기술적 기반입니다.

### [LiteRaceSegNet](https://github.com/jcicaaa3-cloud/LiteRaceSegNet-FINAL-)

경량 도로 손상 세그멘테이션 모델 개발 및 정량 평가. 데이터 검증, ablation, 추론 성능 측정, FastAPI 연동을 포함합니다.

| Metric | Recorded Result |
| --- | ---: |
| mIoU | **0.8072** |
| Damage IoU | **0.7113** |
| Parameters | **0.125M** |
| CUDA Latency | **3.097 ms/image** |

### [Financial Risk Scoring Service](https://github.com/jcicaaa3-cloud/financial-risk-scoring-service-FINAL)

정형 데이터 기반 머신러닝 엔지니어링 프로젝트. 시간 순서 기반 검증, 데이터 누수 방지, FastAPI, 배치 추론 및 Docker/CI를 다룹니다. **합성 데이터 기반 포트폴리오**로서 실제 투자 예측 성능을 주장하지 않습니다.

---

##  Technical Background

**Security (studying):** Computer Security · Cryptography · Malware Analysis · Ransomware Behavior · Threat Detection  
**Programming & ML (project experience):** Python · PyTorch · scikit-learn · NumPy · Pandas · OpenCV  
**Engineering:** Git · GitHub · FastAPI · Docker · GitHub Actions · Linux

##  How I Work

1. **Verify** — 공개 출처, 해시, 파일 형식과 실험 조건을 먼저 확인합니다.
2. **Observe** — 실제 관찰된 행위와 해석·가설을 구분합니다.
3. **Evaluate** — 결과뿐 아니라 오류, 실패 조건과 재현 가능성을 검토합니다.
4. **Document** — 분석 절차, 근거, 한계점을 한국어 기술 문서로 정리합니다.
5. **Handle Safely** — 악성코드는 허가된 격리 환경에서만 다루며 원본 샘플을 공개 저장소에 배포하지 않습니다.

##  Education

**Hankuk University of Foreign Studies**  
Computer Engineering · Double Major in Northeast Asian Diplomacy and Commerce  
Current coursework includes **Computer Security**.

##  Languages & Contact

Korean · Japanese · English  
[GitHub](https://github.com/jcicaaa3-cloud) · [LinkedIn](https://www.linkedin.com/in/%EA%B9%80%EC%9B%90%EC%84%9D-wonseok-kim-1ab559407/)

---

*From AI research to cybersecurity — learning through evidence, analysis, and reproducible experiments.*
