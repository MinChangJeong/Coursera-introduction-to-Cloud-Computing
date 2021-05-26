## Basics of Storage on Cloud

### Storage Types

1. Direct Attached
  
  - Local storage
  - Within same server or rack
  - fast
  - use for os
  - Ephemeral(Temporary == only lasts as long at the compute resource it's attaced to, not shared, not resiliance)

2. File Storage
 
 - NFS Stroage
  
  - 단점
    - slower than either direct-attached storage or block storage
    - 
  - 장점
    - lower cost than either direct-attached storage or block storage
    - attach to multiple servers

3. Block Storage
  - 장점
    - faster read/write speeds and reliable than file storage


#### cf) 
- IOPS : Input/Output Operations per Second
- Persistence : What happens to the storage once the compute node it is attached to is terminated
- SnapShot : A point in time image of the storage
  - fast to create
  - don't require downtime
  - record only changes to data
  - can't recover individual files

4. Object Storage

  - 단점
    - slowest spped
  - 장점
    - least expensive
    - infinite in size


## File Storage

- like direct-attatecd, attacted to a compute node a sotre data
- less expensive
- more resilient to failure
- less disk management & maintenance for user
- provision much larger amounts of storage
- File Storage is mounted on compute nodes via ehternet networks
  - network dedicated for storage
  - network attached storage or network file storage(NFS)
  - speeds vary based on network traffic
  - for workloads where consistent speed is not required
- IOPS : Input /Output Operations Per second - the speed at which the disks can write and read data
  - higher IOPS value = faster speed of underlying disk
  - higer IOPS = higher const
  - Low IOPS value can become a bottleneck


## Block Storage
