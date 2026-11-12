# jcicaaa3

[English](README.md) · [日本語](README_JA.md)

한국외국어대학교에서 컴퓨터공학을 전공하고, 동북아외교통상을 복수전공하고 있습니다. 보안과 머신러닝을 같이 공부합니다. Windows 랜섬웨어를 분석하고 있고, 머신러닝 기반 악성코드 탐지를 시작하는 단계입니다.

[사이트](https://jcicaaa3-cloud.github.io/) · [글](https://jcicaaa3-cloud.github.io/research/) · [프로젝트](https://jcicaaa3-cloud.github.io/projects/) · [jcicaaa3@gmail.com](mailto:jcicaaa3@gmail.com)

## 악성코드 분석

### Calipso 랜섬웨어 (2026)

Ghidra로 정적 분석했습니다. 글에는 암호화 구조(파일 앞 5MB를 XChaCha20으로 암호화하고 세션 키를 RSA-4096 OAEP로 감쌈), MFT를 직접 열거하는 파일 탐색(`FSCTL_ENUM_USN_DATA`), 섀도 복사본·이벤트 로그 삭제 같은 복구 방해 동작, 그리고 IOC·YARA 룰·MITRE ATT&CK 매핑을 정리했습니다.

[분석 v2.0](https://jcicaaa3-cloud.github.io/research/calipso-v2/) · [분석 화면](https://jcicaaa3-cloud.github.io/evidence/)

악성코드 샘플은 공개 저장소에 올리지 않습니다.

## 프로젝트

### [LiteRaceSegNet](https://github.com/jcicaaa3-cloud/LiteRaceSegNet-FINAL-)

경계 헤드를 둔 파라미터 0.125M짜리 도로 손상 세그멘테이션 CNN입니다. 검증 mIoU는 10장 기준 0.807, CUDA에서 3.1 ms/장이고, 변형 7개로 ablation을 했습니다. 가장자리 품질은 아직 약하고(테스트 경계 F1 0.058), README에도 그렇게 적었습니다.

### [HPLS-Eval](https://github.com/jcicaaa3-cloud/HPLS-Eval-v0.2.7)

작은 마스크 세그멘테이션을 런타임(CPU, GPU, NPU, TPU)과 정밀도(FP32, FP16, INT8)를 바꿔 가며 평가하는 도구입니다. 실제로 어느 실행 프로바이더에서 돌았는지, INT8 모델이 정말 양자화됐는지 확인합니다.

### [Financial Risk Scoring](https://github.com/jcicaaa3-cloud/financial-risk-scoring-service-FINAL)

기업의 분기 데이터로 다음 분기의 리스크 세 가지를 점수로 내는 ML 백엔드입니다. 입력 검증, 시간 순서를 지키는 평가, FastAPI, 모니터링 리포트가 들어 있습니다. 데이터는 합성 데이터만 씁니다.

### [MachiLens](https://github.com/jcicaaa3-cloud/machilens-shibuya-ai-predictor)

시부야 도시전략 시나리오를 합성 데이터로 비교하는 BiLSTM 모델입니다. 수업 때 낸 기획을 다시 만들었습니다. 랜덤 포레스트 베이스라인이 더 잘 나왔고, README에 둘 다 적었습니다.

### 로봇 행동 성공·실패 평가

로봇이 작업을 해냈는지를 어떤 기준으로 판정할지 조사한 2026년 1학기 연구 프로젝트입니다. 80회 실험에서 나온 874건을 분석하고, 판정 기준에 따라 결과가 어떻게 달라지는지 봤습니다. [요약](https://jcicaaa3-cloud.github.io/projects/robot-evaluation/)

## 사용한 도구

- 악성코드 분석: Ghidra, YARA, MITRE ATT&CK, Python, PowerShell
- 머신러닝·컴퓨터비전: PyTorch, scikit-learn, OpenCV, NumPy, Pandas
- 개발: Git, Linux, FastAPI, Docker, GitHub Actions

## 연락

[jcicaaa3@gmail.com](mailto:jcicaaa3@gmail.com)
