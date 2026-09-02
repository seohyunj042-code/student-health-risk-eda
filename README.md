# Student Health Risk — EDA & Model Comparison

Kaggle **Predicting Student Health Risk (Playground Series S6E7)** 프로젝트입니다.

## 현재까지 한 작업

- 학습 데이터 구조와 결측치 확인
- 목표값(`health_condition`)의 클래스 불균형 확인
- 숫자형·범주형 변수와 건강 상태의 관계 시각화
- 범주형 변수 6개의 Cramér's V 비교
- 동일한 80:20 Stratified 홀드아웃에서 두 모델 비교

## 핵심 결과

- `at-risk`가 85.87%로 클래스 불균형이 심함
- 스트레스 수준, 수면 시간, 신체 활동 수준, BMI에서 건강 상태별 차이가 확인됨
- HistGradientBoosting Balanced Accuracy: **0.9101**
- LightGBM Balanced Accuracy: **0.9498**
- 같은 검증 행에서 LightGBM이 **3.97%p** 높은 성능을 기록해 현재 주 모델로 선정

## 다음 단계

공개 TabPFN-3 구현의 Kaggle 점수는 0.94688이지만 평가 데이터가 다르므로 위 로컬 점수와 직접 비교하지 않습니다. Kaggle GPU에서 동일한 20% 검증 세트로 추가 확인할 예정입니다.

## 파일

- [EDA 및 모델 비교 노트북](notebooks/01_seohyun_eda_model_plan.ipynb)
