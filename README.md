# jcicaaa3

한국외국어대학교에서 컴퓨터공학을 전공하고, 동북아외교통상을 복수전공하고 있습니다.

최근에는 Windows 랜섬웨어 실행 파일을 분석하고 있습니다. 이전에 진행한 컴퓨터비전·머신러닝 프로젝트와 로봇 행동 평가 연구도 함께 정리하고 있습니다.

[개인 연구 사이트](https://jcicaaa3-cloud.github.io/) · [연구 글](https://jcicaaa3-cloud.github.io/research/) · [프로젝트](https://jcicaaa3-cloud.github.io/projects/)

## 랜섬웨어 분석

### Calipso (2026)

샘플의 SHA-256을 확인한 뒤 PE 헤더, 19개 섹션, 엔트리 포인트와 함수 참조를 조사했습니다. Ghidra에서는 `DeviceIoControl` 호출과 제어 코드 `0x900B3`(`FSCTL_ENUM_USN_DATA`)를 확인했습니다. 해당 호출의 역할과 다른 코드의 연관성은 계속 분석하고 있습니다.

- [정적 분석 기록](https://jcicaaa3-cloud.github.io/research/calipso-02/)
- [분석 화면](https://jcicaaa3-cloud.github.io/evidence/)
- [전체 연구 글](https://jcicaaa3-cloud.github.io/research/)

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

- 악성코드 분석: Ghidra, Python, PowerShell
- 머신러닝·컴퓨터비전: PyTorch, scikit-learn, OpenCV, NumPy, Pandas
- 개발·실험 환경: Git, Linux, FastAPI, Docker, GitHub Actions

## 연락

[개인 연구 사이트](https://jcicaaa3-cloud.github.io/) · [이메일](mailto:jcicaaa3@gmail.com)
