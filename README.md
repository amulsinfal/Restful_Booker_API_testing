# 🧪 Restful Booker API Testing with Postman

This project demonstrates comprehensive API testing of the [Restful Booker API](https://restful-booker.herokuapp.com/apidoc/index.html) using **Postman**, **Newman**, and **Jenkins** for CI/CD automation. It covers end-to-end test cases including authentication, booking operations, and response validation—ideal for showcasing API testing skills.

---

## 📁 Project Structure
1. Collection File: Restful_Booker_API_testing/Restful-booker-api-testing/Restful_Booker_API_testing.postman_collection.json  
[Restful_Booker_API_testing.postman_collection.json](https://github.com/amulsinfal/Restful_Booker_API_testing/blob/main/Restful-booker-api-testing/Restful_Booker_API_testing.postman_collection.json)  <br>

2. Environment variables file: Restful_Booker_API_testing/Restful-booker-api-testing/env-qa.postman_environment.json  
[env-qa.postman_environment.json](https://github.com/amulsinfal/Restful_Booker_API_testing/blob/main/Restful-booker-api-testing/env-qa.postman_environment.json)  <br>

3. Test Results: Restful_Booker_API_testing/Restful-booker-api-testing/TestResults/newman/  
[Test Reports](https://github.com/amulsinfal/Restful_Booker_API_testing/tree/main/Restful-booker-api-testing/TestResults/newman)  <br>
<img width="1200" alt="" src="https://github.com/user-attachments/assets/9f86a209-c143-4915-a999-a964fa39bb1d" />
---

## ✅ Key Features

- 🔐 Token-based authentication testing
- 📝 Create, update, get, and delete booking test cases
- ❌ Positive, Negative and E2E test scenarios
- ♻️ Data-driven testing using environment variables
- 🧾 Automated assertions with `pm.test` and `pm.expect`
- 📊 Newman CLI for command-line execution and reporting
- ⚙️ Jenkins

---

## 🛠️ Tools & Technologies

- Postman
- Newman
- Jenkins
- JavaScript (Postman Tests)
- HTML Reporting

---

## ▶️ How to Use This Project

### 1. 📥 Import into Postman
- Import `Restful-booker-api-testing/Restful_Booker_API_testing.postman_collection.json`
- Import `Restful-booker-api-testing/env-qa.postman_environment.json`

### 2. 🧪 Run in Postman
Use the **Collection Runner** to execute all test cases and view results.

---

## 🖥️ Run via Newman (CLI)

### Run test collection
1. Go to the **Restful-booker-api-testing** folder  <br>
2. Run the following command:
```
newman run Restful_Booker_API_testing.postman_collection.json -r htmlextra --reporter-html-title "Restful Booker API Execution Report"
```

---

## 🔄 Jenkins CI/CD Integration
This project supports API test automation using Jenkins via a Freestyle Project, which integrates Postman tests using Newman CLI.

✅ Steps to Integrate with Jenkins:

Create Jenkins Freestyle Project:
- Project Type: Freestyle
- Build Step: Execute Windows Batch Command
- Batch Script (Windows):
  ```
  newman run "C:\Software_Testing\Automation_Testing\Postman\Restful-booker-api-testing\Restful_Booker_API_testing.postman_collection.json" --folder "E2E API Automation" -r htmlextra --reporter-htmlextra-title "Restful Booker Api Execution Report"
  ```

  <img width="1920" height="1032" alt="" src="https://github.com/user-attachments/assets/e9306349-7e61-4bfd-a1e6-3879e725a05a" />  <br>
  <img width="1920" height="1032" alt="" src="https://github.com/user-attachments/assets/4595474f-e862-45cd-a1d6-490b835f51f5" />  <br>
  <img width="1920" height="1032" alt="" src="https://github.com/user-attachments/assets/bca8f777-2523-4413-a51b-bc809b0888fe" />  <br>
  <img width="1920" height="1032" alt="" src="https://github.com/user-attachments/assets/a3c3a899-23c2-4286-ac94-5c4723285e68" />  <br>

---

### Screenshots 

<img width="1920" height="1080" alt="" src="https://github.com/user-attachments/assets/598c62f2-2dcd-4437-a357-f3caf6d38ac9" />  <br>
<img width="413" height="907" alt="" src="https://github.com/user-attachments/assets/b459f1dd-d2dd-432c-a81c-d29b67d66654" />  <br>  
<img width="410" height="324" alt="" src="https://github.com/user-attachments/assets/f1e0092b-11a3-4466-b512-f15dc164d763" />  <br>  
<img width="411" height="321" alt="" src="https://github.com/user-attachments/assets/e26a3cc3-67bb-4f97-9e46-73e8c88a53bf" />  <br>  



