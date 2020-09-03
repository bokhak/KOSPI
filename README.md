# Kospi
2019 미래에셋대우 대학생 디지털 금융페스티벌 - 빅데이터 페스티벌 - 과제2_국면분석
## 대회 개요
- [2019 미래에셋대우 대학생 디지털 금융 페스티벌 - 빅데이터 페스티벌](https://www.miraeassetdaewoo.com/hki/hki7110/n03_1.do)
  - 주최: [미래에셋대우](https://www.miraeassetdaewoo.com/hki/hki7110/n01.do)
  - 대회기간: 2019.09.23(월) ~ 2019.11.08(금)
  - 팀명: 복학러들

## 과제 개요
### 과제2_국면분석
주어진 데이터를 바탕으로 **5일 후 코스피 지수종가 예측**

#### 문제 정의
- 국면 예측: 5일 대비 **상승**/**하락** [**분류 Classification**]

#### [데이터](data/README.md)
> 데이터 사용 규정으로 인해 데이터 삭제
  - Train Data: kospi_train  economic_train  exchange_train  market_train  per_train
  - Test Data: kospi_test  economic_test  exchange_test  market_test  per_test
  
## 문제 해결 프로세스
1. 데이터 확인
  - [전체 데이터](01_문제접근_데이터탐색.ipynb)
  - [kospi 데이터](01_문제접근_kospi_탐색.ipynb)
2. [EDA](02_EDA_economic.csv)
3. [Preprocessing](03_preprocessing_cleaning.ipynb)
4. Feature Engineering
  - [변수 축소](04_변수축소_market.ipynb)
  - [데이터 병합](04_최종데이터전처리_with_rf_ nn.ipynb)
5. Modeling
  - 접근 방식 2가지
    - Classification: 문제 정의에 따른 classification model 사용
      1. [Random Forest](classification_1.random forest.ipynb)
      2. [SVM](classification_2.SVM.ipynb)
      3. [LGBM](classification_3.LightGBM.ipynb)
      4. [Stacking](classification_4. stacking.ipynb)
    - Regression: 5일 후 지수종가를 시계열 예측
      1. [LSTM](05_Time_Series_Reg_LSTM.ipynb)
      2. [GRU](05_Time_Series_Reg_GRU.ipynb)
6. Evaluation
  - 성능평가: F1 score
7. Conclusion
