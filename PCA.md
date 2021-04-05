### 주성분 분석

  - 차원 축소 방법
      1) 변수 선택 (selection) : 분석 목적에 부합하는 소수의 예측 변수만을 선택
     
        - 장점 : 선택한 변수 해석 용이
        - 단점 : 변수간 상관관계 고려 어려움 
      2) 변수 추출 (extraction) : 예측 변수의 변환을 통해 새로운 변수 추출
      
        - 장점 : 변수간 상관관계 고려, 일반적으로 변수의 개수를 많이 줄일 수 있음
        - 단점 : 추출된 변수의 해석이 어려움


      ![image](https://user-images.githubusercontent.com/79842387/113567323-63701180-9649-11eb-92ff-70b94051856c.png)


    - 비지도 변수 추출법
    - Principal Components Analysis
      : 고차원 데이터를 효과적으로 분석하기 위한 대표적인 분석 기법
        차원 축소, 시각화, 군집화, 압축
        
    - ![image](https://user-images.githubusercontent.com/79842387/113567475-a7631680-9649-11eb-9fc9-31bfec72153a.png)
    - ![image](https://user-images.githubusercontent.com/79842387/113567695-0a54ad80-964a-11eb-8733-2cc48cbb8b79.png)

    - 분산을 최대화하는 축을 찾는다.
    - ![image](https://user-images.githubusercontent.com/79842387/113567812-4556e100-964a-11eb-89b1-20527632f221.png)

    - PCA 수리적 배경
      - Mean vector
      - Covariance Matrix (공분산)
      - Correlation Matrix

        ![image](https://user-images.githubusercontent.com/79842387/113568020-b0081c80-964a-11eb-9f5e-770bd86d2165.png)
        ![image](https://user-images.githubusercontent.com/79842387/113568075-c9a96400-964a-11eb-8478-4558bbeb27d6.png)
        ![image](https://user-images.githubusercontent.com/79842387/113568191-07a68800-964b-11eb-8f0e-e6ffec40f2b8.png)
        
        
    - PCA 알고리즘 _ 주성분 추출
    - 시그마 : PxP 공분산 행렬
    -![image](https://user-images.githubusercontent.com/79842387/113568398-71269680-964b-11eb-8f8e-9909c6dab6b6.png)

  
    - 예제
    - ![image](https://user-images.githubusercontent.com/79842387/113568769-2b1e0280-964c-11eb-9e38-6233c7cac0fb.png)
    - ![image](https://user-images.githubusercontent.com/79842387/113568807-3d983c00-964c-11eb-99c0-47b41c872316.png)

  - ![image](https://user-images.githubusercontent.com/79842387/113568854-57d21a00-964c-11eb-9047-dd372178839a.png)
  - ![image](https://user-images.githubusercontent.com/79842387/113568936-82bc6e00-964c-11eb-8079-35a159e6be3a.png)
  - ![image](https://user-images.githubusercontent.com/79842387/113569006-aaabd180-964c-11eb-9aa6-ae2323fb0b81.png)

  - 몇 개의 주성분을 사용해야 할까?
  - 주성분의 분산 = eigenvalue
 
  - ![image](https://user-images.githubusercontent.com/79842387/113569110-dfb82400-964c-11eb-9af1-d912698e376f.png)
  
  - 가장 큰 z를 사용했을 때 92% 설명력
  - ![image](https://user-images.githubusercontent.com/79842387/113569244-1c841b00-964d-11eb-9160-3bf0cc811eb3.png)

  - ![image](https://user-images.githubusercontent.com/79842387/113569312-3aea1680-964d-11eb-98b2-0679c87d0df9.png)

  - PCA Loading : 실제 변수가 주성분 결정에 얼마나 많은 영향을 미쳤는지
  - 오른 쪽 위에 해당할 수록, 알파 값이 크고, 크게 영향을 미쳤다는 의미
 ![image](https://user-images.githubusercontent.com/79842387/113569547-aa600600-964d-11eb-9ea0-cf4ab0f8b1cf.png)

  - PCA 알고리즘 요약
  - correlation matrix 계산하는 것이 좋음
  - ![image](https://user-images.githubusercontent.com/79842387/113569653-d67b8700-964d-11eb-9d3a-da69f533449d.png)


  - 한계
  - ![image](https://user-images.githubusercontent.com/79842387/113569787-04f96200-964e-11eb-9480-d4982551e2a6.png)
  - ![image](https://user-images.githubusercontent.com/79842387/113569842-222e3080-964e-11eb-9c8b-4755b635aa5d.png)


  - 실제 예제
  - ![image](https://user-images.githubusercontent.com/79842387/113569911-42f68600-964e-11eb-944a-00dbb886b3b4.png)
  - ![image](https://user-images.githubusercontent.com/79842387/113569980-60c3eb00-964e-11eb-8273-629b4fe8e72d.png)
