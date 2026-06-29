# Basketball Position Classification

농구 선수의 경기 기록을 이용해 포지션을 분류하는 머신러닝 프로젝트입니다.

## Problem

선수의 `3P`, `TRB`, `BLK` 기록만으로 포지션(`SG`, `C`)을 예측합니다. 데이터 수가 작기 때문에 성능 수치 자체보다 feature 분포를 확인하고 KNN/SVM 모델을 비교하는 과정을 강조했습니다.

## Data

- Train: 80 rows
- Test: 20 rows
- Features: `3P`, `TRB`, `BLK`
- Target: `Pos`

## Models

- KNN
- Linear SVM
- RBF SVM

## Evaluation

- Test Accuracy
- Classification Report
- Confusion Matrix

## What This Shows

- 거리 기반 모델에서 스케일링이 필요한 이유
- 작은 데이터셋에서 평가 지표를 조심스럽게 해석하는 태도
- KNN과 SVM의 모델 특성 비교

## Files

- `basketball_position_classification.ipynb`: 정리된 분석 노트북
- `data/basketball_train.csv`: 학습 데이터
- `data/basketball_test.csv`: 테스트 데이터
