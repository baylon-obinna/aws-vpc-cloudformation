PREREQUISTE

 - Aws account(iam user with admin privilege)
   
 - Linux terminal
   
 - Aws-cli installed and configured on host machine
 
 STEPS
 
 - Login to Aws account
   
 - Search for cloudformation at the search bar
   
![image](https://github.com/baylon-obinna/aws-vpc-cloudformation/assets/111370498/85073591-64e1-4b42-8d18-183390d6c880)

 - Click on create stack
  
![image](https://github.com/baylon-obinna/aws-vpc-cloudformation/assets/111370498/8327d083-3af3-4a7d-b723-2d1d23767db7)

 - Click upload template, choose the file from your local device(download the template from the repo locally)
   
![image](https://github.com/baylon-obinna/aws-vpc-cloudformation/assets/111370498/3e1ae5ae-fb16-4876-a75d-9382fb4f4dac)

 - Provide metadata
   
![image](https://github.com/baylon-obinna/aws-vpc-cloudformation/assets/111370498/5c3fd4fd-20ee-4a1f-8186-b184e0879c3f)

 - Submit
   
![image](https://github.com/baylon-obinna/aws-vpc-cloudformation/assets/111370498/f05ec062-3e27-49de-9194-b579f3e0954b)

![image](https://github.com/baylon-obinna/aws-vpc-cloudformation/assets/111370498/4fe0746b-e809-47c1-bf80-d6c7c3a0ce23)

Either verify the resources created using the AWS user interface or AWS-CLI in the terminal, here i used AWS user interface.

![image](https://github.com/baylon-obinna/aws-vpc-cloudformation/assets/111370498/07b219b8-bd92-45a6-8188-d9243b7ab03d)

![image](https://github.com/baylon-obinna/aws-vpc-cloudformation/assets/111370498/61fcb0e5-2c1c-4e4a-9679-2e625563a5b2)

This virtual private cloud consists of 4 subnets private and public divided in twos each, two route table for the public and private subnets each, an internet gateway associated with the public subnets, Two NAT gateways for each of the public subnets, an autoscaling group with a desired state of two instances and maximum of four, a load balancer in the public subnet to route traffic into the instances in the private subnets, a security group in the private subnet for additional security to the instances, a bastion host to mask the ip addresses of the instances when accessing the internet.

![image](https://github.com/baylon-obinna/aws-vpc-cloudformation/assets/111370498/55a51dde-8d3e-4e24-97b8-478de075e709)






