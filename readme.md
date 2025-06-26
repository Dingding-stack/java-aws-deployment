![Tomcat Started](screenshots/4_tomcat_started.png)


# Java Web App Deployment on AWS (Tomcat + MySQL + Nginx + Alarm)

This project was completed as part of a DevOps foundation course. The goal was to practice deploying and troubleshooting a full-stack Java web application on AWS EC2 instances.

---

## 🚀 Deployment Stack

- **Cloud Provider**: AWS EC2 (Ubuntu 20.04)
- **Application Server**: Apache Tomcat 9
- **Database**: MySQL 8
- **Reverse Proxy**: Nginx on second EC2 instance
- **Monitoring**: Alarm endpoint simulated for CPU usage >80%
- **Artifact**: Prebuilt `ROOT.war` Java package

---

## 💡 Key Skills Practiced

- Remote server setup and SSH access  
- MySQL installation, root password reset, and service check  
- Tomcat deployment and 404 error troubleshooting  
- AWS security group configuration for port exposure  
- Nginx installation and multi-instance load access  
- Alarm endpoint simulation and status verification  
- Linux system troubleshooting and service management  

---

## 📋 Deployment Steps

1. Launch two AWS EC2 Ubuntu instances (Node 1 & Node 2)
2. Install Java, MySQL, and Tomcat on Node 1
3. Deploy `ROOT.war` to Tomcat’s `/webapps` directory
4. Open port 8080 in AWS security group for Node 1
5. Restart Tomcat, verify the application loads correctly
6. Install Nginx on Node 2 to proxy or redirect HTTP traffic
7. Simulate alarm endpoint for CPU status visualization

   
## 🗼 Key Screenshots

✅ **1. MySQL Root Password Reset**  
This screenshot shows the process of resetting the MySQL root password using the `ALTER USER` command followed by `FLUSH PRIVILEGES;`.  
![1_mysql_login](screenshots/1_mysql_login.png)

✅ **2. WAR Upload to Tomcat**  
This step shows the `ROOT.war` file being uploaded to the `webapps` directory of Tomcat to replace the default root application.  
![2_upload_root_war](screenshots/2_upload_root_war.png)

✅ **3. EC2 Security Group Port Configuration**  
Port 8080 (TCP) was opened to `0.0.0.0/0` via AWS security group to allow external access.  
![3_ec2_port_8080](screenshots/3_ec2_port_8080.png)

✅ **4. Tomcat Started Successfully**  
Tomcat was restarted to deploy the WAR file, confirmed by the console output.  
![4_tomcat_started](screenshots/4_tomcat_started.png)

✅ **5. Tomcat Login Page Display**  
Successfully loaded the web app on browser using EC2 public IP and port 8080.  
![5_login_page](screenshots/5_login_page.png)

✅ **6. Architecture Diagram**  
This diagram outlines the complete setup:
- EC2 instance with Apache Tomcat + MySQL  
- Deployed WAR application  
- Port 8080 open for HTTP access  
- Separate EC2 instance running Nginx  
- End-user accesses via browser  
![6_architecture Diagram](screenshots/6_architecture Diagram.png)

✅ **7. Translated Blogging Platform Web Interface**  
English-translated UI for the blogging platform showing an empty post list and Q&A tabs.  
![nginx1](screenshots/nginx1.png)

✅ **8. Nginx Welcome Page on Node 2**  
Nginx default page confirms HTTP service running on second EC2 instance.  
![nginx2](screenshots/nginx2.png)

✅ **9. Alarm Status Page (Custom Endpoint Test)**  
Simulated alarm endpoint was tested for accessibility and frontend status display.  
![alarm](screenshots/alarm.png)

---

📁 📁 Repository Structure java-aws-deployment/

screenshots/ (all screenshots used in this README)

1_mysql_login.png

2_upload_root_war.png

3_ec2_port_8080.png

4_tomcat_started.png

5_login_page.png

6_architecture_Diagram.png

7_nginx1.png

8_nginx2.png

9_alarm.png

ROOT.war (the Java WAR file)

README.md (project explanation file)




This project helped me:

- Reinforce my understanding of full-stack web deployment on Linux servers  
- Gain hands-on experience with cloud service setup, port access, and troubleshooting  
- Document and present technical work clearly using GitHub best practices  

---

## ✅ Next Steps

- Automate the deployment with shell scripts  
- Create a Dockerized version of the app  
- Add system monitoring using AWS CloudWatch or Prometheus  



