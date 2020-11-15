# task3
# #awscloud #awscli #aws #vimaldaga #righteducation #educationredefine #rightmentor #worldrecordholder #linuxworld #makingindiafutureready #righeudcation  #awsbylw #arthbylw
# ARTH-TASK-3 
# TASK WHICH WE WILL PERFORM:
# 1.Create a key pair.
# 2.Create a security group.
# 3.Launch an instance using the above created key pair and security group.
# 4.Create an EBS volume of 1 GB.
# 5.The final step is to attach the above created EBS volume to the instance created in the previous steps.


To use AWS CLI, we need to download and install "AWS CLI" on the top of Operating System. After install "AWS CLI" to check whether its successfully installed or not, use the command:


"aws --version" 



Here, we need to add the Access-key and Secret-key provided by AWS while creating this IAM User. Also, along with this we need to mention the default output format and the region. Here, region I am using is Mumbai i.e. ap-south-1.

![Capture1] (https://user-images.githubusercontent.com/69908356/95878879-560d5500-0d93-11eb-8de4-e7b104b12547.JPG)

So, now creating a keypair :
--key-name is an option to give a name to our key.

![Capture2](https://user-images.githubusercontent.com/69908356/95879197-b3a1a180-0d93-11eb-9f2a-cef5d2789347.JPG)

Now, we have our keypair ready and we can see that on the console too. 'taskkey' is created successfully.

![Capture3](https://user-images.githubusercontent.com/69908356/95879991-9caf7f00-0d94-11eb-865b-0f8fc7f0b2c5.JPG)

A security group acts as a virtual firewall for your instance to control inbound and outbound traffic. When you create a security group, you specify a friendly name of your choice. You can have a security group for use in EC2-Classic with the same name as a security group for use in a VPC. However, you can't have two security groups for use in EC2-Classic with the same name or two security groups for use in a VPC with the same name.Now, for creating a security group.

![Capture4](https://user-images.githubusercontent.com/69908356/95880380-13e51300-0d95-11eb-908e-f7d972fc7864.JPG)
![Capture5](https://user-images.githubusercontent.com/69908356/95880567-468f0b80-0d95-11eb-8f2e-176cb1316f3c.JPG)


Now, lets create an EC2 instance. This instance will have the keypair and security groups attached that we created just now.


![Capture6](https://user-images.githubusercontent.com/69908356/95880743-78a06d80-0d95-11eb-932c-65818b292b0d.JPG)


Our instance is now launched in ap-south-1a.

![Capture7](https://user-images.githubusercontent.com/69908356/95880938-aab1cf80-0d95-11eb-837a-0fd02793e306.JPG)


Now, we will create a 1 GB Volume using EBS. EBS comes under the EC2 service of AWS.The volume type will be general purpose SSD Volume:


![Capture8](https://user-images.githubusercontent.com/69908356/95881089-d3d26000-0d95-11eb-94c0-8d3981bcebe6.JPG)


Our EBS volume is now created and ready. This volume we need to attach to the EC2 instance we have created earlier.

![Capture9](https://user-images.githubusercontent.com/69908356/95881223-fe241d80-0d95-11eb-882e-a5b430e7248c.JPG)

Our volume is now successfully attached and we can see that in the Console of AWS:

![Capture10](https://user-images.githubusercontent.com/69908356/95881387-2875db00-0d96-11eb-86da-bd7d2374d4ba.JPG)
![Capture11](https://user-images.githubusercontent.com/69908356/95881532-4fcca800-0d96-11eb-8c20-7a3e47c3f9fd.JPG)
