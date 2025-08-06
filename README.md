[우유 맛 예측을 위한 K-최근접 이웃 및 선형 회귀 분석 - pH, 온도, 색상 변수의 영향]
**프로젝트 수행일: 07.10 ~ 0811**

**Tool: colab**

**Language: python**

데이터 처리 pandas
데이터프레임을 다루는 데 사용. CSV 파일을 읽어들여 데이터셋을 처리.
파일 업로드 Google Colab
데이터를 Google Colab에 업로드하여 분석.
데이터 분할 train_test_split (from sklearn.model_selection)
데이터를 학습 세트와 테스트 세트로 나누는 데 사용. train_size=0.7로 학습 데이터는 70%, 테스트 데이터는 30%로 분리.
데이터 정규화 Normalizer (from sklearn.preprocessing)
독립변수(X)에 대해 정규화를 진행. 모든 특성들이 같은 범위 내에서 비교될 수 있도록 변환.
K-최근접 이웃 회귀 (KNN Regression) KNeighborsRegressor (from sklearn.neighbors)
K-최근접 이웃 알고리즘을 사용해 회귀 모델을 학습. 여러 k 값에 대해 모델을 학습시키고, 훈련 세트와 테스트 세트에 대한 예측 성능(R²)을 비교. 최적의 k값을 선택하여 예측.
선형 회귀 OLS (from statsmodels.api)
선형 회귀 분석을 위해 사용. X_train에 대해 선형 회귀 모델을 학습하고, Taste에 대한 예측 모델을 만들었음. 회귀 계수를 통해 각 독립변수가 Taste에 미치는 영향을 분석. p-value를 통해 각 변수의 유의미성을 평가.
시각화 matplotlib.pyplot
모델의 성능을 시각화하는 데 사용. 여러 k 값에 대해 훈련 정확도와 테스트 정확도를 비교하는 그래프를 생성.

PPT url:

https://docs.google.com/presentation/d/1CmexNFEkOCnVJsDuY-iU2xzWMFiBPxsg/edit?usp=drive_link&ouid=112062542611161741390&rtpof=true&sd=true
