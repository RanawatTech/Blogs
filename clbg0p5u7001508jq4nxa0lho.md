# Load Balancer on AWS

### How to create a Simple Application Load Balancer on AWS

### Pre-requisites: -

1.  Create 2 different instances where 2 different websites are hosted on that machine as shown in the image.  
    For Reference =[How to Host static Website on EC2](https://ranawattech.hashnode.dev/host-static-website-on-ec2)
    
2.  Create a Security Group (where inbound & outbound rules specify as per the needs)
    
3.  Create a Target Group (where 2 instances are allocated as per the requirement)
    

### Steps:-

1.  After Done With Pre-requisites Go to load Balancer Create A Load Balancer.
    
2.  While Creating Provide All the subnets that are available and provide security & target group.
    
3.  Once Done Create the Load Balancer & Verify whether the Load Balancer is handling 2 different machines or not.
    

### Pre-requisites: -

1.  Create 2 different instances where 2 different websites are hosted on that machine as shown in the image.
    

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb1.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb1.jpg)

2.  Create a Security Group (where inbound & outbound rules specify as per the needs)
    
3.  Create a Target Group (where 2 instances are allocated as per the requirement)
    

### Create a Security Group (with specific inbound/outbound rules)

Search Security Groups on your AWS Console.

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb2.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb2.jpg)

Now open security Groups and click on Create a New Security Group

Now give a name & description for your Security Group.

Specify the Inbound rule as HTTP and Source anywhere so your website is accessible globally.

Note: It's important to specify inbound rules as HTTP & Source anywhere.

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb3.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb3.jpg)

Now Click on Create a New Security Group

### Create a Target Group (where you specify instances for your load balancer)

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb4.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb4.jpg)

Search Target Groups on your AWS Console.

Now open Target Groups and click on Create a Target Group

Give a name for your target group and let all settings remain as it is.

For Settings Refer to the below image.

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb5.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb5.jpg)

Now click on next. After clicking Next choose the 2 Available instances and click on include as pending refer to the below Image.

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb6.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb6.jpg)

In review targets, you can see 2 instances as shown in the image now click on Create a Target Group.

Now you are ready to go to create a new application load balancer as your prerequisites are completed.

#### Create an Application Load Balancer (Which is our Main Goal)

Go to your EC2 dashboard and search for load balancing ec2.

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb7.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb7.jpg)

Now open Load Balancers and click on Create a Load Balancer, after that choose Application load balancer and click on create.

Give your Load Balancer Name. In Network, mapping selects all the subnets that are available as shown in the image. (Select all the available subnets)

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb8.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb8.jpg)

Now select your security group and target group which we created for the pre-requisites.

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb9.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb9.jpg)

Now click on Create Load Balancer.

Once your load balancer state is active you can use your load balancer

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb10.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb10.jpg)

Now open the website with the help of DNS Name copy that URL and open it in a new tab.

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb11.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb11.jpg)

In the Below Image you can see with 1 URL we can visit 2 different websites hosted on 2 different machines.

[![](https://github.com/GovindSingh9447/DevOps/raw/main/Exercises/Load_Balancer/Images/lb_ex01/lb12.jpg align="left")](https://github.com/GovindSingh9447/DevOps/blob/main/Exercises/Load_Balancer/Images/lb_ex01/lb12.jpg)