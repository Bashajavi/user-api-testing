# 🧪 User Management API - Basic Auth (Automated Testing)

This project automates API testing for a **User Management System** using **Postman** and **Newman CLI**, including **Basic Authentication**, **random test data**, **negative testing**, and **CI/CD integration** via **GitHub Actions** and **Jenkins**.

---

## 🚀 Features

- ✅ **Basic Authentication** for secure API access  
- 🔁 **Dynamic Test Data** — generates random usernames and IDs  
- ❌ **Negative Testing** for:
  - Invalid credentials  
  - Missing required fields  
- 🧾 **HTML Reports** via Newman CLI  
- ⚙️ **CI/CD Integration** using:
  - GitHub Actions (automated workflow)  
  - Jenkins (optional for advanced use)

---

## 🧰 Tech Stack

- **Postman** – API request creation and test scripting  
- **Newman** – CLI tool to run Postman collections  
- **Node.js** – for executing Newman  
- **GitHub Actions / Jenkins** – CI/CD automation  
- **HTML Extra Reporter** – detailed visual test reports  

---

## 🧩 Project Files

| File | Description |
|------|--------------|
| `User Management API - Basic Auth.postman_collection.json` | Main Postman collection with requests and tests |
| `AUTH API TEST.postman_environment.json` | Environment variables (e.g., Base URL, credentials) |
| `.github/workflows/api-tests.yml` | GitHub Actions workflow for CI/CD |
| `newman-report.html` | HTML report generated after test execution |

---

## 🧠 Test Scenarios

### 🔐 Basic Auth
Verifies API access using valid username and password.

### 🧍‍♂️ Create User (Dynamic Data)
```javascript
pm.variables.set("randomId", Math.floor(Math.random() * 1000) + 1);
pm.variables.set("randomUsername", "user" + Math.floor(Math.random() * 1000));
