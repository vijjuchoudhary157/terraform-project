Successfully completed the task which was:

•	A working ALB DNS URL serving a web page 

•	EC2 instances running in private subnets 

•	Infrastructure is modular and reusable

here is the website link: 
http://my-alb-1650621584.us-east-1.elb.amazonaws.com/

and below are screen shots of tf apply and the site
<img width="1919" height="1141" alt="image" src="https://github.com/user-attachments/assets/9d8911bb-e552-4305-8e49-76f899228ff9" />
<img width="1919" height="1133" alt="image" src="https://github.com/user-attachments/assets/9ff83b89-adb2-499d-ad3e-0d65dba99efe" />
<img width="1618" height="1004" alt="image" src="https://github.com/user-attachments/assets/60d447ae-1e8e-4467-965e-ee407493e0ce" />



THANK YOU

AND below is my terminal code


module.ec2.aws_instance.my_instance2: Creating...
module.vpc.aws_route_table.public: Creation complete after 4s [id=rtb-0ce803460447499f4]
module.alb.aws_lb_target_group.my_tg: Creation complete after 7s [id=arn:aws:elasticloadbalancing:us-east-1:590183811932:targetgroup/my-target-group/19645f8cc023f0b4]
module.alb.aws_security_group.alb_sg: Creation complete after 8s [id=sg-04c63c72a6bcca7fe]
module.ec2.aws_security_group.ec2_security_group: Creating...
module.vpc.aws_subnet.public_subnet2: Still creating... [00m10s elapsed]
module.vpc.aws_subnet.public_subnet1: Still creating... [00m10s elapsed]
module.vpc.aws_subnet.public_subnet2: Creation complete after 14s [id=subnet-09438a31c10ace46e]
module.ec2.aws_security_group.ec2_security_group: Creation complete after 6s [id=sg-0ed9c159ea748247c]
module.vpc.aws_route_table_association.pub2: Creating...
module.ec2.aws_instance.my_instance1: Creating...
module.ec2.aws_instance.my_instance2: Still creating... [00m10s elapsed]
module.vpc.aws_subnet.public_subnet1: Creation complete after 16s [id=subnet-02b773cab892b132f]
module.vpc.aws_route_table_association.pub1: Creating...
module.vpc.aws_nat_gateway.my_nat_gateway: Creating...
module.alb.aws_lb.my_alb: Creating...
module.vpc.aws_route_table_association.pub2: Creation complete after 3s [id=rtbassoc-0b1b55aa970fedd79]
module.vpc.aws_route_table_association.pub1: Creation complete after 2s [id=rtbassoc-02e34254e5b74941b]
module.ec2.aws_instance.my_instance1: Still creating... [00m10s elapsed]
module.ec2.aws_instance.my_instance2: Still creating... [00m20s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [00m10s elapsed]
module.alb.aws_lb.my_alb: Still creating... [00m10s elapsed]
module.ec2.aws_instance.my_instance1: Still creating... [00m20s elapsed]
module.ec2.aws_instance.my_instance2: Still creating... [00m30s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [00m20s elapsed]
module.alb.aws_lb.my_alb: Still creating... [00m20s elapsed]
module.ec2.aws_instance.my_instance1: Still creating... [00m30s elapsed]
module.ec2.aws_instance.my_instance2: Still creating... [00m40s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [00m30s elapsed]
module.alb.aws_lb.my_alb: Still creating... [00m30s elapsed]
module.ec2.aws_instance.my_instance2: Creation complete after 44s [id=i-0f2e5130f1ccf6b84]
module.ec2.aws_instance.my_instance1: Creation complete after 40s [id=i-0a37e20bac46fee61]
aws_lb_target_group_attachment.attach_tg[1]: Creating...
aws_lb_target_group_attachment.attach_tg[0]: Creating...
aws_lb_target_group_attachment.attach_tg[1]: Creation complete after 0s [id=arn:aws:elasticloadbalancing:us-east-1:590183811932:targetgroup/my-target-group/19645f8cc023f0b4,i-0f2e5130f1ccf6b84,80]
aws_lb_target_group_attachment.attach_tg[0]: Creation complete after 1s [id=arn:aws:elasticloadbalancing:us-east-1:590183811932:targetgroup/my-target-group/19645f8cc023f0b4,i-0a37e20bac46fee61,80]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [00m40s elapsed]
module.alb.aws_lb.my_alb: Still creating... [00m40s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [00m50s elapsed]
module.alb.aws_lb.my_alb: Still creating... [00m50s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [01m00s elapsed]
module.alb.aws_lb.my_alb: Still creating... [01m00s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [01m10s elapsed]
module.alb.aws_lb.my_alb: Still creating... [01m10s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [01m20s elapsed]
module.alb.aws_lb.my_alb: Still creating... [01m20s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [01m30s elapsed]
module.alb.aws_lb.my_alb: Still creating... [01m30s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [01m40s elapsed]
module.alb.aws_lb.my_alb: Still creating... [01m40s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [01m50s elapsed]
module.alb.aws_lb.my_alb: Still creating... [01m50s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Still creating... [02m00s elapsed]
module.alb.aws_lb.my_alb: Still creating... [02m00s elapsed]
module.vpc.aws_nat_gateway.my_nat_gateway: Creation complete after 2m5s [id=nat-045616b35017a5b81]
module.vpc.aws_route_table.private: Creating...
module.vpc.aws_route_table.private: Creation complete after 4s [id=rtb-05e8e9c30ac8303e9]
module.vpc.aws_route_table_association.pri2: Creating...
module.vpc.aws_route_table_association.pri1: Creating...
module.alb.aws_lb.my_alb: Still creating... [02m10s elapsed]
module.vpc.aws_route_table_association.pri2: Creation complete after 2s [id=rtbassoc-01b99653e13265c0e]
module.vpc.aws_route_table_association.pri1: Creation complete after 3s [id=rtbassoc-01fbc06b225848dbb]
module.alb.aws_lb.my_alb: Still creating... [02m20s elapsed]
module.alb.aws_lb.my_alb: Still creating... [02m30s elapsed]
module.alb.aws_lb.my_alb: Creation complete after 2m34s [id=arn:aws:elasticloadbalancing:us-east-1:590183811932:loadbalancer/app/my-alb/cea31e9fec682d40]
module.alb.aws_lb_listener.listener: Creating...
module.alb.aws_lb_listener.listener: Creation complete after 4s [id=arn:aws:elasticloadbalancing:us-east-1:590183811932:listener/app/my-alb/cea31e9fec682d40/7e00117c6b1c3400]

Apply complete! Resources: 24 added, 0 changed, 0 destroyed.

Outputs:

alb_dns = "my-alb-1650621584.us-east-1.elb.amazonaws.com"
instance_ids = [
  "i-0a37e20bac46fee61",
  "i-0f2e5130f1ccf6b84",
]
private_subnet = [
  "subnet-071aafb43fcfdfc2d",
  "subnet-0d9485914d238efd9",
]
public_subnet = [
  "subnet-02b773cab892b132f",
  "subnet-09438a31c10ace46e",
]
vpc_id = "vpc-0828c891d526fad40"
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git add .
git : The term 'git' is not recognized as the name of a cmdlet, function, script file, or operable program. Check the spelling of the name, or if a path was 
included, verify that the path is correct and try again.
At line:1 char:1
+ git add .
+ ~~~
    + CategoryInfo          : ObjectNotFound: (git:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
 
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> 
 *  History restored 

PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git --version
git version 2.54.0.windows.1
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git init
Initialized empty Git repository in C:/Users/VIJENDRA CHOUDHARY/terraform-project/.git/
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git add .
warning: in the working copy of '.terraform.lock.hcl', LF will be replaced by CRLF the next time Git touches it
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git commit -m "Terraform modular infra setup (VPC, EC2, ALB)"
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'VIJENDRA CHOUDHARY@VijLAPTOP-BQUDN9NB.(none)')
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git config --global user.name "Vijendra Choudhary"
>> 
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git config --global user.name "Vijendra Choudhary"
>> git config --global user.email "vijjuchoudhary157@gmail.com" 
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git commit -m "Terraform modular infra setup (VPC, EC2, ALB)"
[master (root-commit) e412ffe] Terraform modular infra setup (VPC, EC2, ALB)
 14 files changed, 482 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 .terraform.lock.hcl
 create mode 100644 main.tf
 create mode 100644 modules/alb/main.tf
 create mode 100644 modules/alb/outputs.tf
 create mode 100644 modules/alb/variables.tf
 create mode 100644 modules/ec2/main.tf
 create mode 100644 modules/ec2/outputs.tf
 create mode 100644 modules/ec2/variables.tf
 create mode 100644 modules/vpc/main.tf
 create mode 100644 modules/vpc/outputs.tf
 create mode 100644 modules/vpc/variables.tf
 create mode 100644 outputs.tf
 create mode 100644 variables.tf
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git remote add origin https://github.com/vijjuchoudhary157/terraform-project.git
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git branch -M main
>> 
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> git push -u origin main
>> 
info: please complete authentication in your browser...
Enumerating objects: 20, done.
Counting objects: 100% (20/20), done.
Delta compression using up to 16 threads
Compressing objects: 100% (20/20), done.
Writing objects: 100% (20/20), 4.54 KiB | 775.00 KiB/s, done.
Total 20 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/vijjuchoudhary157/terraform-project.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\VIJENDRA CHOUDHARY\terraform-project> 
