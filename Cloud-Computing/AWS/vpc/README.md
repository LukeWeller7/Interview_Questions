### Why use a VPC?

- A VPC allows you to secure your virtual networking environment, including your IP addresses, subnets and network gateways. You can also decide what virtual machines are internet facing or internal.

### How can I set up HA-SC on AWS?

- Auto-scaling group, setting up a cpu-usage threshold, load-balancer all to ensure HA

### What needs to be done with a VPC to ensure my database is secure

- Set up a private subnet (no connection to internet) have to be accessed via public subnet, extra security to not include ssh in nsg as well as only ip address to link being app.

### What are the disadvantages of ASG?

- Cost of running more instances
- Spike performance??

### Alternative monitoring system to ASG?

- CloudWatch Alarm, setting threshold condition such that you can be emailed when threshold is meet.

### What do we not need to configure in launch template for ASG?

- Leave the subnets as default so that the asg can provide HA by splitting the VM into different availability zones

### How can I assume some HA redundancies in VPC?

- Set up both the public and private subnets into different subnet/ availability zones to avoid redundancies.

### How can you set up your group size to provide HA in an ASG?

- Min, Max, Desire. Having at least 2 to ensure that more than one availability zone is covered. Avoid any fails or redundancies.

### How would you update the app vm in an ASG?

- Create a new launch template with the updated app, then in ASG, edit the launch template used. You can have different versions of the launch template.
- blue green deployment
- https://www.redhat.com/en/topics/devops/what-is-blue-green-deployment
- Blue green deployment is an application release model that gradually transfers user traffic from a previous version of an app or microservice to a nearly identical new release—both of which are running in production. 

### In a VPC, what takes care of internal routing.

- This is taken care by the internal router which uses the default routing table to navigate internally.

### How would you access the db on a 2tier VPC?

- Find a secure way to get the .pem file onto the app vm as well as the finding the db ip address

### Why would you want to set up a warmup time on alarm?

- During instance set up a higher cpu usage occurs so warmup timer avoids any alarms to go off during this.
