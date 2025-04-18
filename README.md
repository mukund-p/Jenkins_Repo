# Jenkins_Repo

This repository demonstrates the integration of a simple Java application with Jenkins for implementing Continuous Integration and Continuous Deployment (CI/CD). It includes:

- A sample Java app
- Maven configuration for build management
- A `Jenkinsfile` to automate the pipeline

---

## 📁 Project Structure

Jenkins_Repo/ <br>
├── src/ <br>
├── .gitignore  <br>
├── Jenkinsfile <br>
├── README.md <br>
└── pom.xml <br>

---

## 🚀 Prerequisites

Ensure the following tools are installed on your machine:

- Java Development Kit (JDK)
- Apache Maven
- Jenkins
- Git

---

## ⚙️ Setup Instructions

1. **Clone the Repository**

```bash
git clone https://github.com/mukund-p/Jenkins_Repo.git
cd Jenkins_Repo
```
2. **Build the Java Application**

- `mvn clean install` <br>
- Set Up Jenkins Job

3. **Open Jenkins and create a new Pipeline job.**

- Configure the job to pull this repository.
- Add the path to the `Jenkinsfile` in the pipeline definition (default is root).

4. **Run the Pipeline**

- Trigger the build manually OR
- Configure GitHub webhook for auto-builds on code pushes.

5. **🛠️ Troubleshooting**

- **Jenkins can't find Maven**: Ensure Maven is installed and configured in Jenkins under `Global Tool Configuration`.
- **Build fails due to missing JDK**: Make sure JDK is installed and added in Jenkins configuration.
- **Permission issues**: If Jenkins can't clone your repo, add GitHub credentials under `Credentials` in Jenkins.
