# Kospi
2019 미래에셋대우 대학생 디지털 금융페스티벌 - 빅데이터 페스티벌 - 과제2_국면분석
## 대회 개요
- [2019 미래에셋대우 대학생 디지털 금융 페스티벌 - 빅데이터 페스티벌](https://www.miraeassetdaewoo.com/hki/hki7110/n03_1.do)
  - 주최: [미래에셋대우](https://www.miraeassetdaewoo.com/hki/hki7110/n01.do)

## 과제 개요
### 과제2_국면분석
주어진 데이터를 바탕으로 **5일 후 코스피 지수종가 예측**

#### 문제 정의
- 국면 예측: 5일 대비 **상승**/**하락** [**분류 Classification**]

#### 데이터
  - Independent Vars.
  - Response Vars.
  
## 문제 해결 프로세스
1. 데이터 확인
2. EDA
3. Feature Engineering
4. Modeling
  - 접근 방식 2가지
    - Classification: 문제 정의에 따른 classification model 사용
      1. Adaboost
      2. Random Forest
      3. Logistic Regression
      4. Stacking
    - Regression: 5일 후 지수종가를 시계열 예측
      1. LSTM
      2. GRU
5. Evaluation
  - 성능평가: F1 score
6. Conclusion
  


