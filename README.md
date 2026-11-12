# jcicaaa3

한국외국어대학교에서 컴퓨터공학을 전공하고, 동북아외교통상을 복수전공하고 있습니다.

최근에는 Windows 랜섬웨어를 분석하고, 머신러닝 기반 악성코드 탐지를 준비하고 있습니다. 이전에 진행한 컴퓨터비전·머신러닝 프로젝트와 로봇 행동 평가 연구도 함께 정리하고 있습니다.

[개인 연구 사이트](https://jcicaaa3-cloud.github.io/) · [연구 글](https://jcicaaa3-cloud.github.io/research/) · [프로젝트](https://jcicaaa3-cloud.github.io/projects/)

## 랜섬웨어 분석

### Calipso (2026)

Ghidra로 정적 분석했습니다. XChaCha20으로 파일 앞 5MB를 암호화하고 세션 키를 RSA-4096(OAEP)으로 감싸는 구조, MFT 직접 열거(`FSCTL_ENUM_USN_DATA`)로 파일을 찾는 방식, 섀도 복사본 삭제·이벤트 로그 삭제 같은 복구 방해 동작을 정리하고 IOC, YARA 룰, MITRE ATT&CK 매핑을 만들었습니다.

- 분석 v2.0: [한국어](https://jcicaaa3-cloud.github.io/research/calipso-v2/) · [English](https://jcicaaa3-cloud.github.io/en/research/calipso-v2/) · [日本語](https://jcicaaa3-cloud.github.io/ja/research/calipso-v2/)
- [분석 화면](https://jcicaaa3-cloud.github.io/evidence/) · [전체 연구 글](https://jcicaaa3-cloud.github.io/research/)

악성코드 원본은 공개 저장소에 올리지 않습니다.

## 프로젝트

### [LiteRaceSegNet](https://github.com/jcicaaa3-cloud/LiteRaceSegNet-FINAL-)

도로 균열과 포트홀을 분할하는 경량 세그멘테이션 모델입니다. 데이터 검증부터 모델 구현, 비교 실험, 추론 API 연동까지 진행했습니다.

- mIoU: **0.8072**
- Parameters: **0.125M**
- CUDA latency: **3.097 ms/image**

[프로젝트 정리](https://jcicaaa3-cloud.github.io/projects/literacesegnet/)

### [Financial Risk Scoring](https://github.com/jcicaaa3-cloud/financial-risk-scoring-service-FINAL)

합성 재무 데이터를 사용해 데이터 처리, 시간 순서에 따른 모델 검증, FastAPI 예측 API 및 배치 추론 기능을 구현한 프로젝트입니다. 실제 투자 성과를 예측하는 서비스는 아닙니다.

[프로젝트 정리](https://jcicaaa3-cloud.github.io/projects/financial-risk/)

### 로봇 행동 성공·실패 평가

로봇이 수행한 작업을 어떤 기준으로 성공 또는 실패로 판단할 수 있는지 조사한 연구 프로젝트입니다(2026년 1학기). 80회 실험에서 나온 874건의 사례를 분석하고, 판정 기준에 따라 결과가 달라지는 문제를 살펴봤습니다.

[연구 요약](https://jcicaaa3-cloud.github.io/projects/robot-evaluation/)

## 사용한 도구

- 악성코드 분석: Ghidra, YARA, MITRE ATT&CK, Python, PowerShell
- 머신러닝·컴퓨터비전: PyTorch, scikit-learn, OpenCV, NumPy, Pandas
- 개발·실험 환경: Git, Linux, FastAPI, Docker, GitHub Actions

## 연락

[개인 연구 사이트](https://jcicaaa3-cloud.github.io/)
