## Virtualization and Virtual Machines Explained

### virtualization ?
- virtualiazation (가상화) is the process of creating a software based or virtual, version of something whether that be compute, storage, networking, servers, or applications
- virtualization을 가능하게 해주는 것은 hypervisor이다.
- hypervisor is a peace of software that runs above the pysical server of host


## Hypervisor
- type 1 : BM(Bare Metal) => 물리적인 서버위에 직접적으로 설치되는 하이퍼바이저
  - ex) VMware, ESXi, Microsoft Hyper-v, open-source KVM
- type 2 : Hosted => type1과 다른점은 host와 하이퍼바이저 사이에 host OS layer가 자리한다.
  - ex) oracle, virtualBox

hypervison을 설치하게 되면 가상 환경 또는 가상머신을 구축할수 있게 된다
VM 은 독립적이여서 다른 OS를 run 할수 있는데 host(local host)웨에 하이퍼바이저를 깔고 여러개의 vm , 예를들어 window, linux, unix등을 run 할수 있게 된다.

## benefits

1. cost savings
2. agility and speed
3. lower your downtime

# Virtual Machines = Virtaul Servers = Virtual Instance = Instance     depending on the cloud provider

 When you create a virtual server in the cloud, you specify the Region and Zone or Data Center you want the server to be provisioned in and the Operating System you want on it. You can choose between shared (that is, a multi-tenant) VMs or dedicated (that is, a single-tenant) VMs. You can also choose between hourly or monthly billing, and select storage and networking options for the virtual server
 
## Types of Virtual Machines


### Shared or Public VMs
 - are provider-managed, multi-tenant deployments that can ve provisioned on-demand with predefined size
 - Being multi-tenant means that the underlying pysical server is virtualized and is shared across other tenats or users

### Transsient or Spot Vms
 -  take advantage of unused capacity in a cloud data center
 -  testing and developing applications. They are also useful for running stateless workloads, testing scalability, or running big data and high performance computing (HPC) workloads at a low cost

### Reserved virtual server instaces
 - reserve capacity and guarantee resources for future deployments

### Dedicated Hosts 
 -  dedicated hosts offer single-tenant isolaton
 -  This means that only your VMs run on a given host so they can make exclusive use of full capacity and resources of the underlying hardware.
 -  전용 호스트는 일반적으로 컴플라이언스 및 규정 요구사항을 충족하거나 특정 라이센스 조건을 충족하는 데 사용됩니다.

