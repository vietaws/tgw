

# VietAWS - AWS Transit Gateway Tutorials

## 1. Why AWS Transist Gateway?
	
	- Before Transit Gateway (Nov 26, 2018 [read more](https://aws.amazon.com/about-aws/whats-new/2018/11/introducing-aws-transit-gateway/) )
	ref: 

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
