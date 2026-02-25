# **Task #1**
## **Manually Create an EC2 Instance on AWS and Connect to it using SSH**
### Step 1: Create a folder **DevOps_Workshop** on desktop
### Step 2: Go to **AWS Management Console** and login as a **root user** and go to **Mumbai** region
### Step 3: Go the service **EC2**
### Step 4: Go to **Instances**
### Step 5: Click on **Launch instances**
### Step 6: Provide all the following details:
* _**Note:** Ensure the **region** in which you are creating the instance._
* **Name:** Instance1
* **OS:** Ubuntu
* **Instance Type:** t2.xlarge (4 vCPUs, 16 GB RAM)
* **Create key pair:** demo
* _**Note:** Keep .pem file securely in a folder (eg. DevOps_Workshop)_
* Create a security group by allowing SSH (22), HTTP (80) and HTTPS (443).
* Increase the storage from 8 GB to 16 GB if you want.
* _**Note:** Remember the storage as we will check this in Linux Command **df –h** in next_ task.
* Keep **number of instances** as 1.
* Click on **Launch instance**.
* You will see a **success message**.

### Step 7: Explore all the details of newly created EC2 instance
* Click on the **Instance ID** shown in success message.
* Make sure that the Instance1 is in **Running** state and **passed 2 checks**.
* Note down the **Private IP** and **Public IP**
* Look at **Instance type**
* Look at the **Elastic IP**
* Look at the **user name** of the instance
* Note down the **security group ID**
* Ensure the **inbound rules** and **outbound rules**
* Look at the **IAM role**
* Look at **VPC ID**
* Look at **Subnet ID**

### Step 8: Connect to the EC2 Instance
* Select the **Instance1**
* Click on **Connect** button
* Click on **SSH client** and copy the ssh command by clicking on the copy icon.
* _**Note:** Observe the syntax of **ssh** command as we will see it in Linux Commands in next task._
* Go to the folder where you saved your **.pem** file
* Right click and select **Open GitBash here**
* Paste the copied ssh command and hit Enter key
* Type **yes** when it prompts confirmation for connection
* Now you successfully connected your **local machine** to **remote EC2 instance**
* Obeserve **private IP** in terminal
