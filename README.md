# 📌 Automated API Testing with Postman & Newman

## 📖 **Project Overview**
This project demonstrates **API test automation** using **Postman** for test case design and **Newman** for execution. Additionally, it integrates with **Jenkins** to automate the testing process in a CI/CD pipeline.

---

## 🛠 **Technologies Used**
✅ **Postman** - API testing tool for designing test cases.
✅ **Newman** - Command-line runner for executing Postman collections.
✅ **Newman Reporter HTML Extra** - Generates detailed HTML reports.
✅ **Jenkins** - Automates test execution in a CI/CD environment.
✅ **GitHub** - Version control system for managing test collections.

---

## 🚀 **Project Features**
🔹 **Create & Export API Test Cases in Postman** - Design and export collections as `.postman_collection.json`.
🔹 **Execute Tests via Newman** - Run tests from the command line.
🔹 **Generate HTML Reports** - Store execution results in an easy-to-read format.
🔹 **Automate Execution with Jenkins** - Schedule and execute tests in a pipeline.

---

## 📂 **Project Structure**
```
AutomatedAPITesting/
│── collections/
│   ├── MyCollection.postman_collection.json
│   ├── MyEnvironment.postman_environment.json (optional)
│── reports/
│   ├── newman-report.html
│── scripts/
│   ├── run_tests.sh (Linux/Mac)
│   ├── run_tests.bat (Windows)
│── README.md
```

---

## ⚙️ **How to Use This Project**

### 1️⃣ **Clone the Repository**
```sh
git clone https://github.com/DevelUps/AutomatedAPITesting.git
cd AutomatedAPITesting
```

### 2️⃣ **Install Dependencies**
Ensure **Node.js** and **Newman** are installed:
```sh
npm install -g newman newman-reporter-htmlextra
```

### 3️⃣ **Run API Tests with Newman**
```sh
newman run collections/MyCollection.postman_collection.json -r htmlextra
```
After execution, an HTML report will be generated in the `reports/` folder.

### 4️⃣ **Automate Tests in Jenkins**
- Configure a Jenkins **Freestyle Project**.
- Add a **Build Step** to execute the following command:
  ```sh
  newman run collections/MyCollection.postman_collection.json -r htmlextra
  ```
- Set up post-build actions to display the report.

---

## 📌 **Contributing**
If you would like to contribute, fork the repository and submit a pull request with improvements!

---

## 🔗 **License**
This project is licensed under the MIT License. Feel free to use and modify it.

🚀 **Happy Testing!**

