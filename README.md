# 🗳️ Online Poll / Voting Application  
### Spring Boot + Angular + Bootstrap CSS

An end-to-end web application that allows users to create polls, vote on options, and view results in real time.  
Built using **Spring Boot** for the backend and **Angular + Bootstrap** for the frontend.

---

## 🚀 Features

- Create polls with multiple options  
- Retrieve all existing polls  
- Vote on any poll option  
- View updated vote counts instantly  
- REST API with clean endpoints  
- Fully responsive UI built with Bootstrap  
- Seamless interaction between Angular frontend and Spring Boot backend  

---

## 🛠️ Tech Stack

### **Frontend**
- Angular  
- TypeScript  
- Bootstrap CSS  

### **Backend**
- Spring Boot  
- Java  
- Spring Data JPA  
- H2 / MySQL (configurable)

---

## 📡 API Endpoints

| API | Endpoint | Method | Description | Request Body | Response |
|-----|----------|--------|-------------|--------------|----------|
| **Create Poll** | `/api/polls` | **POST** | Creates a new poll with options for voting. | JSON | **201 Created** with created poll. |
| **Get All Polls** | `/api/polls` | **GET** | Retrieves a list of all polls. | None | **200 OK** with list of polls. |
| **Get Poll by ID** | `/api/polls/{id}` | **GET** | Retrieves details of a specific poll by ID. | None | **200 OK** or **404 Not Found**. |
| **Vote on Poll** | `/api/polls/vote` | **POST** | Submits a vote for a selected option in a poll. | Poll ID + Option Index | **204 No Content**. |

---
Online-Poll_Voting-Application/
│
├── poll-app/ # Angular Frontend
│ ├── src/
│ ├── package.json
│ └── angular.json
│
└── votingapp/ # Spring Boot Backend
├── src/main/java/com/voting/votingapp
│ ├── Controller
│ ├── Module
│ ├── Repository
│ └── Service
├── application.properties
└── pom.xml


---

## ▶️ How to Run the Application

### **1️⃣ Start Backend (Spring Boot)**

```bash
cd votingapp
mvn spring-boot:run
```
Backend will run at:
👉 http://localhost:8080

### **2️⃣ Start Frontend (Angular)
```bash
cd poll-app
npm install
ng serve
```

Frontend will run at:
👉 http://localhost:4200
## 📁 Project Structure

# 🧪 Sample JSON for Creating a Poll
```
{
  "question": "What is your favorite programming language?",
  "options": [
    { "optionText": "Java", "voteCount": 0 },
    { "optionText": "JavaScript", "voteCount": 0 }
  ]
}
```
# 📷 Screenshots
![image alt](https://github.com/patelaviral/Online-Poll_Voting-Application/blob/c3be283c238a62e0ca62581459ba3f8f078f3a73/vote_poll_application.png)
