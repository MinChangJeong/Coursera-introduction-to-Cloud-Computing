## Secure Networking in Cloud

- 클라우드 네트워크를 생성하려면 먼저 네트워크의 크기나 경계 또는 클라우드 네트워크를 설정 하는 IP 주소 범위를 정의해야한다.
- 클라우드 네트워크는 VPC(Virtual Private cloud)를 비롯한 옵션을 사용하여 논리적으로 분리된 네트워크 세그먼트에 배포되며 이를 subnets이라고 하는 더 작은 세그먼트로 나눌수 있다.
- 논리적으로 세분화된 클라우드 네트워크는 private 클라우드의 보안과 public cloud의 확장성을 고객에게 제공하는 private cloud의 영역이다. 
- VM 또는 VSLs(Virtual Server Instances), storage, network connecticvity 및 load balancers와 같은 클라우드 리소스가 subnets에 배포된다.
- subnets은 클라우드 보안이 구현되는 주요 영역이다.
- 모든 subnets은 subnets 수준 방화벽 역할을 하는 ACL(Access Control List) 에 의해 보호된다.
- subnets 내에서 VSI와 같은 인스턴스 수준에서 보안을 제공하는 Security Group을 생성할수 있다.
- subnets을 구축한 후에는 application을 실행할 수 있도록 일부 VSI 및 storage를 subnets에 추가 해야 한다.

ex) 웹 액세스 VSI, application 계층 VSI 및 백엔드 데이터베이스 VSI가 필요한 3계층 애플리케이션이 있다고 가정
   이경우 VSI를 향한 웹을 하나의 Security Group에 배치하고 애플리케이션 vsi는 두번째 Security Group에 배치하고 데이터 베이스 VSI는 세번째 Security Grout에 배치하게 된다.
  
