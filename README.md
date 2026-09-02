# Student Health Risk — EDA & Model Plan

Kaggle **Predicting Student Health Risk (Playground Series S6E7)** 프로젝트입니다.

## 현재까지 한 작업

- 학습 데이터 구조와 결측치 확인
- 목표값(`health_condition`)의 클래스 불균형 확인
- 주요 변수별 건강 상태 분포 시각화
- 기준 모델(HistGradientBoosting) 학습
- 성능 지표: Balanced Accuracy **0.9101**
- 다음 모델 후보: **TabPFN-3**, 비교 모델: **LightGBM**

## 핵심 EDA 결과

- 클래스 비율이 크게 불균형함
- 스트레스 수준, 수면 시간, 신체 활동 수준, BMI에서 건강 상태별 차이가 확인됨
- 일반 Accuracy보다 클래스별 성능을 균등하게 보는 Balanced Accuracy가 더 적절함

## 파일

- [EDA 및 모델링 계획 노트북](notebooks/01_seohyun_eda_model_plan.ipynb)
