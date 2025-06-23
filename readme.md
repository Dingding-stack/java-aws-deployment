![Tomcat Started](screenshots/4_tomcat_started.png)


# Java Web Application Deployment on AWS

> The `ROOT.war` package was provided as part of a DevOps training project. I was fully responsible for independently deploying, configuring, and troubleshooting the application on AWS.

## 🔧 Deployment Stack

- **Cloud**: AWS EC2 (Ubuntu 20.04)
- **App Server**: Apache Tomcat 9
- **Database**: MySQL 8
- **WAR File**: `ROOT.war` (given, not developed by me)
- The web app was successfully deployed and tested on two AWS EC2 instances (Node 1 and Node 2). For security reasons, public IP addresses are not included.

## 💡 Skills Practiced

- SSH remote login and Ubuntu system management
- MySQL root password reset and connection testing
- Apache Tomcat installation and configuration
- WAR deployment and resolving 404 errors
- AWS EC2 security group setup for port 8080

## 🚀 Deployment Steps

1. Launched EC2 Ubuntu instance
2. Installed Java, MySQL, and Tomcat
3. Uploaded and deployed `ROOT.war` to `/webapps`
4. Opened port 8080 in security group
5. Restarted Tomcat and verified service

## 🗼 Key Screenshots

✅ **1. MySQL Root Password Reset**
 This screenshot shows the process of resetting the MySQL root password using the `ALTER USER` command followed by `FLUSH PRIVILEGES;`. It confirms the password change was successful without any errors.

------

✅ **2. WAR Upload to Tomcat**
 This image displays the step where the `ROOT.war` file is uploaded to the Apache Tomcat server's `webapps` directory. This file will replace the default root application.

------

✅ **3. EC2 Security Group Port Configuration**
 This screenshot shows the AWS EC2 security group settings where port 8080 (custom TCP) is opened to `0.0.0.0/0`, allowing public access to the Tomcat web server.

------

✅ **4. Translated Blogging Platform Web Interface**
 This is the translated English version of the deployed blogging platform. The interface includes tabs for “Articles” and “Q&A”, and a message indicating that no content is available yet.

------

✅ **5. Tomcat Login Page Display**
 This image confirms that the Tomcat-deployed application is working. It shows a running login page with a functional UI, accessible via the specified public IP and port 8080.



## 📁 Repository Structure

```
java-deployment-demo/
├── screenshots/           # All screenshots used in this README
├── ROOT.war               # The Java WAR file 
└── README.md              # Project explanation (this file)
```

## 📍 Notes

This project helps demonstrate my ability to deploy and troubleshoot cloud-based web apps, useful for IT Support or DevOps entry-level roles.
