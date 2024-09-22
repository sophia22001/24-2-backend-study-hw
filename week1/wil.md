### 주제: 웹과 백엔드

## 1. 웹

- 클라이언트-서버 패러다임으로 정보를 주고받는다.

## 2. 프로토콜과 HTTP

- 프로토콜: 네트워크를 할 때 필요한 규칙
- 웹 -> HTTP 프로토콜

### HTTP method & URL

- HTTP로 요청할 때는 HTTP method와 URL이 필요하다.
- **HTTP method**: 데이터를 다루는 방법
- **URL**: 다룰 데이터의 위치
  - ex> GET http://www.naver.com

### HTTP method 종류

- `GET`: 데이터 가져오기
- `POST`: 데이터 게시하기
- `PUT`: 데이터 교체하기
- `PATCH`: 데이터 수정하기
- `DELETE`: 데이터 삭제하기

### URL 구조

: scheme, domain, path

### query string

: .com/post/search?page=1&keyword=hello에서 **?page=1&keyword=hello**

### HTTP 헤더와 바디

- HTTP 데이터는 HTTP 헤더와 HTTP 바디로 구성된다.
- **HTTP 헤더**: 언제, 누가, 어떤 경로로 보내는 지, HTTP method가 무엇인지 등의 통신에 대한 정보
- **HTTP 바디**: 주고 받으려는 데이터 (보통 json)

### 상태 코드

- 요청에 대한 처리 결과는 HTTP가 정의하는 상태 코드로 나타낸다.
- 상태 코드는 응답 데이터의 HTTP 헤더에 들어간다.
- ex> 200 OK

## 3. 프론트엔드와 백엔드

: 자주 변하는 화면 UI(프론트엔드)와 자주 변경되는 컨텐츠(백엔드)를 분리하자.

- 프론트: 화면에 채울 컴텐츠 데이터를 백엔드에게 *요청*하면,
- 백엔드: DB에서 가져온 데이터를 프론트에게 *응답*한다.

## 4. API (Application Programming Interface)

HTTP는 단순한 웹의 규칙이므로 구체적인 통신 방법은 API로 직접 정의할 수 있다.
== 어플리케이션의 사용 설명서

- 백엔드 API: 어떤 http method, url을 사용해야 할지, 어떤 응답을 보내는 지 정의하는 것.

### REST (Representational State Transfer) API

: REST 아키텍처를 따르도록 설계한 API

### 프로젝트 진행 과정

1. API 설계
2. DB, ERD 설계
3. API 서버 프로그램 작성
4. 테스트
5. 배포
