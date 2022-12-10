# Host Static Website on EC2

## Problem Statement

### Host A Static Website on EC2

1.  Create an EC2 Machine with OS as Linux Amazon Linux 2
    
2.  After Creating the instance Install the Apache Server and start the Apache service also make it a startup service so it can automatically start at the startup
    
3.  Now change the Content of `index.html` in directory `var/www/html/` to `Hello World`
    

**Solutions**

Launch an EC2 instance by login into your AWS Account we are using Amazon Linux 2

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670499200946/-RehMERJC.jpg align="center")

Create a new key pair to connect to your instance.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670499144726/QcFJvXJwI.jpg align="center")

Allow HTTP Traffic for your instance by enabling the checkbox.

Note: - Without HTTP Access your website is not accessible globally.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670499249793/BXhR0V8HiA.jpg align="center")

Now Connect to your Instance.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670499265740/NBeT3EzPs.jpg align="center")

Now the most important steps.

Install the Apache Server By using Below Command

```plaintext
yum install –y httpd
```

Now start the Apache service by using below command

```plaintext
systemctl start httpd
```

Now to run Apache Service automatically at startup use the below command

```plaintext
systemctl enable httpd
```

Now to put your html code to the file use below command

```plaintext
echo “<h1>Hello World</h1>” /var/www/html/index.html
```

Now Access your website with the public IPV4 address.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670499349148/S9406MBri.jpg align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670499368492/Yv_eiwdps.jpg align="center")