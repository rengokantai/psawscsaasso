# psawscsaasso
## Understanding Amazon Route 53
### 2 Route 53 Characteristics
You can extend on-premise DNS to Amazon VPC  
You cannot extend Route 53 to on-premises instances  
You cannot automaticcally register EC2 instances with private hosted zones


###  DNS records
```
nslookup
set type=mx
google.com
```
#### 07:11
A record: ip address of href  
PTR record: href of ip

```
set type=ptr
8.8.8.8
```

## 4.Understanding and Configuring NAT Instances gateways, and VPC Endpoints
#### 02:11
NAT Instances
- Use a script tp manage failover berween instances
- Depends on the bandwidth of the instance type
- Managed by you
- A generic Amazon linux AMI that's configured to perform NAT
- Manual port forwarding
- Use a bastion server
- View Cloudwatch alarms

NAT Gateways
- Hoghly available. NAT gateways in each availability zone are implemented with redundancy
- Suppoers brsts of up to 1-Gbps
- Managed by AWS
- Software is optimized for handling NAT traffic
- Port forwarding is not supported
- Bastion servers not supported
- Traffic metrics not supported

## 9.Understanding Elastic Bolck Store(EBS) and Elastic File System(EFS)
### 2 Instance Storage Types
####05:02
Cannot be attached to more than one instance at the same time  
Can be transferred between availbility zones  
EBS volume data is replicated across multiple servers in an availablity zone.

## Additional AWS Services
### 3. Partition Key

Use partition keys associated with each data record to determine which shard a given data record belongs to
