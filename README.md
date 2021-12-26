# Micro Service with Spring Cloud

위 프로젝트는 기존의 
1. Spring MVC -> https://github.com/hyunsooryu/spring-web-mvc
2. Spring REST API - HATEOAS  -> https://github.com/hyunsooryu/spring-restApi
를 이은 3번 째 데모 프로젝트 이다.

### 들어가며
간단한, 회원, 주문, 상품, 매장 도메인의 Micro Service를 구현해본다.
https://github.com/hyunsooryu/Simple-MSA-Architeture
위의 기존의 FrontServer, ApiServer, Spec 형태로 통합 하였던 maven Project는 그 한계점이 명확했다.
이번 데모 프로젝트에서는 간단한 Shopping App Api를 구현해보며
1. AutoScaling
2. Chaos Engineering
3. Continuous Integration / Continuous Deployments
4. MicroServices

이 4가지 원칙을 잘 지킬 수 있는 방향으로 구현할 것이며, 확장 가능한 아키텍쳐와 탄력적인 아키텍쳐, Stateless한 통신 프로토콜을 잘 지켜내는 Cloud Native Architecture을 지향할 것이다.

사용기술은
Spring Boot 2.5.x, Spring Cloud, Spring Data JPA, H2 Database, Redis, MongoDB, Apache Kafka, Rabbit MQ, Docker, Zipkin, Grafana 이며
빌드 툴은 maven을 활용한다.

추가적으로 이번 기회의 Container에 Netty 를 활용한다.(Spring Cloud Gate Way 특성상)
이 후 4번째 데모 프로젝트에서는 Reactor 기반의 비동기 프레임워크인 Spring-webFlux에 대해 논해본다.

