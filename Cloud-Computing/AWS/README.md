### What is EC2?

- AWS EC2 (Elastic Compute Cloud) is a web service that allows users to **rent virtual servers**, known as instances, in the cloud. It provides **scalable computing capacity**, enabling users to run applications, host websites, and process data without investing in physical hardware. EC2 offers flexibility, cost-effectiveness, and on-demand resource allocation.

### Why is it important to be on a certain regional database?

- Being on a regional database in AWS is crucial for **efficiency and reliability**. It reduces latency by storing data closer to users, ensuring **faster access**. It also enhances disaster recovery as data is replicated across availability zones within the region. In short, it boosts performance and safeguards data integrity.

### How do you create an instance?

- When you are on EC2, you can start by going to launch instance, in there you need to fill out the settings for the instance you want including name, AMI, key pair, security group, instance type, storage. You can check the instance summary before launching.

### What is a security group?

- A security group in AWS EC2 is like a virtual firewall that **controls inbound and outbound traffic** for your instances. Think of it as a set of rules that determine who can communicate with your EC2 instances. It acts as a protective barrier, allowing or blocking traffic based on your defined rules.

### What is a port?

- A port on AWS EC2 is like a door in a building. It's a **specific entry point** for network traffic to reach an EC2 instance. Think of it as each service having its own unique door number, allowing data to come in or go out. Ports enable communication and control between different software applications on the instance.

### What is a shell script?

- A shell script is a simple yet powerful tool used for automating tasks on a computer. Think of it as a series of instructions written in a language that the computer's operating system understands. It's like giving your computer a to-do list to perform tasks like file manipulation, program execution, and more, saving time and effort.

### What is an image?

- 

### How do you create your own AMI?

- 

### Why would businesses want to use an alarm?

- **Auto-scaling and monitoring**.

### How through EC2 can you run an App?

- Update && Upgrade, install nginx, git clone app folder, install nodejs, install pm2, run the app through pm2.

### How to connect db instance to app instance?

- In db instance, change the bindip to allow all ip access
- Environment Variable: export DB_HOST=mongodb://<app public ip>:27017/<db info folder>


