# GraphQL로 영화 API 만들기

## 📌 용어 복습
- ### API(Application Programming Interface)
  - 컴퓨터나 컴퓨터 프로그램 사이의 연결, 주로 프로그래밍할 때 사용하고, 어플리케이션과 상호작용할 때 사용한다.
  - 인터페이스 - interaction + face라고 이해하면 이해하기 쉽다. 서로 상호작용하는 방식

- ### REST API
  - 간단하게 말해서 URL의 모음이다. URL에 따라 각 기능에 맞는 HTTP 메서드를 사용하고, 그 URL을 서버에 요청하고 응답을 받으면서 각각 다른 작업을 한다.
  - URL에 해당 기능의 동작을 의미하는 단어를 사용하지 않고, 어떤 HTTP 메서드를 사용하느냐에 따라 기능을 분리한다.

## 📌 REST API나 GraphQL은 어떨 때 사용될까?
- 백엔드와 통신하기 위해서, 예를 들어 사용자가 데이터베이스의 데이터를 요청했을 때 서버에서 데이터를 가져오고, 그 데이터를 이용해서 사용자에게 보여줘야한다.

## 📌 REST API의 단점
- `OverFetching` : 내가 원하는 데이터가 소량이거나, 대량이거나 항상 너무 많은 데이터를 받는다, 내가 필요로 하지 않는 데이터까지 다 불러오는 문제, 즉 백엔드에서 프론트엔드로 보내줄 데이터가 많아지기 때문에 전송 속도가 느려질 수 있다.

## 📌 GraphQL의 해결책
- `UnderFetching` : 데이터를 전부 받아오지 않고, 내가 필요로 하는 데이터만 정의해서 요청할 수 있다. GraphQL API는 필요한 모든 데이터를 `단일 Request`로 가져온다. 그렇기 때문에 느린 모바일 네트워크 환경에서도 빠를 수 있다.



> ### Reference 
> [https://nomadcoders.co/graphql-for-beginners/lobby](https://nomadcoders.co/graphql-for-beginners/lobby)