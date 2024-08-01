# Migrating-an-EC2-Instance-from-one-region-to-another-AWS-Articles

EC2 (Elastic Compute Cloud) is a service provided by Amazon Web Services which lets you set up your own virtual servers. AWS has several data centers across the globe where these services are provided which they call “Region”. Every region is isolated from other regions and their services too. In this article, we will explore how we can migrate an EC2 Instance from one region to another region.

I have already created an EC2 Instance in the ap-south-1 (Mumbai) region and I will migrate it to the ap-southeast-1 (Singapore) region.

![image](https://github.com/user-attachments/assets/3189dabc-f289-468f-821b-3cf35da1ccc6).


## To migrate the EC2 Instance just follow these steps :
1. Create an image of your existing instance. Click on the “Actions” button, then select “Image” and then click on the “Create Image” option.

![image](https://github.com/user-attachments/assets/edc2bdc5-68c0-42cf-8aab-d13925bd14e1)

2. Create an image of the EC2 Instance. Enter a suitable name and description for the image, if you don’t want to reboot your existing instance during the creation of the image just check the “No Reboot” option and then click on “Create Image” option.
  ![image](https://github.com/user-attachments/assets/924b18b7-d196-42c2-b8ad-ec8cefc81c15)

3. Once your image is created you need to copy the ami (image) to the destination region. Select your ami (image), click on “Actions” and then select “Copy AMI”.

  ![image](https://github.com/user-attachments/assets/f453a342-f9fa-4c71-ab26-547ff487e7ce)

  ![image](https://github.com/user-attachments/assets/21ce1405-f68d-4d0b-b892-957e0d027099)

4. Select the destination region, give a suitable name and description for the image and then click on “Copy AMI”.

   ![image](https://github.com/user-attachments/assets/393b30ab-54a7-4683-a5f3-094c6abe9ddf)

5. Now, go to the destination region and wait until your ami (image) gets created. Now, launch your EC2 Instance using the ami (image) you copied.
   
![image](https://github.com/user-attachments/assets/f2cf6bbd-7df8-4707-8ad5-a248a97d3e33)

You have successfully migrated your EC2 instance from one region to another. You can terminate your EC2 instance in the other region if you don’t want to run it anymore.

Thank You 😊
   






