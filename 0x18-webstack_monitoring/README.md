# 0x18. Webstack monitoring

## Background Context
You cannot fix or improve what you cannot measure is a famous saying in the tech industry. In the age of the data-driven business, monitoring how our software systems are doing is an important thing. In this project, we will implement one of many tools to measure what is going on our servers.

Web stack monitoring can be broken down into 2 categories:
- Application monitoring: getting data about your running software and making sure it is behaving as expected
- Server monitoring: getting data about your virtual or physical server and making sure they are not overloaded (could be CPU, memory, disk or network overload)

## Learning Objectives
At the end of this project, you should be able to explain to anyone, without the help of Google:

### General
- Why is monitoring needed
- What are the 2 main area of monitoring
- What are access logs for a web server (such as Nginx)
- What are error logs for a web server (such as Nginx)

## Requirements
### General
- Allowed editors: vi, vim, emacs
- All your files will be interpreted on Ubuntu 16.04 LTS
- All your files should end with a new line
- A README.md file, at the root of the folder of the project, is mandatory
- All your Bash script files must be executable
- Your Bash script must pass Shellcheck (version 0.3.7) without any error
- The first line of all your Bash scripts should be exactly #!/usr/bin/env bash
- The second line of all your Bash scripts should be a comment explaining what the script is doing

## Tasks

### 0. Sign up for Datadog and install datadog-agent
**mandatory**

For this task head to https://www.datadoghq.com/ and sign up for a free Datadog account. When signing up, you'll have the option of selecting statistics from your current stack that Datadog can monitor for you. Once you have an account set up, follow the instructions given on the website to install the Datadog agent.

- Sign up for Datadog - Please make sure you are using the US website of Datadog (https://app.datadoghq.com)
- Use the US1 region
- Install datadog-agent on web-01
- Create an application key
- Copy-paste in your Intranet user profile your DataDog API key and your DataDog application key.
- Your server web-01 should be visible in Datadog under the host name XX-web-01

### 1. Monitor some metrics
**mandatory**

Among the litany of data your monitoring service can report to you are system metrics. You can have a lot of fun with these metrics, and they can give you a good sense of how busy or how healthy your machine is.

Set up some monitors within the Datadog dashboard to monitor and alert you when:
- System load is too high
- CPU usage is too high
- Memory usage is too high
- Disk usage is too high

### 2. Create a dashboard
**mandatory**

Now create a dashboard with different metric graphs:
- One graph per metric mentioned above
- Make sure that the graph shows the past hour
- Make sure that the graph shows the different metrics for your server
- Give each graph a proper title

## Author
- **Your Name** - Initial work

## Repository
- **GitHub repository:** holbertonschool-system_engineering-devops
- **Directory:** 0x18-webstack_monitoring
