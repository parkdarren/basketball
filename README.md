# Basketball Position Classification

농구 선수의 경기 기록을 이용해 포지션을 분류한 머신러닝 프로젝트입니다. 데이터 규모가 크지는 않지만 적은 feature만으로도 포지션 간 차이가 어떻게 드러나는지 확인하고 KNN과 SVM 모델을 비교했습니다.

## 문제 정의

3점슛과 리바운드 및 블록 기록을 바탕으로 선수 포지션을 예측합니다.

- Train: 80 rows
- Test: 20 rows
- Features: `3P`·`TRB`·`BLK`
- Target: `Pos` (`SG`·`C`)

## 분석 흐름

- 포지션별 `3P`·`TRB`·`BLK` 분포 확인
- pair plot과 box plot으로 feature 차이 탐색
- 거리 기반 모델을 위해 StandardScaler 적용
- KNN과 SVM 모델 비교
- Accuracy·classification report·confusion matrix 확인

## 사용 모델

- KNN (`k=3`·`k=5`)
- Linear SVM
- RBF SVM

## 사용 기술

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 파일 구성

```text
basketball_position_classification.ipynb
data/
  basketball_train.csv
  basketball_test.csv
```

## 정리

이 프로젝트는 작은 데이터셋에서 모델 성능 수치만 크게 보이게 만드는 것보다 feature 분포와 모델 특성을 함께 해석하는 데 초점을 둔 작업입니다. KNN처럼 거리 기반으로 판단하는 모델에서 스케일링이 왜 필요한지도 확인할 수 있습니다.
