## Microservices

- Microservices 아키텍처는 단일 애플리케이션이 느슨하게 결합되고 독립적으로 배치 가능한 많은 소형 구성요소 또는 서비스로 구성되는 접근법이다.
- These services typically have their own stack running on their own containers.
- They communicate with one another over a combination of APIs, event streaming, and message brokers
 
 
 ## serverless computing
 
  - 서버리스(Serverless)는 애플리케이션 스택의 확장, 스케줄링, 패치 적용 및 프로비저닝과 같은 일반적인 인프라 관리 작업에 대한 책임을 클라우드 제공자에게 떠넘기는 컴퓨팅 접근 방식으로, 개발자는 애플리케이션 또는 프로세스에 대한 코드와 비즈니스 논리에 시간과 노력을 집중할 수 있습니다.
  - 서버가 없는 것은 서버가 없다는 것이 아니라 기본 물리적 서버 또는 가상 서버의 관리가 사용자로부터 제거된다는 것을 의미합니다.
  - 서버리스 모델은 서버 프로비저닝, 애플리케이션 스택 및 소프트웨어 설치, 개발자에 의한 인프라 운영 등을 필요로 하지 않습니다. 
  - 서버리스 컴퓨팅은 요청당 온디맨드 방식으로만 코드를 실행하며, 서비스되는 요청 수에 따라 투명하게 확장됩니다.
  - 서버리스(serverless)는 개발자로부터 인프라를 추상화합니다. 코드는 각 기능이 상태 비저장 컨테이너 내부에서 실행되는 개별 기능으로 실행됩니다. 요청을 처리하는 데 이전 실행 컨텍스트가 필요하지 않으며, 새로운 요청이 있을 때마다 함수의 새 인스턴스가 호출됩니다.


### Determing fit with serverless

applications that qualify for a serverless architecture include

- show-runnig stateless functions
- seasonal workloads
- production volumetrics data
- event-based processing

### Use case

- Data and event processing
- IoT
- Microservices
- Mobile backends

고유의 자동 확장, 신속한 프로비저닝, 유휴 시간 동안 비용이 들지 않는 가격 모델을 고려할 때, 마이크로 서비스 아키텍처를 지원하는 것은 오늘날 서버리스 컴퓨팅의 가장 일반적인 사용 사례 중 하나가 되었습니다.

- serverless is well-suited to working with
  1. tasks:
    - data enrichement
    - transformation
    - validation and cleansing
    - POF processing
    - audio normalization
    - video transcoding
    - data search and provisioning
    - Genome processing
  2. Data streams:
    - business
    - IoT sensor data
    - log data
    - fiancial market data

### Challenges

-  서버 없는 워크로드는 워크로드에 대응하여 스케일업 및 스케일다운할 수 있도록 설계되었지만, 기존 서버 환경을 관리하는 장기 실행 프로세스로 특징지어지는 워크로드의 경우 보다 단순하고 비용 효율적일 수 있습니다.
-  서버 없는 애플리케이션 아키텍처는 벤더에 따라 달라질 수 있으므로 벤더에 종속될 가능성이 있으며, 특히 인증, 확장, 모니터링 또는 구성 관리와 같은 플랫폼 기능이 포함될 수 있습니다
-  서버리스 아키텍처는 워크로드에 대응하여 확장 및 축소되므로 새로운 요청을 처리하기 위해 0부터 시작해야 하는 경우도 있습니다
