#  **<span style="color:green">Landmark Technologies.</span>**
### **<span style="color:green">Contacts: +1437 215 2483<br> WebSite : <http://mylandmarktech.com/></span>**
### **Email: mylandmarktech@gmail.com**

## Commonly ask questions and answers.
### 1. Who can study Landmark DevOps E. Degree Master Program?
+ Anyone who graduated from High School.
+ At least 18 year old


## ✅2)	I don't have an IT Background. Can I still do this course and succeed? 
+     Yes. We take you from zero IT background to become a highly skilled and Professional IT & DevOps Engineer.
+     Over 95% of our graduates working today had no prior IT background before joining.

``` sh
#!/bin/bash
# Use this script to install tomcat in rehat servers
echo delete the failed version of tomcat
sudo rm -rf /opt/tomcat9
echo assign a hostname to your server 
sudo hostname tomcat
# install Java JDK 1.8+ as a pre-requisit for tomcat to run.
cd /opt 
sudo yum install git wget -y
sudo yum install java-1.8.0-openjdk-devel -y
# Download tomcat software and extract it.
sudo yum install wget unzip -y

sudo wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.62/bin/apache-tomcat-9.0.62.tar.gz
sudo tar -xvf apache-tomcat-9.0.62.tar.gz
sudo rm apache-tomcat-9.0.62.tar.gz
sudo mv apache-tomcat-9.0.62 tomcat9
sudo chmod 777 -R /opt/tomcat9
sudo chown ec2-user -R /opt/tomcat9
sh /opt/tomcat9/bin/startup.sh
# create a soft link to start and stop tomcat
sudo ln -s /opt/tomcat9/bin/startup.sh /usr/bin/starttomcat
sudo ln -s /opt/tomcat9/bin/shutdown.sh /usr/bin/stoptomcat
sudo yum update -y
starttomcat
```
