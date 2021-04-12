#### boosting

  - 순차적으로 구축! (모델 구축에 순서를 고려)
  - 여러개의 learning 모델을 최종적으로 합침 (앙상블)
    - learning 모델은 매우 단순한 모델 : Model that slightly better than chance
  - 각 단계에서 새로운 base learner를 학습하여 이전 단계의 base learner의 단점을 보완
  - 각 단계를 거치면서 모델이 점차 강해짐 : boosting


  1) Adaptive boosting (Adaboost)
  2) Gradient boosting machnies (GBM)
  3) XGboost
  4) Light gradient boost machines(LightGBM)
  5) Catboost

  1) Adaboost
    - 오분류한 관측치에 보다 집중!
    ![image](https://user-images.githubusercontent.com/79842387/114405691-e3feb700-9be1-11eb-9d61-0d8ea0fc78c5.png)
    ![image](https://user-images.githubusercontent.com/79842387/114407954-e95d0100-9be3-11eb-8881-9483518cd4ba.png)
  
    1. 모든 관측치에 가중치 (초기 가중치 : 1/n) = impose equal weight initially
    ![image](https://user-images.githubusercontent.com/79842387/114409040-00502300-9be5-11eb-8200-3311576f23cd.png)
    2. loss function : 0.3
       a1(알파1) : 1번째 classifier의 가중치
       -> 오분류에 가중치를 줌
   ![image](https://user-images.githubusercontent.com/79842387/114408280-38a33180-9be4-11eb-9a55-f09c062d8cfd.png)
    3. 새로운 classifier -> 오분류에 가중치
   ![image](https://user-images.githubusercontent.com/79842387/114408651-98014180-9be4-11eb-9417-bad16b98e378.png)
    4. -> 반복
    5. 결론
    ![image](https://user-images.githubusercontent.com/79842387/114408986-f0d0da00-9be4-11eb-8b2f-79ad30790c08.png)


#### bagging vs boosting
  ![image](https://user-images.githubusercontent.com/79842387/114409381-5e7d0600-9be5-11eb-931e-1035c5b7b9e5.png)

#### GBM (Gradient Boosting Machines)

  - Residual : y - y_hat
  ![image](https://user-images.githubusercontent.com/79842387/114409625-98e6a300-9be5-11eb-8b45-a471ac72b176.png)
  
  - why gradient?
  ![image](https://user-images.githubusercontent.com/79842387/114410028-fe3a9400-9be5-11eb-9707-4ff0d6f1e10e.png)

  - ![image](https://user-images.githubusercontent.com/79842387/114410860-a81a2080-9be6-11eb-802c-adb7d785d98c.png)
  - ![image](https://user-images.githubusercontent.com/79842387/114410984-c2ec9500-9be6-11eb-97c6-7dee43fd0c12.png)

  - ![image](https://user-images.githubusercontent.com/79842387/114412671-465ab600-9be8-11eb-9ae1-ee6e1abec790.png)
