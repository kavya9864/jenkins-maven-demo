# Jenkins Maven Demo 🚀

This project demonstrates how to set up a **Jenkins Freestyle job** to build a simple **Java Maven HelloWorld** application as part of a CI/CD pipeline.

---

## 🛠 Tools Used
- **Jenkins** (installed on AWS EC2)
- **Java JDK 11**
- **Apache Maven**
- **Git & GitHub**
- **Ubuntu EC2 Instance**

---

## 📁 Project Structure

jenkins-maven-demo/ ├── pom.xml ├── README.md └── src/ └── main/ └── java/ └── HelloWorld.java


---

## ✅ Steps Performed

### 1. Setup Jenkins on AWS EC2
- Created a new **Ubuntu EC2 instance** on AWS.
- Installed Java, Maven, and Jenkins manually (via `jenkins.war`).
- Ran Jenkins using:
  ```bash
  nohup java -jar jenkins.war > jenkins.log 2>&1 &


Accessed Jenkins via: http://<your-ec2-public-ip>:8080

📸 Screenshot: Jenkins welcome screen after initial setup

![jwp](https://github.com/user-attachments/assets/d344da52-f0f6-4adf-9917-82053355abcd)

2. Created Java Maven Project
Wrote a simple HelloWorld.java file under src/main/java/HelloWorld.java:
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello from Jenkins Maven Demo!");
    }
}

Created a pom.xml with basic Maven configuration to build the project.


3. Setup GitHub Repository
Repo name: jenkins-maven-demo

Added all project files:
git init
git remote add origin https://github.com/kavya9864/jenkins-maven-demo.git
git add .
git commit -m "Initial commit"
git pull origin main --allow-unrelated-histories
git push -u origin main

📸 Add Screenshot: GitHub repo with committed files
4. Configured Jenkins Freestyle Job
Created a Freestyle project in Jenkins named maven-build-demo.

Configured:

Git repo URL

Build step: mvn clean install

Built the job.


📸 Add Screenshot: Jenkins job config and build console output



✅ Outputs to Include
Jenkins Freestyle job name: maven-build-demo

Screenshot of successful Jenkins build

Screenshot of the GitHub repo with all files pushed

Screenshot showing HelloWorld.java structure or contents

Screenshot of Jenkins Console Output showing successful Maven build



💡 What You Learned
How to run Jenkins on an EC2 instance

How to set up and push a Maven Java app to GitHub

How to configure a Jenkins Freestyle job to build a Maven app

How to troubleshoot Jenkins errors like port conflicts, and Git push/pull issues

📎 Links
GitHub Repo: jenkins-maven-demo

👩‍💻 Author
kavya9864






