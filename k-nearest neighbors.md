### 분류 및 예측을 위한 모델

  1. Model-based Learning
    - 선형/비선형 모델
    - Neural network
    - 의사결정나무
    - Support vector machine
    -> 데이트러부터 모델을 생성하여 분류/예측 진행

  2. Instance-based Learning
    - K-nearest neighbor
    - Locally weighted regression
    -> 별도의 모델 생성 없이 인접 데이터를 분류/예측에 사용
    

#### K-Nearest Neighbors (KNN) 알고리즘

  - Nearest Neighbors : 새로운 데이터의 가장 가까운 이웃을 정의

  - KNN 알고리즘의 구분 및 특징
  ![image](https://user-images.githubusercontent.com/79842387/112480558-8254e500-8db9-11eb-98ee-d1201667ff21.png)

  - 분류/예측 모두 사용 가능
  1) KNN 분류 알고리즘 : 인접 데이터 K개의 다수결로 분류
  ![image](https://user-images.githubusercontent.com/79842387/112481093-027b4a80-8dba-11eb-9697-330b4cfd8ea9.png)
  ![image](https://user-images.githubusercontent.com/79842387/112480837-c1833600-8db9-11eb-85e3-cf3ffb5e4b6d.png)

  2) KNN 예측 알고리즘 : 평균 값으로 반환
  ![image](https://user-images.githubusercontent.com/79842387/112484741-8e42a600-8dbd-11eb-8501-0b0d6f1ce57a.png)

 - 하이퍼 파라미터 (파라미터 존재 X)
  1) K : 인접한 학습 데이터 탐색 수 (1=< k <= 전체데이터수)
    - k가 매우 작을 경우 Overfitting(지역적 특성을 지나치게 반영), 
    - k가 매우 클 경우 Underfitting(다른 범주 개체 너무 많이 포함하여 오분류 위험)
    - 일정 범위 내로 k를 조정하여 가장 좋은 예측 결과를 보이는 k를 선정
      (training 에러와 testing 에러 적정 지점)
  2) Distance Measures : 데이터 간 거리 측정 방법
    - 거리측도(1-유사도)
    - 데이터 내 변수들이 각기 다른 데이터 범위, 분산 등을 가질 수 있으므로 데이터 정규화(혹은 표준화)를 통해 맞추는 것이 중요
  
    1)유클리디안 거리 (Euclidean Distance)
      : 가장 흔히 사용, 대응되는 x,y값 간 차이 제곱합의 제곱근으로써 두 관측치 사이의 직선거리를 의미
      
    2) 맨하탄 거리 (Mangattan Distance)
      : x에서 y로 이동 시 각 좌표축 방향으로만 이동할 경우에 계산되는 거리 (격자 형태)
      ![image](https://user-images.githubusercontent.com/79842387/112486276-14132100-8dbf-11eb-9706-528a899c398a.png)

    3) 마할라노비스 거리 (Mahalanobis Distance)
      : 변수 내 분산, 변수 간 공분산을 모두 반영하여 x,y간 거리를 계산하는 방식
        데이터의 convariance matrix가 identity matrix(단위 행렬)인 경우는 Euclidean distance와 동일
        
    4) Correlation Distance 
      : corr 범위 -1 ~ +1, correlation distance 범위 0~2
        데이터 간 Pearson correlation을 거리 측도로 사용하는 방식으로, 데이터 패턴의 유사도를 반영할 수 있음
        ![image](https://user-images.githubusercontent.com/79842387/112486926-aa474700-8dbf-11eb-990a-fcfd16040a55.png)

    5) Spearman Rank Correlation Distance
      : 범위는 -1 ~ +1

  - KNN 장점, 한계점
   ![image](https://user-images.githubusercontent.com/79842387/112487406-05793980-8dc0-11eb-852a-fe9e38f629c9.png)

  - Weighted KNN
    : 거리에 대한 가중치 고려   
      (새 데이터와 기존 학습 관측치 간의 거리를 가충치로 하여 예측 결과 도출)
      
      
  ![image](https://user-images.githubusercontent.com/79842387/112487986-85070880-8dc0-11eb-81f3-cab59753b7fe.png)

  
