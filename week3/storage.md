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

- Block storage breaks files into chunks(or blocks) of data and store each block separately under a unique address
- must be attatched to a compute node before it can be utilized
- Mounted from remote storage appliances
- extremely resilient to failure
- data is more secure
- single move at the speed of light
- higer price-point
- perfect for workloads that need low-latency
- consistent high speed
- database and mail servers
- not suitable for shared storage between multiple servers
- IOPS
  - specify iops charcteristics
  - adjust the iops as needed
  - depending on requirements and usage behavior

### Common Attributes of File & Block Storage

- Block and File storage is taken from appliances which are maintained by the service provider
- Both are highly available and resilient
- often include data encryption at rest and in transit (종종 정지 상태 및 전송 중인 데이터 암호화를 포함합니다.)

- File Storage
  - Attached via ethernet network
  - speeds vary, based on load
  - can attach to multiple compute nodes at once
  - good for file shared where : fast connectivity isn't required, cost is a factor

- Block storage
  -  attached via high-speed fibre network
  -  only attach to one node at a time
  -  good for applications that need : consistent fast access to disk

#### Remember to consider the IOPS requirements of the application when provisioning either file or block storage


## Object Storage

- Object Storage is used to store files or Objects which are static. 
- The data that you can store using Object Storage can be anything from text files to audio and video files, from IOT data to virtual machine images, from backup files to data archives.
- You cannot run operating systems or other applications such as databases using Object Storage.
- Objects are stored in Buckets. You can have multiple buckets, but you cannot place buckets within buckets.
- You do not need to specify a size for a bucket, you can just use as little or as much space as you need. 
- Many providers offer different types of buckets with different charges for each. Some are based on resilience and availability, while others are based on the frequency at which the objects inside are accessed.

### Object Storage - Tiers and APIs

- Object Storage Tiers
  - Object Storage buckets also have storage tiers, or classes, associated with them, and these tiers are based on how frequently the data is accessed. 
  - A standard tier bucket is where you would store objects that are frequently accessed
  - vault or archive tier is where you might store documents that are only accessed perhaps only once or twice a month, or less, and this will be offered at a lower storage cost. 
  - cold vault tier, where you would store data that is typically accessed only once or twice a year.
  - utomatic archiving rules for your data, meaning that if an object isn't accessed for a period of time, it will automatically be moved to a cheaper storage tier
  
- Application Program Interface or API
  
  
    <img align="center" width="1280" alt="2021-05-27" src="https://user-images.githubusercontent.com/65451455/119764455-602c3000-beec-11eb-8742-6dc4bc21099a.png">


