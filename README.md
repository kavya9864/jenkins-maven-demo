# jenkins-maven-demo
# Jenkins Maven Demo 🚀

A simple Java HelloWorld application built using Maven and integrated with Jenkins for CI/CD demonstration.


 This project is part of a hands-on exercise to set up Jenkins on an AWS EC2 instance and automate the build process using Freestyle jobs.

---

## 📁 Project Structure


jenkins-maven-demo/ ├── src/ │ └── main/ │ └── java/ │ └── HelloWorld.java ├── pom.xml └── README.md


---

## 🔧 Technologies Used

- Java 11  
- Apache Maven  
- Jenkins 2.440.1  
- AWS EC2 (Ubuntu)  
- Git & GitHub  
- MobaXterm (for SSH access)

![jenkins](https://github.com/user-attachments/assets/b66053a2-e8c4-4b04-ad11-9797dcfb286a)

---

## ⚙️ Jenkins Setup & Build Steps

1. **Launch Jenkins on AWS EC2**
   - Installed Jenkins via terminal
   - Opened Jenkins on `http://<ec2-ip>:8080`
     

2. **Install Required Jenkins Plugins**
   - Git Plugin  
   - Maven Integration Plugin

3. **Create a Freestyle Project**
   - Job Name: `maven-build-demo`
   - Source Code Management: Git
     - Repo: `https://github.com/kavya9864/jenkins-maven-demo.git`
   - Build Environment:
     - Maven build step: `clean install`

4. **Run the Build**
   - Triggered a manual build
   - Output: Successful Maven build

![success](https://github.com/user-attachments/assets/7cbfce9d-df10-4ef3-bcf0-002ace8c0fff)



![hello world](https://github.com/user-attachments/assets/b683113b-dd21-4b2b-9c31-84cd06e90b03)

---

## 📸 Recommended Screenshots

> Include these in your project repo or any presentation/doc:

1. ✅ Jenkins Freestyle Job Configuration screen  
2. ✅ Successful Jenkins Console Output (Build #)  
3. ✅ GitHub repository showing the project files  
4. ✅ EC2 instance terminal showing `git pull`, `git push`, and build logs  
5. ✅ `HelloWorld.java` output or structure  
6. ✅ Jenkins dashboard with build history for the project  

---

## 👋 Output

The expected build output in Jenkins should contain:



[INFO] Building jar: /path-to/target/hello-java-maven-1.0-SNAPSHOT.jar [INFO] BUILD SUCCESS


---

## 📌 Author

- GitHub: [@kavya9864](https://github.com/kavya9864)

---

## 🔗 Repo URL

[https://github.com/kavya9864/jenkins-maven-demo](https://github.com/kavya9864/jenkins-maven-demo)

