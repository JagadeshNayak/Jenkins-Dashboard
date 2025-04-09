**Jenkins on AWS EC2 for GitHub and CI/CD pipelines :** Setting up Jenkins on an AWS EC2 instance to work with GitHub allows you to create a powerful and flexible continuous integration/continuous delivery (CI/CD) pipeline.
![A simple illustration showing the connection from AWS to Jenkins dashboard  The image should include](https://github.com/user-attachments/assets/bb3831fd-0322-483e-a37c-f56381231e68)
**Launching an EC2 instance** involves several key steps, whether you're using the AWS Management Console or the AWS Command Line Interface (CLI). Here's a breakdown of the process, with an emphasis on how to give your instance a specific name:

<img width="568" alt="Screenshot 2025-04-08 172023" src="https://github.com/user-attachments/assets/95a251b3-0aa0-4f12-97d1-cbdf6e242b4a" />

**Selecting OS** When selecting an operating system (OS) for your EC2 instance that will host Jenkins for GitHub CI/CD, there are a few excellent choices. Here's a breakdown, focusing on a strong recommendation:

<img width="600" alt="Screenshot 2025-04-08 172117" src="https://github.com/user-attachments/assets/fae71eed-8281-4a08-a7a2-11631ff38e6d" />

let's refine the security group rule for your EC2 instance to ensure it's both functional and secure. Here's a breakdown of the rule and some important considerations:
**Security Group Rules**
The Rule:
Type: Custom TCP
Port Range: 80-10000
Source: 0.0.0.0/0 (Anywhere)
**How to Implement in the AWS Console**:
Go to the EC2 service in the AWS Console.
Select "Security Groups."
Choose the security group associated with your EC2 instance.
Click "Edit inbound rules."
Add a new rule with the refined settings.

<img width="626" alt="Screenshot 2025-04-08 172234" src="https://github.com/user-attachments/assets/32424546-fa96-44e5-964f-b17304134337" />

**Launching Server**
Following the successful provisioning of your EC2 instance, the AWS Management Console provides a streamlined method for establishing a secure SSH connection. This process simplifies the connection procedure, minimizing potential errors and enhancing efficiency.

<img width="946" alt="Screenshot 2025-04-08 172317" src="https://github.com/user-attachments/assets/9d733e01-8fe7-4efa-9dc6-eb33f51ebb7e" />

After connecting to and launching the server, execute the commands provided in the text file one by one. Make sure to follow the sequence carefully. Each command plays a specific role in setting up the environment or deploying the application, so understanding their purpose is essential for a successful deployment.
After executing all commands you will get this dashboard by executing the instance IP Address in the browser like thsi **(18.204.217.91:8080)** .You will get the dashboard like below displayed image

<img width="922" alt="Screenshot 2025-04-08 172714" src="https://github.com/user-attachments/assets/0d66acba-0740-42d9-8ca4-be7c3f27e186" />

Copy the file path provided in the text file and paste it into the server terminal in the following format: sudo cat <path>. This command will display the password stored in that file. Once you retrieve the password from the server, copy it and paste it into the 'Administration Password' input field."

<img width="959" alt="Screenshot 2025-04-08 172803" src="https://github.com/user-attachments/assets/9103499b-686e-4ab1-8942-3d7b630808de" />

Install the suggested plugins that are suitable for our free-tier account and essential for basic usage. These plugins will help enhance functionality without exceeding the limitations of the free plan."

<img width="947" alt="Screenshot 2025-04-08 172828" src="https://github.com/user-attachments/assets/1554331b-3b13-4585-91f1-af589a75023c" />

After clicking on the INSTALL SUGGESTED PLUGINS you will get this dasnboard 

<img width="952" alt="Screenshot 2025-04-08 172855" src="https://github.com/user-attachments/assets/8b74e9f8-7b4e-4c28-866e-0c0b4ac5650d" />

"After completing the installation, you will need to provide the username, email ID, and password to create and configure a Jenkins account. This step is essential to proceed with setting up Jenkins for your project"

<img width="944" alt="Screenshot 2025-04-08 172950" src="https://github.com/user-attachments/assets/bf886b26-6a05-4a80-85b5-6c3fba572a56" />

After entering the username, email ID, and password, click on 'Save and Continue'. Once this step is completed, the Jenkins dashboard will appear, indicating that the setup has been success

<img width="959" alt="Screenshot 2025-04-08 173109" src="https://github.com/user-attachments/assets/40a1e2ea-1f6a-4f1f-8b29-721d42069821" />
fully configured."
Go to 'Create New Item' and create a new job for the Jenkins CI/CD pipeline."

<img width="959" alt="Screenshot 2025-04-08 173109" src="https://github.com/user-attachments/assets/0cf2936c-ce9d-481c-9782-204e0ba5c76f" />

Please provide the Groovy code for generating a Jenkins pipeline, including complete details of each stage and the required credentials."

<img width="951" alt="Screenshot 2025-04-09 214533" src="https://github.com/user-attachments/assets/1bfbfd97-8cab-45ef-bd1b-341cf5b1d557" />

After writing the Jenkins pipeline code, make sure to select the correct branch (main or master) from the repository link, and then proceed to build the job."

<img width="923" alt="image" src="https://github.com/user-attachments/assets/d408211a-6232-4c3f-8ec2-dacac1b79d13" />

After clicking on 'Build Now', Jenkins will display the build history and status under the job name. For example, if your pipeline job is named 'test', you will see the corresponding build entries. The image below shows how it appears in Jenkins."












