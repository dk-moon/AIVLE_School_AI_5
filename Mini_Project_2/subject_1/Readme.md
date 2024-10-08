# **공공데이터를 활용한 미세먼지 농도 예측**

## 수행 목표

- 미세먼지 농도를 예측하는 머신러닝 모델 개발

- 풀어야 하는 문제:
  - 서울 지역의 미세먼지 데이터와 날씨 데이터를 활용하여, 미세먼지 예측에 관련있는 데이터 항목으로 구성된 데이터를 전처리하여 미세먼지 농도를 예측하는 머신러닝 모델 구현

## 데이터 소개

### 기본 데이터

- 학습 데이터
  - air_2022.csv : 2022년 미세먼지 데이터
  - weather_2022.csv : 2022년 날씨 데이터

- 테스트 데이터
  - air_2023.csv : 2023년 미세먼지 데이터
  - weather_2023.csv : 2023년 날씨 데이터

### 데이터셋의 변수 소개(weather_2022,2023)

- 증기압: 증기가 고체 또는 액체와 동적 평형 상태에 있을 때 증기의 압력 (증기가 되려는 힘)

- 이슬점 온도: 불포화 상태의 공기가 냉각될 때, 포화 상태에 도달하여 수증기의 응결이 시작되는 온도

- 일조: 일정한 물체나 땅의 겉면에 태양 광선이 비치는 시간 (1시간 중 비율)

- 일사(량): 태양으로부터 오는 태양 복사 에너지가 지표에 닿는 양 (면적당 에너지 량)

- 전운량: 하늘을 육안으로 관측하여 전부 구름일 때 10, 구름이 덮고 있는 하늘의 비율에 따라 0~10

- 중하층운량: 중층과 하층에 있는 구름의 분포량(중하층 구름이 날씨에 영향 주므로 따로 표기)

- 운형(운형약어): 구름의 종류. 약어 코드로 기재됨

- 최저운고: 가장 낮은 구름의 높이

- 현상번호(국내식): 비, 소낙비, 싸락눈, 눈보라 등의 기상현상을 나타낸 코드번호

- 지면온도: 지면 0cm 온도

- 지중온도: 땅 속 온도변수

## 데이터 분석

<img src="./img/image1.png" alt="eda1" width="300"/>

    - 겨울철 기온이 내려갈수록 석탄 등 화석연료의 사용이 많아져 미세먼지를 증가시키고 대기질에 영향을 미치는 것으로 분석된다.
