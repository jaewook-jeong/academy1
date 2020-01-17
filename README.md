# 경복궁 안내 프로그램(Java Application)
## 1. 개관
### 1.1. 개발 의도
인도여행 때 현지친구의 추천으로 아름다운 경관을 보기위해 오지로 간적이 있다. [N포털사이트](https://search.naver.com/search.naver?sm=tab_hty.top&where=nexearch&query=%EA%B0%A0%EB%94%94%EC%BD%94%ED%83%80&oquery=%EC%BA%94%EB%94%94%EC%BD%94%ED%83%80&tqi=UAakTdp0Jy0ss4bBoowssssstSR-090855)에 검색해도 아무것도 나오지 않던 그곳으로 현지인의 정보만으로 그곳을 찾아갔다. 도착해서 만난 그곳은 힌두어 안내문과 터지지 않는 데이터만 존재했다. 그곳에서 만난 아름다움을 두고 대도시에서 정보를 얻을 수 있었다. 이처럼 인터넷을 접속하지 못하는 상황도 있지만, 정보에 대한 확실성과 경험 공유에 의의를 둔 프로그램을 개발했다. 또한 해당 장소(건축물 등)의 다양한 계절의 사진과 영어 음성해설을 제공함으로써 적확한 정보를 제공하기 위해 노력했다.
### 1.2. 개발 정보
* 개발 인원 : 1인
* 개발 기간 : 2019.07.15 ~ 07.19 (총5일간)
#### 1.2.1. 개발 기간
| 날짜 | 진행사항 | 비고 |
|---|:---:|---:|
| 2019.07.15 | 콘셉트 결정 및 DB구성 | |
| 2019.07.16 | 기초 틀 완성 |  |
| 2019.07.17 | DB입력 및 음성해설 영어번역 |  |
| 2019.07.18 | 사진 및 영어해설 DB 입력 |  |
| 2019.07.19 | 테스트 및 완성 |  |
#### 1.2.2. 개발 환경 및 툴
* OS : Window 7
* Language : Java
* DBMS : Oracle
* DB tool : QueryBox
* Programming tool : Eclipse
---------------
## 2. 본론
### 2.1. 프로젝트 중점
#### 2.1.1. 발전 가능성
Java를 이제 막 접한 나에게 지금의 프로젝트가 나중에도 이용가능토록 개발하고 싶었다. 그래서 단순히 Java Application이 아니라 나중에 Android로 발전하고 Web으로 개발하여 규모를 키우고 싶었다. 그러나 첫 개발물에 내가 할 수 있는 것은 많지 않았다. 경복궁을 실제로 갈 때 GPS를 통해 현재 보이는 유적을 설명하는 `도슨트` 역할의 개발을 하고 싶었다. 그러나 컴퓨터로 위치정보를 바꾸며 운용할 수 없었다. 그래서 생각한 것은 나중에 Android 공부를 통한 확장이었고, 첫 개발물은 화살표 버튼으로 icon의 움직임을 통한 이동경로의 구현이었다. 이를통해 경복궁지도에서 icon의 움직임을 구현하여 경로저장 및 icon을 이동해가며 icon이 해당 유적 근처에 있을 시 해당하는 사진과 영어해설을 실행토록 구현했다. 또한 지도에서 해당 유적 클릭시 도슨트 기능을 작동토록 하였다. 이처럼 나중에 개발을 이어나갈 수 있도록 구성하였다. 더불어 경로의 저장과 공유를 통해 타인과 정보 교류를 할 수 있도록 기초적인 게시판을 구성하였다. 이를통해 Web과 Android App의 확장 가능성을 구상했다.
#### 2.1.2. Thread의 사용
처음 배운 Java는 내게는 너무 정적인 느낌이었다. 그래서 동적인 Java Application을 개발코자 목표했다. 그래서 생각한 것이 Thread였다. Thread는 처음에 받아들이기 쉽지 않은 개념이었다. 그러나 처음배운 sleep메소드를 통해 동적인 아이디어를 구상했고 실현했다. 화살표 버튼을 클릭하면 icon의 위치를 thread를 통해 반복 이동하도록 하여 동적인 모습을 출력했다. 또한 이외에 게시판에서 좌측 구역을 광고 구역으로 설정하여 서울 5대궁궐 이미지를 Thread로 반복하며 클릭시 해당 영어 사이트로 이동하도록 구성하였다.  

----------------------
## 3. 결론
첫 개발에 의의를 둔다. 부족한 Thread의 이해와 코드의 재사용성, 무분별한 클래스의 작성에 대한 고찰이 필요하다. 
[발표PPT](https://docs.google.com/presentation/d/1OPhCKI5rNIF9T_mx4lBNPwL1cUt9242DkIh8DasPSsc/edit?usp=sharing)
