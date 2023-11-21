### What is CI-CD?
Continuous Integration & Continuous Delivery/Deployment
- CI - Source and Build - Developers commit code multiple times a day, fully auto with test process giving fast feedback
- CD (Delivery) - Source, Build, Test, Production - continued from CI, ensuring new changes are released to customers quickly and sustainable.
- CD (Deployment) - Source, Build, Test, Production - automates who process sp when all stages are passed, new changes are released automatically

The main difference between Continuous Delivery and Deployment is that with delivery, the production release is done manually

### Why use CI-CD?

- The main reason to use CICD, is to provide automation to the system which will provide fast releases, leading to cost efficiency.
- Faster software builds
- customer satisfaction
- fault isolations simpler and quicker (easy to find issues with code)

### What is jenkins?

- Jenkins is an open source automation server.
- Java-based program working with Windows, macOS, & Linux.

### Why use Jenkins?

- Open-Source
- Easy-to-use
- AWS, netflix, HMRC, Home Offic, NASA, use it. Even though they can afford any software, they go with Jenkins which is free (Key point - Open-Sourcew)

### What are the Stages to Jenkins?

1. Create a Jenkins Job
2. Build a Pipeline in Jenkins
3. Link the Jobs in Jenkins

### Alternatives to Jenkins

- **circleci** (only supports Linux and macOS)
- **Teamcity** (More supported OS) (On Prem only)
- **Bamboo** (one off payment)
- **GitLab**

They are provide more built-in features
None of these are open-source as well as you have to pay for build agent license price

What is it
Why use it
Business benefits
How you used it?
STAR Method

Research interviewers
Update Linkdlin

```Yaml
# Create a playbook to provision nginx web server in the web-node
---
# Yaml/yml file starts with three dashes
# where do you want to install or run this playboo
- hosts: web

# find the facts (see the logs) - optional
  gather_facts: yes

# provide admin access to this playbook - use sudo
  become: true

# provide the actual instructions - install nginx
  tasks:
  - name: provision/install/configure Nginx
    apt: pkg=nginx state=present

# ensure nginx is running/enable
```
```Yaml
# Create a playbook to provision installation of nodejs in the web-node
---
# Yaml/yml file starts with three dashes

# where do you want to install or run this playboo
- hosts: web

# find the facts (see the logs) - optional
  gather_facts: yes

# provide admin access to this playbook - use sudo
  become: true

# provide the actual instructions - install nginx
  tasks:
  - name: Find version 12 of nodejs
    shell: curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -

  - name: Install Nodejs
    apt: pkg=nodejs state=present

# ensure nginx is running/enable
```
