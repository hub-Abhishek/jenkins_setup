# jenkins_setup

What is Continuous integration?
In the past, developers on a team might work in isolation for an extended period of time and only merge their changes to the master branch once their work was completed. This made merging code changes difficult and time-consuming, and also resulted in bugs accumulating for a long time without correction. These factors made it harder to deliver updates to customers quickly (Source - aws - https://aws.amazon.com/devops/continuous-integration/)


Creating an EC2 instance for For jenkins server - 
1. Log in to EC2 instance - https://us-east-1.console.aws.amazon.com/ec2/v2/
2. Select Launch Instance. Proceed adding with the following configurations - 
    Kernel selection - select Amazon Linux 2 AMI (HVM) - Kernel 4.14, SSD Volume Type
    Instance type - t2.micro
    No changes in instance details
    No changes in storage required
    Add tags - Key: Name; Value: Jenkins_Server
    New Security Group with Security Group name - Jenkins_Server. Add New Rule with Custom TCP. Port Range MUST BE 8080 (Jenkins always defaults to 8080)
3. Review and launch - Create a new pair, save the file

Connecting to EC2 instance - 
You can either connect via your browser (Select the instance > Actions > Connect > Connect), or you can use a software like Putty or MobaXterm ( https://mobaxterm.mobatek.net/download-home-edition.html)
For connecting via external softwares, copy the ip address of the ec2 instance, 