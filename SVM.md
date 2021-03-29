#### 서포트 백터 머신

  - Maximizing margin over the training set (트레인 데이터의 마진을 최대화)
      = minimizing generalization error (에러 최소화)
      
  - Margin : 각 클래스에서 가장 가까운 관측치 사이의 거리
  - W (기울기)로 표현 가능 : W의 2/L2 Norm
   
  ![image](https://user-images.githubusercontent.com/79842387/112860858-2fe43300-90ef-11eb-9f40-7f22c9c2d45a.png)

  ![image](https://user-images.githubusercontent.com/79842387/112861107-75a0fb80-90ef-11eb-8781-3f40b12f3114.png)

  ![image](https://user-images.githubusercontent.com/79842387/112861966-4212a100-90f0-11eb-8edb-7c291531c332.png)

  ![image](https://user-images.githubusercontent.com/79842387/112862077-5b1b5200-90f0-11eb-8cf0-cb5487513b47.png)

  ![image](https://user-images.githubusercontent.com/79842387/112862152-6f5f4f00-90f0-11eb-949c-812c928a2d88.png)

  
  - 비선형 : Soft Margin SVM (Linearly Nonseparable Case)
      cf. Hard Margin SVM
  
  ![image](https://user-images.githubusercontent.com/79842387/112862493-c7965100-90f0-11eb-8028-6a81a9fd8e2c.png)
  
  
  - 플러스 Plane, 마이너스 Plan의 거리인 마진이 최대가 되는 함수를 찾는 것
  - 결정 변수 3개 (Slack variable 도입)
  
  ![image](https://user-images.githubusercontent.com/79842387/112862884-32e02300-90f1-11eb-8a39-81072062bfac.png)

  ![image](https://user-images.githubusercontent.com/79842387/112862845-28be2480-90f1-11eb-8b1c-2f7646b95a39.png)
  
  
  - 비선형 SVM
  ![image](https://user-images.githubusercontent.com/79842387/112863686-11cc0200-90f2-11eb-83f0-9596250d652e.png)

  ![image](https://user-images.githubusercontent.com/79842387/112864557-de3da780-90f2-11eb-85e3-212768fb7219.png)

  ![image](https://user-images.githubusercontent.com/79842387/112864726-0f1ddc80-90f3-11eb-85d0-ac251e679383.png)
  
  ![image](https://user-images.githubusercontent.com/79842387/112865055-5f953a00-90f3-11eb-8b53-ac7cc54d5b8e.png)


