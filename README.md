# Jenkins Begginers Tutorial

## Jenkins Installation on Ubuntu:

Jenkins Installation Guide : 
https://www.jenkins.io/doc/book/installing/linux/

## prerequisites:
1. Java:
Jenkins requires Java to run. Ensure that you have Java Development Kit (JDK) installed

2. Web Browser : 
Jenkins is primarily accessed through a web browser. Ensure that you have a modern web browser installed, such as Google Chrome

3. Ports:
Jenkins runs on port 8080 by default. Ensure that this port is not being used by any other application, or configure Jenkins to use a different port if needed.

## Java Installation: 
sudo apt update 

sudo apt install openjdk-11-jdk  

## Jenkins Installation:

### 1. Download Jenkins GPG Key:
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key

### 2. Add Jenkins Repository Information:
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null

### 3. Update Package Lists:
sudo apt-get update

### 4. Install jenkins:
sudo apt-get install jenkins

# Check Jenkins Service Status:

### Current Status:
sudo systemctl status jenkins
### To Start if Not Running:
sudo systemctl status jenkins
### Enable Jenkins Service (to start on boot):
sudo systemctl enable jenkins

# Access Jenkins in a Web Browser:
http://<public-ip>:8080

After Completing all the above steps , you should be able to access the jenkins Unlock page by going to the above URL in your web browser
