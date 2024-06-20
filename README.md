# 이츠유얼턴
비보호 좌회전 안전 보조 시스템, It's your turn!

## Outline
프로젝트 주제: AI를 활용한 서비스 제작

프로젝트 수행자: 인텔 엣지 AI SW 개발자 아카데미 4기 / 팀 이츠유얼턴 (김승민, 박민혁, 유지승, 조수환)

프로젝트 수행기간: 24/06/20 ~ 24/07/02

* 라즈베리파이와 태블릿을 사용하여 비보호 좌회전 시 교통 안전을 보조하는 디지털 계기판 디스플레이 시스템의 프로토타입을 구현한다.
* 이 시스템은 교통 표지판, 신호등을 인식하고, 반대 차선의 차량을 감지하여 안전한 좌회전을 돕는다.

## 팀 구성

* Members
  | Name | Role |
  |----|----|
  | 김승민 | Project lead, Hardware Setup  |
  | 박민혁 | UI design, AI modeling    |
  | 유지승 | AI modeling, Project Manager   |
  | 조수환 | AI modeling, System integration |
  
* Project Github : https://github.com/suhwanjo/Intel-Eged-AI-Project.git
* 발표자료 : https://github.com/wodud6423/Intel-Edge-AI-/tree/main

## Motivation
### 문제 정의
#### 비보호 좌회전 시 발생한 사고
* 통계
    * 교통사고 통계에 따르면 비보호 구역 내 도로에서 발생하는 교통사고 발생률이 일반 도로보다 30% 높은 수준입니다.
* 문제 인식
    * 비보호 좌회전은 종종 운전자에게 혼란을 주고 교통 사고의 주요 원인 중 하나로 작용합니다. 특히 교차로에서의 판단 착오로 인해 사고가 발생할 가능성이 큽니다.

#### 프로젝트 필요성
* 운전자 교육 및 인식 개선
    * 많은 운전자들이 교통법규를 제대로 알지 못하거나 오해하여 발생하는 사고가 많습니다. 이 프로젝트는 실시간 도로 정보와 신호를 제공함으로써 이러한 문제를 해결하고자 합니다.
* 안전한 운전 환경 조성
    * 운전자들에게 교차로에서의 비보호 좌회전 시 안전한 판단을 도울 수 있는 시스템을 제공함으로써, 교통 상황을 명확하게 인지하고 안전한 운전 환경을 조성할 수 있습니다.
* 교통 사고 예방
    * 실시간 도로 정보와 신호를 제공하여 운전자의 판단을 돕고, 이를 통해 교통 사고를 예방할 수 있습니다. 이는 교통 체계의 효율성 향상에도 기여할 것입니다.

#### 기대 효과
* 안전한 교차로 주행
    * 본 시스템이 구현되면, 교차로에서의 비보호 좌회전 시 안전한 판단을 돕는 기능을 제공함으로써 교통 사고를 크게 줄일 수 있을 것입니다.
* 교통사고 감소
    * 교통사고 통계에 따르면 비보호 구역 내 도로에서 발생하는 교통사고 발생률이 일반 도로보다 30% 높은 수준입니다. 이 시스템을 통해 비보호 구역에서의 사고를 효과적으로 감소시킬 수 있습니다.
* 교통 흐름 개선
    * 실시간으로 도로 상태와 신호 정보를 제공함으로써 교통 흐름을 더 원활하게 하고, 운전자의 예측 가능성을 높여 교차로에서의 교통 혼잡을 줄일 수 있습니다.
* 운전자 신뢰도 향상
    * 운전자들이 교통 상황을 명확히 인지하고 안전하게 주행할 수 있도록 도와줌으로써, 전체 교통 시스템에 대한 신뢰도를 향상시킬 수 있습니다.

## Project Schedule
![plan](https://github.com/suhwanjo/Intel-Eged-AI-Project/assets/112834460/6662b3db-6ef7-4363-9631-36c73bb08e2f)

## High Level Design

### 기능 명세서

#### 각 기능의 세부 요구사항

1. **좌회전 인식**
    - 방향 지시등 대체 스위치를 통해 좌회전 시작을 인지.
    - 방향 지시등 신호가 입력되면 시스템 활성화.

2. **교통 표지판 및 신호 인식**
    - 비보호 좌회전 표지판 인식.
    - 신호등 인식 및 신호 분석.

3. **반대 차선 차량 인식**
    - 반대 차선 차량 감지.
    - 차량의 거리 측정 및 거리 추정.

4. **안전 판단**
    - 교통 표지판 정보 및 반대 차선 차량 정보를 종합하여 안전 여부 판단.
    - 판단 결과를 실시간으로 HUD에 표시.

5. **HUD 디스플레이**
    - 태블릿을 통해 운전자가 쉽게 볼 수 있는 HUD 화면 구현.
    - 안전 여부 및 관련 정보를 시각적으로 표시.

### 기능별 우선순위

1. 좌회전 인식
2. 교통 표지판 및 신호 인식
3. 반대 차선 차량 인식
4. 안전 판단
5. HUD 디스플레이

### 시스템 구상도(초안)
<img width="3312" alt="시스템구상도" src="https://github.com/suhwanjo/Intel-Eged-AI-Project/assets/112834460/8e81bc01-c197-498b-bd54-dbe60f611aec">


