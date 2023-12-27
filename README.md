# Jenkins Begginers Tutorial

## Jenkins Installation on Ubuntu:

Jenkins Installation Guide : 

``` bash
https://www.jenkins.io/doc/book/installing/linux/
```
## prerequisites:
1. Java:
Jenkins requires Java to run. Ensure that you have Java Development Kit (JDK) installed

2. Web Browser : 
Jenkins is primarily accessed through a web browser. Ensure that you have a modern web browser installed, such as Google Chrome

3. Ports:
Jenkins runs on port 8080 by default. Ensure that this port is not being used by any other application, or configure Jenkins to use a different port if needed.

## Java Installation: 
```bash
sudo apt update 

sudo apt install openjdk-11-jdk  
```
## Jenkins Installation:

### 1. Download Jenkins GPG Key:
``` bash
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
```
### 2. Add Jenkins Repository Information:
``` bash
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
```

### 3. Update Package Lists:
``` bash
sudo apt-get update
```
### 4. Install jenkins:
``` bash
sudo apt-get install jenkins
```
# Check Jenkins Service Status:

### Current Status:
``` bash
sudo systemctl status jenkins
```
### To Start if Not Running:
``` bash
sudo systemctl status jenkins
```
### NOTE: In below image when we chcek the jenkins status & if its running , The initial Password is also Displayed:
![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/db00c9ae-579e-4757-9436-060e7b1c3c16)

### Enable Jenkins Service (to start on boot):
``` bash
sudo systemctl enable jenkins
```
# Access Jenkins in a Web Browser:
``` bash 
http://<public-ip>:8080
``` 
After Completing all the above steps , you should be able to access the jenkins Unlock page by going to the above URL in your web browser

![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/ab8964f1-0570-4ed8-bd5c-0d6f499e7fa2)

# Unlock Jenkins:
``` bash
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```
copy the password & Unlock the Jenkins
![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/80dda44a-3d41-42b4-b3db-06ed06953ecd)

# Customize Jenkins:
Install Suggested Plugins & wait for jenkins to download all the plugins:

![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/3e2b9558-5a78-40e6-af17-541d8a6be927)

# Enter Login Credentials:
NeedNot to enter Real Gmail-ID
![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/90f5822c-bafe-4168-b6d1-10e5b71320ad)

# Instance Configuration:
Save & Finish ! ---------> Start Using Jenkins.
![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/0a0b2cd4-f041-4463-9a9f-51871b96fe05)

# Jenkins UI:
Lets Explore Everything About Jenkins in Meanwhile: 
![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/f82c8ef5-d1e1-4fe8-8581-2076781bb790)

# Creating 1st Job In Jenkins:
### 1 . Click on Create job / New Item 

### 2 . Select FreeStyle Project 

![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/45f7a11c-37f5-4fe9-80dc-4bfd3053244b)

### 3 . Select Execeute Shell Section Under ADD BUILD STEP:
![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/11ab916e-f9c9-4c64-a41d-2cb11762715d)

### 4. Let's Write some basic shell commands & Build it:
apply & save !
![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/2fd84b91-e792-4c51-9874-f66f02833fa4)

### 5. Build The Project / JOb :
click on Build Now:
![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/aa670e0f-0ddf-4b7b-9fc0-e84d95f608ae)

![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/1be77013-3aa6-48e3-9ae7-3426b1cf51fa)

![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/9fa75e85-3b44-49ff-b12b-8dfc7006291e)

![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/781ef6fe-b138-41e2-8bcd-4900422c8b68)

![image](https://github.com/Sudhakar-09/Jenkins_Begginers_TutZ/assets/129831125/cecdc010-66c6-4104-a47f-eaaf430ebb26)
