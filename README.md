# Jenkins Maven Demo 🚀

This project demonstrates how to set up a **Jenkins Freestyle job** to build a simple **Java Maven HelloWorld** application as part of a CI/CD pipeline.

---

## 🛠 Tools Used
- **Jenkins** (installed on AWS EC2)
- **Java JDK 11**
- **Apache Maven**
- **Git & GitHub**
- **Ubuntu EC2 Instance**


![jenkins](https://github.com/user-attachments/assets/f9149975-6e15-4ae9-b530-a7e2bb00361d)

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

📸 Added Screenshot: GitHub repo with committed files

![git](https://github.com/user-attachments/assets/d406f1dc-401e-4eba-943c-59e493fb2c96)

4. Configured Jenkins Freestyle Job
Created a Freestyle project in Jenkins named maven-build-demo.

Configured:

Git repo URL

Build step: mvn clean install

Built the job.


📸 Screenshot: Jenkins job config and build console output

![success](https://github.com/user-attachments/assets/dfcc32d2-2e9e-42f9-9d3d-8b1c7675058e)




✅ Outputs to Include
Jenkins Freestyle job name: maven-build-demo

Screenshot showing HelloWorld.java structure or contents

![hello world](https://github.com/user-attachments/assets/b7b8af88-fed6-4e0a-9751-ccf534febc3b)


![git push](https://github.com/user-attachments/assets/d9327274-70c9-4f60-8104-5ddb24151bc4)


💡 What You Learned
How to run Jenkins on an EC2 instance

How to set up and push a Maven Java app to GitHub

How to configure a Jenkins Freestyle job to build a Maven app

How to troubleshoot Jenkins errors like port conflicts, and Git push/pull issues

📎 Links
GitHub Repo: jenkins-maven-demo

👩‍💻 Author
kavya9864






