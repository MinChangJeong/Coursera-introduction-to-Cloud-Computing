## Overview of Cloud Service Models

## Three Model 

### IaaS 

- 사용자가 원하는 방식으로 접근하고 구성할 수 있도록 cloud제공자가 가상화한 컴퓨팅 네트워킹 및 저장 리소스 set입니다.
- Personas 라고 불리는 사용자는 IaaS의 시스템 관리자이자 IT 관리자이다.
- IaaS cloud 제공자는 Data centers, Colling, Power, Networing&Security, Servers&Storage 등을 관리한다.

### Paas

- Platform as a Service는 IaaS로 부터의 가상화된 리소스를 이용하고 추상화한다.
- PaaS의 유저는 보통 시스템 관리자가 아니고 보통 "dev"라고 부르는데 'IBM'에서는 보통 "개발"이라고한다.
- PaaS cloud 제공자는 Platfrom Infrastructure 를 관리하는데 Operating System(os), development tools, database, business analytics등을 포함한다.

### SaaS

- Software as a Service 는 자신이 가지고있는 장비에 설치하거나 업데이트 하지 않아도 되는 sw이다.
- SaaS는 모든 사람이 다 유저가 될 수 있다. (ex 우리가 유튜브를 본다면 우리는 youtube(SaaS)의 user가 되는 것이다.)
- 보통 일회성 라이센스 요금을 지불하는 모델이라기보다 구독료를 지불하는 모델이다.
- SaaS 모델에서는 인프라 및 플랫폼 리소스 외에도 제공자가 애플리케이션과 데이터를 호스팅하고 관리합니다.

- SaaS에서 IaaS로 내려갈수록 인프라 리소스에대한 지식과 관리 측면에서 복잡성이 증가하고 사용자의 용이성이 증가한다.

# IaaS - Infrastructure as a Service

- Iaas is a form of cloud computing that delivers funmental(근본적인) compute, network, storage resource to consumers on-demand, over the internet, on a pay-as-you-go-basis.
- Iaas 는 전통적으로 사내 데이터 센터에서 제공하는 인프라 구성요소와 가상화 또는 hypervisor layer를 hosting한다.
- IaaS 클라우드 환경에서는 소비자가 virtual machines을 생성하고 제공할 수 있다.
- 클라우드 제공자는 소비자들에게 자신들이 수행하는 일을 추적하고 모니터 할수 있고 클라우드 서비스의 사용과 disaster를 복구할 수 있게 한다.

### cf) Key Components of Cloud infrastructure

- Phsical data centers : IaaS 공급자는 추상화의 다양한 계층을 지원하는 데 필요한 물리적 머신을 포함하는 대규모 데이터 센터를 관리합니다.
- Compute :  IaaS 공급자는 하이퍼바이저를 관리하고 최종 사용자는 원하는 양의 컴퓨팅, 메모리 및 스토리지 리소스로 가상 인스턴스를 프로그래밍 방식으로 provision 합니다.
- Network : 사용자는 가사화 또는 프로그래밍 방식으로 API를 통해 클라우드에서 네트워크 리소스에 접근할 수 있다.
- Storage : cloud data storage에는 object(most common mode of storage in the cloud), file, block storage 3가지 타입이 있다


### typical use cases

1. Test and Development
- Enable their teams to set up test and development environments faster.
- Helping developers focus more on business logic than infrastructure manegement

2. Business Continuity and Disaster Recovery
- Require a significant amount of technology and staff investments.
- Make applications and data accessible as usual during a disaster or outage

3. Faster Deployments and Scaling
- To deploy their web applications faster
- Scale infrastructure up and down as demand fluctuates

4. High Performance Computing
- To solve complex problems involving millions of variables and calculation

5. Big Data Analysis
- Patterns, trends, and associations requires a huge amount of processing power
- Provides the required high-performance computing but also makes it economically vialble


# PaaS - Platform as a Service

- PaaS 는 완전한 어플리케이션 플랫폼을 제공하는 클라우드 컴퓨팅 모델이다.
- develop, deploy, manage, and run application 플랫폼 제공
- PaaS 제공자는 Host & Mangaeg => Servers, NetWork, Storage, OS, Application runtimes, APIs, Middleware, database
- PaaS는 Installation, Configuration, Operation of Application Infrastructure 등을 책임진다.
- IaaS를 사용하면 클라우드 제공자가 서버, 스토리지 및 네트워킹과 같은 '원시' 컴퓨팅 리소스에 액세스할 수 있고 사용자는 플랫폼 및 애플리케이션 소프트웨어를 담당합니다. 클라우드 서비스 프로바이더는 PaaS를 통해 전체 플랫폼 인프라를 제공하고 관리하며, 환경의 하위 수준 세부 정보로부터 사용자를 추상화합니다.


### Essential Characteristics of PaaS

- High level of Abstraction : Eliminate complexity of deploying applications
- Support Services and APIs : Simplify the job of developers
- Run-time environments : Execute code according to application owner and cloud provider policies
- Rapid deployment mechanisms : Deploy, run, and scale apllications efficiently.
- Middleware capabilities : Support a range of application intrastructure


### Use case

- API development and management 
- Internet of Things(IoT)
- Business analytics / intelligence
- Business Process Management (BPM)
- Master data management (MDM)


### Advantages of PaaS

- Scalability : made possible because of the rapid allocation and deallocation of resources with a pay-as-you-use model offered by PaaS
- Faster time to marget :  Middleware capabilities also reduce the amount of code that needs to be written while expanding the application’s functional capabilities.
- Greater agility and innovation : you can experiment with multiple operating systems, languages, and tools without having to invest in these resources.


### PaaS available offerings

- AWS Elastic Beanstalk
- Cloud Foundry
- IBM Cloud Parks
- Window Azure
- RedHat OpenShift
- Magento commerce Cloud
- Force.com
- Apach Stratos


### Rist of PaaS

- information security threats
- Dependency on service provider's infrasturcture
- Customers lack control over changes in strategy, service offerings, or tools


# SaaS - SoftWare-as-a-Service

- SaaS is a cloud offering that provides access to a service provider's cloud-based software.
- Provider maintains => Servers, Database, Application code, Security.
- Providers manage Application => Security, Availability, Performance


### SaaS Supports

- Email and Collaboration : Ms office 265, Gmail
- Customer Relationship Management : NetSuite CRM , Salesforce
- Human Resouce Management : Workday, SAP SuccessFactors
- Finanial Management


### Key Characteristics

- Multitenat Acritecture : infrastructure and code are maintained centrally and accessed by all users
- Manage Privileges and Monitor Data 
- Security, compliance, and maintenance are all part of the offerings
- customize Applications
- Subscription Model
- Scalable Resources


### Key Benefits

- Greatly reduce the time from decision to value
- Increase workforce productivity and efficiency
- User can access core business apps from anywhere
- Buy and deploy apps in minutes
- Spread out sw costs over time


### Use Case
 ##### Oragnizations are moving to SaaS to :
- Reduce on-premiss IT infrastructure and capital expenditure
- Avoid ongoing upgrades, maintenance and patching (지속적인 업그레이드 유지 패치를 피하기 위해서)
- Run application with minimal input
- Manage websites, marketing sales, and operations
- Gain resilience and business continuity of the cloud provider (클라우드 프로바이더의 비즈니스 복원력 및 유지성 확보)
 
 #### Trending towards SaaS integration platforms
 
 
 ### Concerns
 
 - data ownership and data safety
 - third-party maintains business-critical data
 - nedss good internet connection






 



