## Overview of Cloud Infrastructure

서비스 모델 +  클라우드 유형 다음에는 인프라 아키텍처를 계획해야함
인프라 계층은 클라우드를 기반이다
이 계층은 영역 및 데이터 센터에 있는 물리적 리소스로 구성됨
클라우드 제공자의 IT환경은 전세계여러 지역으로 분산되어있음
클라우드 영역이란 클라우드 제공자의 인프라가 클러스터된 지리적영역 또는 위치 NA South 또는 US Easte와 같은 이름을 가짐
클라우드 지역은 다른 지역이 피해를 입더라도 클라우드 운영이 계속 되도록 서로 격리되어있다.
각클라우드 영역에는 여러개의 영역  = 가용성 영역  == AZ 이 있을수 있다.
AZ에는 고유한 전력, 냉각 및 네트워킹 리소스를 가진 고유한 데이터 센터이다.
이러한 영역은 DAL-09, us-east-1 과같은 이름을 가짐
영역을 분리하면 클라우드 전체 장애확률 떨어짐, 지연시간 단축, 단일공유장애지점 생성 X 
AZ는 높은 대역폭 네트워크를 연결하여 다른 AZ 및 지역, 개인 데이터 센터 및 인터넷에 연결된다.
클라우드 데이터 센터는 클라우드 인프라를 포함하는 대규모 회의실 또는 창고
이 데이터 센터에는 팟, 랙, 서버, 스토리지 및 네트워킹 장비와 같은 컴퓨팅 리소스의 표준화된 컨테이너가 포함되어 있음
클라우드 데이터 센터의 대부분의 서버는 하이퍼바이저를 실행하여 가상화 기술을 기반으로 소프트웨어 기반 컴퓨터인 가상 서버
또는 가상 시스템(VM)을 생성한다.
랙의 다른 서버는 가상화되지 않은 물리적 서버인 베어메탈 서버
고객은 필요할때 VM,  베어메탈 서버를 프로비저닝하고 워크로드를 실행한다.
클라우드 사용자는 가상 머신 위에 있는 추상화 계층인 서버리스 컴퓨팅 리소스에서도 워크로드 실행가능

Computing Resources

cloud providers offer several compute options
- Virtural Servers: software based
- Bare Metal Servers : pysical servers
- Serverless computing resources : abstraction

 Storage
 
 - vm, bare meatal server모두 사용자의 on-demand방식으로 provision할수 있다.
 - vm, bare metal server모두 default storage를 가지고 있다.
 - 또한 storage option이 존재하는데 사용자가 얼마나 자주 쓰는지, 얼마나 중요하게 생각하는지 얼마나 보안에 신경쓰는지에따라 Block storage, file storage, object storage를 포함 하고있다.
 - 하지만 block 과 file storage는 규모와 performance의 어려움 때문에 전통적인 방식으로 머무르고 object storage방식을 더많이 쓴다.

  Networking
  
  - 네트워킹 인프라는 routers, switcher와 같은 전통적인 네트워크 하드웨어를 포함한다.
  - 클라우드안에 있는 서버가 제공되면 너는 public 과 private network interface를 셋업 할 필요가 있다.
  - public interface : connect the servers to the public internet
  - private interface : provide connectivitiy to your other cloud resource and help keep them secure
  - 네트워크 인터페이스안에서 클라우드느 개인 ip 주소와 subnets를 필요로 한다.
  - 

