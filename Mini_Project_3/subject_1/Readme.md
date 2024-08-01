# **스마트폰 센서 데이터 기반 모션 분류**

## 프로젝트 수행과정

- 데이터 준비
- 데이터 전처리
- 모델링
- 결과 분석

## 데이터 분석 및 전처리

- 목표 변수 확인

    <img src="./img/image1.png" alt="eda1" width="300"/>

    <img src="./img/image2.png" alt="eda2" width="300"/>
    
  - T-SNE를 이용하여 목표변수 군집화 수행
    - LAYING의 경우, 센서가 지표면과 평평한 상태에서 움직이지 않는 경향으로 분류
    - STANDING과 SITTING의 경우, 센서가 움직이지 않는 상태에서 두 클래스는 단순히 높낮이의 차이만 보이기에 군집이 비슷한 위치에 분류
    - WALKING, WALKING DOWNSTAIRS, WALKING UPSTAIR의 경우, 동적인 활동으로 지표면으로부터의 높낮이에 따라 차이가 나기 때문에 크게 비교할 수 없어서 군집이 비슷한 위치에 분류

- 데이터 전처리 흐름

<img src="./img/image3.png" alt="eda3" width="300"/>

## 모델링

<img src="./img/image4.png" alt="model1" width="300"/>

## 결과

<img src="./img/image5.png" alt="result1" width="300"/>

- 정확도 98.2%
- SITTING과 STANDING의 분류 성능 향상에 개선점이 보임