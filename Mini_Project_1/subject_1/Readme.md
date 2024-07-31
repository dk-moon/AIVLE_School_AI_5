# 서울시 생활정보 기반 대중교통 수요 분석 프로젝트

## 가설 수립

- 우리 조에서 설정한 가설

1. 인구수와 정류장 수에는 양의 상관관계가 있다.
2. 승하차 총 승객수와 정류장 수에는 양의 상관관계가 있다.
3. 특정 업종이 밀집된 지역은 교통 수요(총 이동 인구)가 높을 것이다.

## 단변량 분석 (가설 1, 가설 2)

- 인구수와 정류장 수

<img src="./img/image1.png" alt="pop_bus1" width="300"/>

<img src="./img/image2.png" alt="pop_bus2" width="300"/>

- 승하차 승객수와 정류장 수

<img src="./img/image3.png" alt="down_up1" width="300"/>

## 가설 검증 과정 (가설 1, 가설 2)

- 인구 수와 정류장 수

<img src="./img/image4.png" alt="pop_bus3" width="300"/>

    - 상관계수 0.608로 인구와 정류장 수는 중간정도(<0.7)의 상관관계가 있다.

- 승하차 승객수와 정류장 수

<img src="./img/image5.png" alt="down_up2" width="300"/>

    - 상관계수 0.578로 인구와 정류장수는 중간정도(<0.7)의 상관관계가 있다.

## 정류장 수 결론 (가설 1, 가설 2)

- 가설 1과 가설 2

    - 구별 인구와 정류장 수의 상관계수가 구별 승하차 인구와 정류장 수의 상관계수보다 미미하게 높다.

    - 따라서, 현재 승하차 인원보다는 구별 인구 기준으로 정류장이 설치되어있을 가능성을 제시하며, 인구보다는 실제 승하차 인원 기준으로 정류장을 세워야 한다.

    - 가설 3을 통해 교통 실수요를 측정하고 실수요 대비 정류장이 부족한 구를 우선 추천한다.

    - $\frac{정류장 수}{승객 총수} - \frac{정류장 수}{인구수}$가 가장 작은 **종로구**, **마포구**, **성동구**를 제안한다.

## 다변량 분석 (가설 3)

- 각 자치구 별 업종 수 분포

<img src="./img/image6.png" alt="gu_store1" width="300"/>

- 자치구 총 이동인구 별 요식업 종사자 수

<img src="./img/image7.png" alt="move_job1" width="300"/>

<img src="./img/image10.png" alt="move_job2" width="300"/>

    - '한식 일반 음식점업', '기타 주점업', '커피전문점', '한식 육류요리 전문점' 종사자를 묶어서 '요식업 종사자'로 묶음

<img src="./img/image11.png" alt="heatmap" width="300"/>

## 단변량 분석 (가설 3)

- 업종 수

<img src="./img/image8.png" alt="job1" width="300"/>

- 총 이동인구

<img src="./img/image9.png" alt="move1" width="300"/>

## 가설 검증 과정 (가설 3)

- 요식업 종사자 수와 총 이동인구 사이에는 매우 높은 상관관계를 보인다.

- 데이터의 최대값으로 분석하면 서울시의 업종별 사업장 수는 '운송업', '요식업', '서비스업'순으로 되어있다. 그리고 서울시의 업종별 종사자의 수는 '요식업', '서비스업', '운송업'순으로 되어있다.

- 이를 통해, 사업장의 수는 운송업이 많지만, 운송없의 경우 **개인 사업자의 성향**이 강하고 요식업과 서비스업의 경우 **한 사업장에 많은 사람이 종사**하기 때문이라고 볼 수 있다.

## 업종 수 결론 (가설 3)

- 특정 업종이 밀집된 지역은 해당 업종 종사자가 많을 것이다.

- 종사자 수가 많다면 인구의 이동이 활발하다.

- 요식업 종사자 수와 이동인원수가 서로 상관관계가 있다.

- 이동이 활발하면, 교통의 수요가 높을 것이다.

- 이동이 활발하지 않다면 해당 지역구는 접근성이 떨어지기 때문에 교통 효율성이 떨어질 것이다.

- 교통의 효율성이 떨어진 지역구에 대해서 대중교통의 효율성을 개선할 필요가 있다.

- 따라서, 요식업 종사자 수 대비 총 이동 인구수가 높은 **노원구**와 요식업 종사자 수 대비 총 인구수가 노원구 다음으로 높은 **강동구**에 버스 시설의 추가가 가장 필요하다.