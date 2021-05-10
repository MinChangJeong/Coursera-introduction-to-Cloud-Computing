## Defintion and Essential Charateristics of Cloud Computing

### 클라우드란?

#### NIST 정의 

- 최소한의 관리 작업이나 서프스 프로바이더의 상호 작용으로 신속하게 프로비저닝 및 릴리스 할 수 있는 구성 가능한 컴퓨팅 리소스의 공유 풀에 대한 편리한 on-demand Network 접근을 지원하는 모델 

### Cloud Model 
- 5 Essential Characteristics 
- 3 Deployment Models
- 3 Service models

#### 5 Esstial Charcteristics

1. on-demand Self service
  각 서비스의 provider와 인적 상호작용 없이 간단한 interface를 사용하여 processing power, storage, network(you need)
  등의 cloud resource에 접근할수 있는 것을 의미한다.

2. Broad Network Access
  표준 메커니즘과 휴대폰, 태블릿, 노트북 및 workstations과 같은 플랫폼을 통해 네트워크를 통해 클라우드 컴퓨팅 리소스에 액세스 할수 있다는 것을 의미한다.

3. Resource Polling
  클라우드 제공자가 고객에게 전달하는 규모의 경제를 제공하여 클라우드를 비용 효율적으로 만드는 요소이다. 
  Multi-tenant Model(tenant : 소작농) 을 사용하여 컴퓨팅 리소스를 polling하여 여러 소비자에게 서비스를 제공하고 
  클라우드 리소스를 동적으로 할당 및 재할당한다. 
  고객들은 이러한 리소스의 물리적 위치를 신경쓰지 않아도 된다.

4. Rapid Elastic 
  resource are elastically provisioned and released 되기 때문에 필요한 경우 더 많은 리소스에 액세스하고 필요하지 않은 경우 
  다시 확장 할 수 있음을 의미한다.
  
5. Measured Service 
  자신이 사용하거나 예약한 것에 대해서만 지불한다는 것을 의미한다.
  리소스 사용은 활용률에 따라 투명하게 모티터링, 측정 및 보고 된다.
  
##### Summary
  * 클라우드 컴퓨팅은 "서비스로서의 기술"을 활용하고, 개방형 인터넷을 통해 on-demand 방식으로 원격 시스텔을 활용하고,
      scaling up, scaling back 하며 사용한 만큼 비용을 지불하는 것이다. 
  
  *전 세계가 컴퓨팅 서비스를 소비하는 방식, 즉 비용 효율성을 높이는 동시에 기업의 시장 변화에 보다 민첩하게 대응할 수 있도록 지원한다.
      
#### 3 Deployment Model

1. Public
  - 클라우드 제공자가 소유한 하드웨어에서 개방형 인터넷을 통해 클라우드 서비스를 활용하지만 그 사용량은 다른 회사에서 공유하는 것을 말한다.
2. Private
  - 클라우드 인프라를 단일 조직에서 독점적으로 사용하도록 provisioned 하는 것을 의미한다.
  - 사내에서 실행하거나 서비스 공급업체가 소유, 관리 및 운영할 수 있다.
3. Hybrid
  - public, private를 함께 사용하여 원할하게 함께 작업하는 경우를 의미한다.

### Computer Stacks
- Infrastructure (IaaS)
  인프라 및 물리적 "컴퓨팅 리소스" (ex> Server, Network, Storage, Data center space)를 관리하거나 운영할 필요 없이 접근할 수 있다.

- Platform  (Paas)  
  일반적으로 인터넷을 통해 애플리 케이션을 개발하고 사용자에게 배포하는데 필요한 하드웨어 및 소프트웨어 툴인 플랫폼에 접근 할수 있다.

- Application (SaaS)
  소프트웨어와 애플리케이션이 중앙에서 hosting되고 구독에 license가 부여되든 소프트웨어 라이센스 및 전송 모델이다.
