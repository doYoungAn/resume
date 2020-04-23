# Preview
<img src="https://avatars0.githubusercontent.com/u/31813858?s=400&u=e5797f22f49c9270e4f6d1e71d9933d65cd7321a&v=4" width=200>

- 안도영
- email - jispoop@gmail.com
- github - https://github.com/doYoungAn


# 경력
- 토이스미스
    - 서버팀
    - Frontend Developer
    - 2019.04 ~ (1년)
- 위니플
    - 개발팀
    - Frontend Developer
    - 기간 2017.03 ~ 2019.03 (2년)

# 프로젝트

## 정화 사업 대시보드

### 인덕원 정화사업 대시보드
`토이스미스 | 웹 프론트엔드, 백엔드 개발 | 2019.03 ~ now`

#### 주소
https://hyorim.toysmythiot.com

#### 개발
- Typescript를 사용하여 Frontend는 React 사용
- Typescript를 사용하여 Backend는 Node.js 기반 Express 프레임워크 사용
- DB를 통해 정보를 전달하여 디바이스 컨트롤 기능 개발
- 실제 서비스는 docker swarm으로 서비스
- 배포는 gitlab CI/CD 를 사용하여 Frontend, Backend 빌드 후 docker 이미지 생성 -> swarm에 올리는 작업까지 자동화

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
- Jest를 사용하여 Backend 테스트 자동화
- 실제 서비스는 docker swarm으로 서비스
- 배포는 gitlab CI/CD 를 사용하여 Frontend, Backend 빌드 후 docker 이미지 생성 -> swarm에 올리는 작업까지 자동화

### 녹사평 유류감지 정화사업 대시보드
`토이스미스 | 웹 프론트엔드, 백엔드 개발 | 2020.03 ~ now`

#### 개발
- Typescript를 사용하여 Frontend는 React 사용
- Typescript를 사용하여 Backend는 Node.js 기반 Express 프레임워크 사용

## 수원 스마트 시티 대시보드
---
`토이스미스 | 웹 프론트엔드, 백엔드 개발 | 2019.08 ~ 2019.10`

수원시 행궁동 일대에 설치한 디바이스에서 수집한 데이터를 기반으로 시각화를 진행하였습니다. 방문자, 재방문자, 구역 이동 등의 데이터를 차트 기반으로 보여줍니다. 

#### 주소
https://suwon.toysmythiot.com

#### 개발
- Typescript를 사용하여 Frontend는 Vue.js 프레임워크 사용
- Typescript를 사용하여 Backend는 Node.js 기반 Express 프레임워크 사용
- D3.js를 사용하여 방문자 등등의 데이터 시각화
    - Line Chart, Bar Chart, Dount Chart 구현
- 실제 서비스는 docker swarm으로 서비스
- 배포는 gitlab CI/CD 를 사용하여 Frontend, Backend 빌드 후 docker 이미지 생성 -> swarm에 올리는 작업까지 자동화

#### 이슈 및 해결
- 한 페이지에서 보여주어야 하는 것을 초점으로 맞추어 페이지 이동 대신 모달 필요
    - Vue Plugin 형식으로 만들어 모달을 추가하는 기능 개발
- 차트에 대해 한눈에 보여야 된다는 기능 필요
    - 차트에 마우스 이벤트 추가 (hover)

## 하트비트 대시보드
---
`토이스미스 | 웹 프론트엔드, 벡엔드 개발 | 2019.03 ~ `

사내에서 내보낸 디바이스들에 대한 정보를 쉽게 볼 수 있는 요구가 있었습니다. 디바이스가 언제 살아 있었는지 어떤 정보를 보내는 지에 대한 정보를 보여주는 대시보드입니다.

#### 개발
- Typescript를 사용하여 Frontend는 React 프레임워크 사용
- Typescript를 사용하여 Backend를 Node.js 기반 Express 프레임워크 사용
- D3.js를 사용하여 디바이스 생존 시간 시각화 - Timeline 구현
- 실제 서비스는 docker swarm으로 서비스
- 배포는 gitlab CI/CD 를 사용하여 Frontend, Backend 빌드 후 docker 이미지 생성 -> swarm에 올리는 작업까지 자동화

#### 이슈 및 해결
- 새로고침시 다시 검색해야 되는 번거로움이 있다.
    - url query로 키값, 날짜값등을 가지고 있어서 url이 바뀔때 api 호출 하는 방식으로 변경
- Mysql row 데이터가 많아서 쿼리의 속도가 느리다.
    - 대시보드 상에서 로딩 추가
    - 테이블 인덱싱 추가

#### 보완점


## IotGateway Validator
---
`토이스미스 | CLI 개발 | 2019.10 ~ 2019.11`

사내에서 MongoDB를 도입하면서 Collection에 Document를 저장할 때 각각의 Collection 마다 Validator를 관리 할 수 있게 도와주는 프로그램.  
하나의 repo를 사용해서 Validator이 정의된 json 파일들을 관리가 가능하다.

#### 개발
- Typescript를 사용하여 Node.js 기반으로 개발
- gitlab v3 api를 사용하여 repo에 있는 Validator이 정의된 json 파일을 불러와 DB command를 사용하여 적용

#### 보완해야 할 점
- gitlab이 private 이므로 api를 사용할때 필요한 토큰에 대한 관리를 cli 실행할 때 인자로 넣어주게 바꾸어야 한다. 


## 티켓바이
---
`위니플 | 웹 프론트엔드, 백엔드 개발 | 2019.01 ~ 2019.03`

뮤지컬 티켓, 영화 티켓 등 중고 티켓을 거래하는 서비스

#### 개발
- Typescript를 사용하여 Frontend는 Vue.js 프레임워크 사용
- Typescript를 사용하여 Backend는 Node.js 기반 Express 프레임워크 사용
- 결제 관련 내용은 세틀뱅크 PG 사를 이용하여 연동
- 실제 서비스는 AWS S3에 올려 ClountFront로 연동
- frontend 배포는 gulp를 사용하여 AWS S3에 업로드
- Backend 배포는 EC2에서 pm2로 배포

## 위니플 서비스
--- 
`위니플 | 웹 프론트엔드 개발 | 2017.11 ~ 2018.09`

사용자들이 앱 이름, 앱 아이콘, 메뉴등을 설정하면 앱을 자유롭게 빌드하여 사용할 수 있게 해주는 서비스

#### 개발
- Typescript를 사용하여 Frontend는 Angular 프레임워크 사용
- 유저 상태 관리를 위해 Ngrx 도입
