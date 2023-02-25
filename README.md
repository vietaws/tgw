

# VietAWS - AWS Transit Gateway Tutorials

## 1. Why AWS Transist Gateway?
	
- Without Transit Gateway 
	- VPC Peering
	- VPC Transit with IPSec
	- VPN per VPC to On-premises
- Transit Gateway Annoucement [Nov 26, 2018](https://aws.amazon.com/about-aws/whats-new/2018/11/introducing-aws-transit-gateway/)
- [Amazon VPC Quotas](https://docs.aws.amazon.com/vpc/latest/userguide/amazon-vpc-limits.html)


AWS TGW Highlights:

1. Number of attachements: 5,000
2. Peering attachments per transit gateway: 50
3. Transit gateways per VPC: 5
4. Maximum bandwidth per VPC attachment, DXG, Peering TGW: 50 Gbps
5. Maximum bandwidth per VPN tunnel: 1.25 Gbps


- [AWS Transit Gateway Quotas](https://docs.aws.amazon.com/vpc/latest/tgw/transit-gateway-quotas.html)
- [Transit Gateway Pricing](https://aws.amazon.com/transit-gateway/pricing/)

## 2. Architecture to Build (Multi-VPC, Cross-Region, Cross-Account)

	VPC:
		1. DEV VPC (US1 - Account1)
		2. TEST VPC (US1 - Account1)
		3. SHARE VPC (US1 - Account1)
		4. BRANCH VPC (US2 - Account1)
		5. CROSS VPC (US1 - Account2)
		6. EGRESS VPC (Singapore - Account1)
	Transit Gateway:
		1. TGW_US1
		2. TGW_US2
		3. TGW_SGN

### Build Scenerios:

	#1. Multi-VPC - Single Account - Single Region

	#2. Multi-VPC - Cross Account - Single Region

	#3. Multi-VPC - Single Account - Cross Region

	#4. Multi-VPC - Cross Account - Cross Region

## You also learn:
	1. Transit Gateway Single Route Table vs Multi Route Table
	2. Using AWS RAM (Resource Access Manager)
	3. Setup VPC, IGW, Amazon EC2, Security Group
