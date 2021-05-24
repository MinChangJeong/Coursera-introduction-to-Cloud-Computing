# DeploymentModel

#### Depolyment models indicate

- where the infrastructure resides (인프라가 상주하는 곳)
- who owns and manages it (모델을 소유하고 관리하는 자)
- how cloud resources and services are made available to users (어떻게 클라우드 리소스와 서비스가 유저에게 제공하는 방법)

#### Depoloyment model은 위의 세가지를 알수 있다.

## Public

- users get access to servers, storage, network, security, and applications as services delivered by cloud service
- Useing web consoles and APIs, users can provision the resources and services they need
- The cloud provider owns, manage, provisions, and maintains the infrasturcture
- Public clouds offer cost savings as the provider bears all the capital, operational, and maintenance expoense for infra and the facilities they are hosted in 
- user does not have any control over the computing  environment 


### Public cloud providers in the market 

- aws
- Azure
- IBM Cloud 
- Google Cloud 
- Alibaba Cloud


### Public cloud characteristics

- Virtualized multi-tenant architecture enabling tenats or users to share computing resources (사용자가 리소스를 공유할수 있는 multi-tenant 구조)
  - single-tenant로는 클라우드 제공자의 인프라, 플랫폼, sw를 포함하는 리소스 풀을 사용할 수 없다.
- Resources are distributed on an as-needed basis offered through a variety of subscription and pay-as-you-go-models


### Public cloud benefits

- on-demand resources : allowing applications to response seamlessly to fluctuation in demand
- Economies of scale : Considering the large number of users that share the centralized-cloud-resources on-demand
- Highly reliable : if on physical component falls, the service still runs unaffected on the remaining avilable components


### Public cloud concerns

- Security
  - Data breaches, data loss, account hijacking, insufficient due dilligence, and system and application vulnerability
- Data sovereignty compliance (데이터 주권 준수)
  -  It's increasingly critical for compliant with data sovereignty regulations governing the storage, transfer, and security of data


### Public cloud use cases

1. Building and testing applications and reducing time-to-market for their products and services
2. Business with fluctuating(변동하는 비즈니스) capacity and resourcing needs (용량과 리소스 요구가 변동하는 비즈니스)
3. Build secondary infrastructures for disaster recovery, data protection, and buisness continuity
4. Cloud storage data management services for greator accessbility, easy distribution, and backing up their data
5. IT departments are outsourcing the management of less critical and standardized business platforms and applications to public cloud providers


## Private Cloud


### Internal or External

1. Internal Infrastructure
  - on-premiss : owned and managed by organization

2. External Infrastructure
  - owned, managed, and operated by service provider


### Virtual Private Cloud (VPC)

- An external cloud that offerings a private, secure, computing, environment in a shared public cloud
    -VPC는 조직에서 공유 public cloud의 논리적으로 분리된 부분에 자체 private 및 보안 클라우드와 유사한 컴퓨팅 환경을 구축할 수 있도록 지원하는 퍼블릭 클라우드 오퍼링입니다.


### Benefits of Private Clouds

- controllerd by internal IT
- Reduced costs
- Better Scalability
- Controlled Access security
- Greater Agility


### Common Use cases

- Modernize and unity in-house & legacy applications (applicaion을 통합하고 모더나이징 한다)
- Integrate data & application services from existing applications
    - 이를 통해 private 클라우드의 컴퓨팅 기능을 더 큰 작업에 활용하는 동시에 private 클라우드의 애플리케이션에 데이터를 가져와 public 클라우드 서비스를 활용할 수 있습니다. 이는 데이터 센터가 클라우드 서비스와 함께 작동하도록 하는 데 필수적입니다. 
-  Build applications anywhere & move them without compromising security or compliance
- Full control over critical security & compliance issues within dedicated cloud


## Hybrid Cloud


- Hybrid Cloud는 조직의 사내 private cloud와  타사 public cloud를 유연한 단일 인프라로 연결하여 조직의 애플리케이션과 워크로드를 실행하는 컴퓨팅 환경입니다.
- Flexibility, workloads move freely, choice of security & regulation features
   - 일정한 용량을 사용하는 중요한 업무에 해당하는 application이나 workload를 처리할 때는 private cloud
   - 덜 민감하고 다이나믹한 workload를 처리할때는 public cloud를 사용함
- 추가 public cloud 용량을 활용하여 클라우드 확장이라고도 하는 private cloud application에 대한 수요 증가를 수용할 수 있습니다. 
 
 
 ### The Three Tenets(주의, 교리)

1. interoperability (상호운용성)
  - Public & Private clouds understand each other's APIs, configuration, data formaats, authentication & authorization

2. scalability (확장성)
  - Private clouds can leverage Public cloud capacity

3. portability (휴대성)
  - Move applications & data between on-premiss, cloud system & cloud service providers


### Types of Hybrid Clouds

1. Hybrid MonoCloud
  - one cloud provider 

2. Multicloud
  - open standards-based stack that can be on any public cloud infrastructure (개방형 표준 기반 스택)

#### Hybrid MultiCloud가 한 Provider에서 다른 Provider로 workload와 환경을 이동할 수 있는 유연성을 제공한다는 점에서 차이가 있습니다.

3. composite Multicloud
 - Greater flexbility
    - 이를 통해 단일 애플리케이션을 여러 공급업체에 분산시킬 때 유연성이 더욱 세분화되어 필요에 따라 클라우드 서비스 및 공급업체 간에 애플리케이션 구성 요소를 이동할 수 있습니다.


### Benefits

- Security and compliance
- Scalability and resilience
- Resource optimization
- const-saving


### Hybrid Cloud Use Case

- Software-as-a-Service integration
- Data & AI integration
- Enhancing legacy apps
- VMware migration
- 




