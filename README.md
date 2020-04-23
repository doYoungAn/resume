# Preview
<img src="https://avatars0.githubusercontent.com/u/31813858?s=400&u=e5797f22f49c9270e4f6d1e71d9933d65cd7321a&v=4" width=200>

- 안도영
- email - jispoop@gmail.com
- github - https://github.com/doYoungAn

개발자라고 하면 공부의 최전선에 있어야 된다고 생각합니다.  
 개발자가 학습하는 이유는 비지니스 가치를 구현하는데 필요한 기술을 가려내는 눈이 필요하기 때문입니다. 


# 경력
- 토이스미스 (재직중)
    - 서버팀
    - Frontend Developer
    - 기간 : 2019.04 ~ now (1년)
- 위니플
    - 개발팀
    - Frontend Developer
    - 기간 : 2017.03 ~ 2019.03 (2년)

# 보유 기술

## Frontend
- 자주 사용하는 언어는 Typescript, Javascript 입니다.
- React 라이브러리, Vue.JS 프레임워크에 익숙합니다.
- Redux, Vuex, Ngrx 구조에 익숙합니다.
- css, scss를 자주 사용합니다.
- create-react-app과 같은 CLI 말고 커스텀으로 webpack을 설정해서 작업하는데 익숙합니다.

## DevOps
- Docker을 자주 사용합니다.
- docker-compose을 사용해서 여러개의 docker container들을 관리할 수 있습니다.
- gitlab CI/CD에 익숙합니다.

# 프로젝트

## 정화 사업 대시보드

각 각의 지역에서 진행되는 정화사업에서 사용하는 대시보드.  
정화사업에서 사용되는 관정에 대한 컨트롤, 관정 정보, 관정에서 수집하는 오염물질, 지하수등의 데이터에 대해 시각화를 진행한 프로젝트


### 인덕원 정화사업 대시보드
`토이스미스 | 웹 프론트엔드, 백엔드 개발 | 2019.03 ~ now`  

#### 주소
https://hyorim.toysmythiot.com

#### 개발
- Typescript를 사용하여 Frontend는 React 사용
- Typescript를 사용하여 Backend는 Node.js 기반 Express 프레임워크 사용
- three.js를 사용하여 heat map 개발
- DB를 통해 정보를 전달하여 디바이스 컨트롤 기능 개발
- 기상청 API를 사용하여 cron job로 해당 지역의 기온, 강수량 데이터 축적
- 실제 서비스는 docker swarm으로 서비스
- 배포는 gitlab CI/CD 를 사용하여 Frontend, Backend 빌드 후 docker 이미지 생성 후 swarm에 올리는 작업까지 자동화

#### 이슈 및 해결
- 프로젝트에 들어가는 이미지의 사이즈가 커 불 필요한 자원 낭비
    - imagemin-webpack-plugin
(webpack plugin)을 사용하여 이미지가 추가 될때마다 이미지 압축 실행

#### 보완해야 할 점
- 데이터 불러오는 속도가 느릴 경우가 있어 로딩 컴포넌트 제작

### 강릉 마그네슘 정화사업 대시보드
`토이스미스 | 웹 프론트엔드, 백엔드 개발 | 2019.07 ~ 2019.11`  

#### 주소
https://gangneung.toysmythiot.com

#### 개발
- Typescript를 사용하여 Frontend는 React 사용
- Typescript를 사용하여 Backend는 Node.js 기반 Express 프레임워크 사용
- D3.js를 사용하여 오염물질 등등의 데이터 시각화
    - Line Chart, bar Chart 구현
- GraphQL을 사용하여 비슷한 종류의 API 묶어서 개발
- DB를 통해 정보를 전달하여 디바이스 컨트롤 기능 개발
- 기상청 API를 사용하여 cron job로 해당 지역의 기온, 강수량 데이터 축적
- Jest를 사용하여 Backend 테스트 자동화
- 실제 서비스는 docker swarm으로 서비스
- 배포는 gitlab CI/CD 를 사용하여 Frontend, Backend 빌드 후 docker 이미지 생성 후 swarm에 올리는 작업까지 자동화

#### 이슈 및 해결
- MySQL row 양이 많아 쿼리가 느렸다.
    - 로딩 컴포넌트를 만들어 frontend에 적용
    - 테이블 인덱스 추가
- MYSQL row데이터를 일단위, 월단위로 묶어서 저장해야 했다.
    - cron job을 등록하여 일 00시, 월 1일 00시에 동작하도록 설정

### 녹사평 유류감지 정화사업 대시보드
`토이스미스 | 웹 프론트엔드, 백엔드 개발 | 2020.03 ~ now`  

#### 개발
- Typescript를 사용하여 Frontend는 React 사용
- Typescript를 사용하여 Backend는 Node.js 기반 Express 프레임워크 사용

## 수원 스마트 시티 대시보드
`토이스미스 | 웹 프론트엔드, 백엔드 개발 | 2019.08 ~ 2019.10`

수원시 행궁동 일대에 설치한 디바이스에서 수집한 데이터를 기반으로 시각화를 진행하였습니다. 방문자, 재방문자, 구역 이동 등의 데이터를 차트 기반으로 보여줍니다. (현재 서비스 되고 있지 않음)

#### 주소
https://suwon.toysmythiot.com

#### 개발
- Typescript를 사용하여 Frontend는 Vue.js 프레임워크 사용
- Typescript를 사용하여 Backend는 Node.js 기반 Express 프레임워크 사용
- D3.js를 사용하여 방문자 등등의 데이터 시각화
    - Line Chart, Bar Chart, Dount Chart 구현
- 실제 서비스는 docker swarm으로 서비스
- 배포는 gitlab CI/CD 를 사용하여 Frontend, Backend 빌드 후 docker 이미지 생성 후 swarm에 올리는 작업까지 자동화

#### 이슈 및 해결
- 한 페이지에서 보여주어야 하는 것을 초점으로 맞추어 페이지 이동 대신 모달 필요
    - Vue Plugin 형식으로 만들어 모달을 추가하는 기능 개발
- 차트에 대해 한눈에 보여야 된다는 기능 필요
    - 차트에 마우스 이벤트 추가 (hover)

#### 보완해야 할점
- d3.js 를 사용하면서 공통으로 사용되는 append('svg') 혹은 append('g').attr('transform', \`translate(${}, ${})\`) 코드등이 각 차트마다 중복으로 사용됨 해당 부분을 하나의 함수로 묶어야 함


## IotGateway CLI
`토이스미스 | CLI 개발 | 2019.10 ~ 2019.11`

사내에서 MongoDB를 도입하면서 만든 CLI 프로그램.  
MongoDB Validator 등록, User 리스트 보기, 각 커넥션 리스트 보기 기능, DB에 정의된 role 리스트 보기 기능이 있다.

#### 개발
- Typescript를 사용하여 Node.js 기반으로 개발
- [commander](https://www.npmjs.com/package/commander) 를 사용하여 개발
- gitlab v4 api를 사용하여 repo에 있는 Validator이 정의된 json 파일을 불러와 DB command를 사용하여 적용
- DB command를 사용하여 User 리스트, 커넥션 리스트, roles 을 가져와서 보여준다.
- CLI 사용할때 MongoDB user, password 인자로 넣어주게 개발

#### 보완해야 할 점
- gitlab이 private 이므로 api를 사용할때 필요한 토큰에 대한 관리를 cli 실행할 때 인자로 넣어주게 바꾸어야 한다. 


## 하트비트 대시보드
`토이스미스 | 웹 프론트엔드, 벡엔드 개발 | 2019.03 ~ now`

사내에서 내보낸 디바이스들에 대한 정보를 쉽게 볼 수 있는 요구가 있었습니다. 디바이스가 언제 살아 있었는지 어떤 정보를 보내는 지에 대한 정보를 보여주는 대시보드입니다.

#### 개발
- Typescript를 사용하여 Frontend는 React 프레임워크 사용
- Typescript를 사용하여 Backend를 Node.js 기반 Express 프레임워크 사용
- D3.js를 사용하여 디바이스 생존 시간 시각화 - Timeline 구현
- 실제 서비스는 docker swarm으로 서비스
- 배포는 gitlab CI/CD 를 사용하여 Frontend, Backend 빌드 후 docker 이미지 생성 후 swarm에 올리는 작업까지 자동화

#### 이슈 및 해결
- 새로고침시 다시 검색해야 되는 번거로움이 있다.
    - url query로 키값, 날짜값등을 가지고 있어서 url이 바뀔때 api 호출 하는 방식으로 변경
- Mysql row 데이터가 많아서 쿼리의 속도가 느리다.
    - 대시보드 상에서 로딩 추가
    - 테이블 인덱싱 추가

#### 보완해야 할점
- 엘리먼트 사이즈가 변할때 마다 차트도 같이 reponsive 하게 바꾸어 줘야 한다.


## 티켓바이
`위니플 | 웹 프론트엔드, 백엔드 개발 | 2019.01 ~ 2019.03`

뮤지컬 티켓, 영화 티켓 등 중고 티켓을 거래하는 서비스 (현재 서비스 되고 있지 않음)

#### 개발
- Typescript를 사용하여 Frontend는 Vue.js 프레임워크 사용
- Typescript를 사용하여 Backend는 Node.js 기반 Express 프레임워크 사용
- 결제 관련 내용은 세틀뱅크 PG 사를 이용하여 연동
- frontend 배포는 gulp를 사용하여 AWS S3에 업로드 자동화
- Backend 배포는 EC2에서 pm2로 배포

## 위니플 서비스
`위니플 | 웹 프론트엔드 개발 | 2017.11 ~ 2018.09`

사용자들이 앱 이름, 앱 아이콘, 메뉴등을 설정하면 앱을 자유롭게 빌드하여 사용할 수 있게 해주는 서비스 (현재 서비스 되고 있지 않음)

#### 개발
- Typescript를 사용하여 Frontend는 Angular2+ 프레임워크 사용
- 유저 상태 관리를 위해 Ngrx 도입
