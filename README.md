# Wonseok Kim

**Computer Vision / ML Engineer**

경량 컴퓨터 비전 모델을 설계하고, 실험 결과를 검증하여 API와 데모 형태로 연결합니다.
모델 성능만 제시하는 것이 아니라 데이터 검증, 정량 평가, 추론 속도 측정, 서비스 연동까지 직접 구현하는 것을 목표로 합니다.

* Hankuk University of Foreign Studies
* Computer Engineering
* Double Major in Northeast Asian Diplomacy and Commerce
* Focused on Computer Vision, ML Evaluation, and Deployment

---

## Featured Project

### [LiteRaceSegNet](https://github.com/jcicaaa3-cloud/literacesegnet)

Lightweight boundary-aware network for road-damage semantic segmentation.

도로 손상 영역의 경계 정보가 경량 모델에서 손실되는 문제를 분석하고, detail/context feature와 boundary-guided fusion을 적용한 세그멘테이션 모델입니다.

| Metric       |         Result |
| ------------ | -------------: |
| mIoU         |         0.8072 |
| Damage IoU   |         0.7113 |
| Parameters   |         0.125M |
| CUDA Latency | 3.097 ms/image |

### What I Built

* 경량 도로 손상 세그멘테이션 모델 설계 및 구현
* 이미지와 마스크의 파일명, 해상도, 누락 여부를 검사하는 데이터 검증 과정 구축
* mIoU, Damage IoU, 추론 지연시간 기반 성능 평가
* 구조 및 손실 함수 변경에 따른 ablation experiment 수행
* PyTorch 모델을 FastAPI 추론 API 및 웹 데모와 연동
* 예측 마스크, overlay 이미지 및 정량 결과를 활용한 시각적 검증

### Tech Stack

`Python` `PyTorch` `OpenCV` `NumPy` `Semantic Segmentation` `FastAPI`

---

## Selected Project

### [Financial Risk Scoring Service](https://github.com/jcicaaa3-cloud/financial-future-prediction-service)

Structured-data ML service for estimating future financial deterioration risk.

단순 모델 학습에 그치지 않고 데이터 처리, 시간 순서 기반 검증, API 추론, batch scoring 및 monitoring artifact까지 연결한 ML 엔지니어링 프로젝트입니다.

### Key Features

* 시간 순서를 고려한 train/validation 분리
* 데이터 누수를 방지하기 위한 feature generation
* FastAPI 기반 단건 추론 API
* batch scoring pipeline
* Docker 실행 환경
* GitHub Actions 기반 자동 테스트
* synthetic data 사용 범위와 프로젝트 한계 명시

### Tech Stack

`Python` `FastAPI` `scikit-learn` `Pandas` `Docker` `GitHub Actions`

---

## Engineering Approach

프로젝트를 진행할 때 다음 과정을 중요하게 생각합니다.

### 1. Validate the Data

모델을 학습하기 전에 데이터 파일의 누락, 이름 불일치, 해상도 차이, 잘못된 mask value를 먼저 검사합니다.

### 2. Measure the Result

정확도 하나만 제시하지 않고 task-specific metric, latency, parameter count와 qualitative result를 함께 확인합니다.

### 3. Analyze Failures

평균 성능뿐 아니라 작은 손상 영역, 불명확한 경계, 복잡한 배경 등 모델이 실패하는 조건을 분석합니다.

### 4. Connect the Model

학습된 모델을 추론 API와 웹 데모로 연결하여 실제 입력과 출력 흐름을 검증합니다.

### 5. Document the Evidence

실험 설정, 평가 조건, 결과 이미지, 한계점을 문서화하여 결과를 재현하고 검토할 수 있도록 정리합니다.

---

## Technical Skills

### AI / Machine Learning

* Python
* PyTorch
* OpenCV
* NumPy
* Pandas
* scikit-learn
* Semantic Segmentation
* Object Detection
* Model Evaluation
* Ablation Study

### Backend / Deployment

* FastAPI
* REST API
* Docker
* GitHub Actions
* AWS
* Linux
* GitHub Pages

### Development

* Git
* GitHub
* JavaScript
* HTML
* CSS
* WSL

---

## Education

**Hankuk University of Foreign Studies**

* Major: Computer Engineering
* Double Major: Northeast Asian Diplomacy and Commerce

---

## Languages

* Korean
* English
* Japanese

---

## Current Focus

현재는 Vision-Language-Action 에이전트의 실행 실패를 감지하고 복구하는 외부 검증 계층을 연구하고 있습니다.

주요 관심 분야는 다음과 같습니다.

* Vision-Language-Action agents
* Robot action failure detection
* World-state verification
* Recovery planning
* Robustness evaluation under environmental perturbations

연구 결과와 재현 가능한 실험 코드가 정리되면 별도의 공개 저장소로 제공할 예정입니다.

---

## Contact

프로젝트와 구현 세부 내용은 각 저장소의 README 및 실험 문서에서 확인할 수 있습니다.
