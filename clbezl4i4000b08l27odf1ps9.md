# AWS - IAM User

## Problem Statement

### Create an Admin user with IAM

Create a User with the Following Configurations

*   Must have Custom Password & Required password reset checkbox as unselect
    
*   Add `Administrator Access` Policy
    
*   Create a Tag as `key=role` & `value=tester`
    
*   Try to log in with that newly created admin user
    

## Create an Admin User with IAM (AWS)

Go to AWS Console search For IAM and open the Service

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670497916039/CsqNsPeK2.jpg align="center")

After that click on Users, select Add Users

Now give the username for that User

In AWS Credential Type Select Password- AWS Management Console Access

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670497978664/f9CG3eRO7.jpg align="center")

Use Custom Password & Unselect checkbox for the required password reset

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670498104245/8_FT-e7q4.jpg align="center")

After that Click on Next

Now in Set Permissions select Attach Existing Policies Directly

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670498115244/IvF1oVULs.jpg align="center")

In Policies select `Administrator Access`

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670498151546/4V3U4gEUO.jpg align="center")

Click on Next Tags

We are using tags as keys (`role`)=Value(`tester`), You can give anything as per your needs

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670498190028/qOsQ4BCsX.jpg align="center")

After that Click on Next & Click on Create User

Your IAM Admin User is Successfully Created

To access the user, go to IAM & then users click on your username

Go to security Credentials & Console-sign in link Given in the summary

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1670498226817/gAXQkIWmI.jpg align="center")

Enter your Username & Password & click on Sign in.

Now you can use your IAM user with all Access except Billing Dashboard.

Note: - It is very necessary to not use your root user account for any services, the best practices always suggest creating a new user admin user by Admin.