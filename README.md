소프트웨어 아키텍쳐

Anti Fragile?
	Auto scaling - 조건에 따라 자동으로 처리할 수 있는 능력
	Microservices - 넷플릭스 / 아마존 -> 클라우드를 가장 잘 맞춰짐. 넷플릭스가 클라우드에 굉장히 적극적이죠. 
	Chaos engineering -> 시스템이 급격한 예측하지 못한 상태라도 버틸 수 있는 그러한 규칙 / 예견되지 않은 불확실성에서도 안정적으로 서비스를 제공해줘야 합니다.
	Continuous deployments -> CI CD -> Continuous Integration / Continuous Deployment / Development
	

Cloud Native Architecture?

	1. 확장 가능한 아키텍쳐
		시스템의 수평적 확정에 유연하다
		확장 된 서버로 시스템의 부하 분산, 가용성 보장
		시스템 또는, 서비스 애플리케이션 단위의 패키지 (컨테이너 기반 패키지)
		모니터링

	2. 탄력적 아키텍쳐
		서비스 생성 - 통합 - 배포, 비즈니스 환경 변화에 대응 시간 단축
		분활 된 서비스 구조
		무상태 통신 프로토콜
		서비스의 추가와 삭제를 자동으로 감지
		변경된 서비스 요청에 따라 사용자 요청 처리(동적 처리)
	
	3. 장애 격리 (Fault isolation)
		특정 서비스에 오류가 발생해도 다른 서비스에 영향 주지 않음


Cloud Native Application?

	1. 마이크로 서비스로 개발 된다.
	2. CI/CD를 통한다.
	3. DevOps 가 가능하다.
	4. 컨테이너 가상화 기술을 활용한다.

	CI  -> 지속적인 통합 / Jenkins, Team CI, Travis CI -> 통합 서버 / 소스 관리 / 빌드 도구 / 테스트 도구
	CD -> 지속적인 배포 -> Continuous Delivery(수동반영) / Continuous Deployment(자동반영) / Pipe line


Service Discovery 
	일종의 전화번호 책같다고 생각합시다.. - 서비스 등록 / 서비스 검색에 관련한 일을 해주는데 -> Netflix - Eureka 를 활용하겠습니다..
	Java-Spring 재단에 기부를 했습니다.. 감사합니다 넷플릭스 형님.. 잘 사용하겠습니다.
	Eureka Server 
	Client -> API GATEWAY (LOAD BANLANCER) -> SERVICE DISCOVERY(EUREKA) -> SERVER 1 OR SERVER 2 OR SERVER 3 
	요청정보에 따라 필요한 서비스의 위치를 알려주는 서비스라고 생각할 수 있습니다..








	
