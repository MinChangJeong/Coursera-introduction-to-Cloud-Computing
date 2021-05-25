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
