# mc-vanilla-setup

# AWS CloudFormation Template

## Validate the template
```
aws cloudformation validate-template --template-body file://ec2-server-cft.yml
```

## Deploy the template
```
aws cloudformation deploy --template-file ec2-server-cft.yml --parameter-overrides SGUserIPAddress=YOUR_IP_HERE EC2KeyName=YOUR_KEY_PAIR_NAME_HERE SGVPCId=YOUR_VPC_ID_HERE ENIVPCSubnetId=YOUR_VPC_SUBNET_ID_HERE
```