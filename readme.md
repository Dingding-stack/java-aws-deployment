# Java Web Application Deployment on AWS

> The `ROOT.war` package was provided as part of a DevOps training project. I was fully responsible for independently deploying, configuring, and troubleshooting the application on AWS.

## 🔧 Deployment Stack

- **Cloud**: AWS EC2 (Ubuntu 20.04)
- **App Server**: Apache Tomcat 9
- **Database**: MySQL 8
- **WAR File**: `ROOT.war` (given, not developed by me)

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

### ✅ MySQL Login (after password reset)



### ✅ WAR Upload to Tomcat



### ✅ Open Port 8080 in AWS Security Group



### ✅ Tomcat Started Successfully



### ✅ Web Interface (Chinese)

> > Final Deployed Web Interface (UI in Chinese)
> >  ⚠️ Please note that the application frontend is in Chinese. It was provided as part of the training package and was not developed by me. The deployment environment, however, was fully built and managed in English (Ubuntu, MySQL, Tomcat on AWS).



## 📁 Repository Structure

```
java-deployment-demo/
├── screenshots/           # All screenshots used in this README
├── ROOT.war               # The Java WAR file 
└── README.md              # Project explanation (this file)
```

## 📍 Notes

This project helps demonstrate my ability to deploy and troubleshoot cloud-based web apps, useful for IT Support or DevOps entry-level roles.