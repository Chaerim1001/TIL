# 목차

- [목차](#목차)
- [HTTP란](#http란)
- [HTTP 특징](#http-특징)
  - [클라이언트-서버 구조](#클라이언트-서버-구조)
  - [Stateless](#stateless)
  - [Connectionless](#connectionless)
- [HTTPS vs HTTP](#http-vs-https)
  <br>

# HTTP란

- HTTP - HyperText Transfer Protocol)
- HTTP란 텍스트 기반의 통신 규약으로 인터넷에서 주고받을 수 있는 **프로토콜** 이다.
  - 프로토콜(protocol): 서로 다른 시스템에 있는 개체 간에 데이터를 전송하는 통신 규약
- WWW(World Wide Web)에 내장된 프로토콜이다.

 <br>

# HTTP 특징

## 클라이언트-서버 구조

- 클라이언트가 서버에 요청을 보내면 요청을 받은 서버는 그에 대한 적절한 응답을 보내주는 구조

## Stateless

- HTTP 통신은 state 개념이 존재하지 않는다. -> **무상태 프로토콜**
- 서버가 클라이언트의 상태를 저장하지 않는다.
- 장점: 서버 확장성이 높다.
- 단점: 클라이언트가 추가적인 데이터를 포함하여 서버에게 요청을 보내야 한다.

## Connectionless

- HTTP는 기본이 연결을 유지하지 않는 모델이다. -> **비연결성**
- 실제 요청을 주고 받을 때만 연결을 유지하고 응답을 주고나면 TCP/IP 연결을 끊는다.
- 장점: 최소한의 자원으로 서버 유지가 가능하며, 트래픽이 많지 않고 빠른 응답을 제공할 수 있는 경우에 효율적으로 작동한다.
- 단점: 트래픽이 많고 큰 규모의 서비스를 운영할 때에는 한계가 있다.
- HTTP 초기에는 각각의 자원을 다운로드하기 위해 연결과 종료를 반복해야 했지만 **HTTP 지속 연결 (Persistent Connections)** 를 사용하면 연결이 이루어지고 난 뒤 각각의 자원들을 요청하고 모든 자원에 대한 응답이 돌아온 후에 연결을 종료한다.

  <br>

# HTTP vs HTTPS

## HTTPS란

- HTTPS는 HTTP에 S가 붙은 것이다. 여기서 S는 Over **Secure** Socket Layer의 약자로 Secure에서 알 수 있듯이 보안이 강화된 HTTP이다.

- HTTP는 암호화되지 않은 방법으로 데이터를 전송하기 때문에 서버와 클라이언트가 주고 받는 메시지를 제 3자가 감청하고 조작하기 매우 쉽다. HTTP의 이러한 보안적인 부분을 보완한 것이 HTTPS이다.

> 출처
> <br> https://opentutorials.org/course/228/4894
