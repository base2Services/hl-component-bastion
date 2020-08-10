![build-status](https://travis-ci.com/theonestack/hl-component-bastion.svg?branch=master)

### Cfhighlander bastion component

```bash

# install highlander gem
$ gem install cfhighlander 

# build and validate standalone component
$ cfhighlander cfcompile --validate bastion

```

### Requirements
VPC component

### Parameters

| Name            | Use                              | Default      | Global       | Type                | Allowed Values               | Required      
| -------------   | ---------------------------------|------------- |------------- |-------------------- |----------------------------- |----------- |
| EnvironmentName | Tagging                          | dev          | True         | String              |                              | Yes
| EnvironmentType | Tagging                          | development  | True         | String              | ['development','production'] | Yes
| Ami             | Bastion AMI                      |              | False        | AWS::EC2::Image::Id |                              | Yes
| SpotPrice       | Set the instance spot price      |              | False        | Integer             |                              | No
| InstanceType    | EC2 instance type                | t3.micro     | False        | String              |                              | Yes
| KeyName         | Bastion SSH key                  |              | False        | String              |                              | No
| DnsDomain       | Domain name to connect with      |              | False        | String              |                              | Yes
| SubnetIds       | Subnet(s) bastion will reside in |              | False        | CommaDelimitedList  |                              | Yes
| VPCId           | VPC bastion will reside in       |              | False        | AWS::EC2::VPC::Id   |                              | Yes
| AsgMin          | Autoscaling group minimum value  | 1            | False        | Int                 |                              | Yes
| AsgMax          | Autoscaling group minimum value  | 1            | False        | Int                 |                              | Yes
    

### Configuration options

TBD

### Outputs

TBD
