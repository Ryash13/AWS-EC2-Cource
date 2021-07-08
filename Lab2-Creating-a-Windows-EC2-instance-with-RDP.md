### Lab02 Creating a new Windows EC2 instance and login with RDP (Remote Desktop Protocol)

- Login to AWS Console
- From the top Navigation Bar Click Services
- Select EC2 service
- Click on Launch Instance
- Choose Windows 2016 Server Base AMI
- Choose EC2 instance type of t2.micro
- Configure Instance Details
    There are various configuration we can make but for this lab we will leave the configuration as default.
    NOTE: Network and Subnet is important configuration and Default subnet will be of any availability zone

- Click on Next: Add Storage => There we can set the Size of the GiB storage we want in our Volume(Leave it as default)
- Click on Next: Add Tags
    You can add various tags and its respective value in the EC2 instance (Atleast add a name tag)

- Click on Next: Configure Security Group
    Either you can choose an existing Security group or you can create a new Security Group from scratch

- Click on Review and Launch
- Create a Key Pair, Download it in your local machine, Check the Acknoledge box and Launch Instance

Your Instance will launch now.

- You will be able to see the InstanceID, Click on that
- Select the Instance and click on Connect

- Now you will see two connection options 
    1) Session Manager
    2) RDP Client
- Click on RDP Client

- You will see a button with label "GET PASSWORD"
- Click on that and will ask you to upload your Key i.e. .pem file
- After that click on Decrypt Password
- A Password will be visible to you, Copy that password and Click on Download Remote Desktop File

For Windows User Only

- RDP Will Run a Remote Windows EC2 Instance and will ask for UserName and Password
- UserName = "ADMINISTRATOR" and Password = "Copied String"
- Click enter and your Remote access of that Windows EC2 Instance will run