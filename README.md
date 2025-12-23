# 📝 Quiz Application – Java | Spring Boot | Maven

A **Java-based Quiz Application** built using **Spring Boot** and **Maven**, designed with a **modular MVC architecture**.  
The application supports **quiz creation, quiz attempts, QR code-based access, authentication**, and **JSON-based storage**, making it lightweight, scalable, and easy to extend.

---

## 🚀 Features

- ✅ Create and manage quizzes  
- ✅ Attempt quizzes with real-time validation  
- ✅ QR code generation for easy quiz access  
- ✅ User authentication and authorization  
- ✅ JSON-based data storage (no external DB required)  
- ✅ Modular **MVC architecture** for clean code separation  
- ✅ RESTful APIs for smooth client-server interaction  

---

## 🛠️ Tech Stack

- **Language:** Java  
- **Framework:** Spring Boot  
- **Build Tool:** Maven  
- **Architecture:** MVC (Model–View–Controller)  
- **Data Storage:** JSON files  
- **Authentication:** Spring Security (basic authentication)  
- **Utilities:** QR Code Generator  

---

## 📂 Project Structure

# QRCodeGenerationApp
quiz-application/
├── src/main/java/
│ ├── controller/ # REST controllers
│ ├── service/ # Business logic
│ ├── model/ # Data models
│ ├── repository/ # JSON storage handlers
│ └── QuizApplication.java
├── src/main/resources/
│ ├── application.properties
│ └── data/ # JSON files
├── pom.xml
└── README.md
🔐 Authentication

Secure endpoints using authentication

User credentials are validated before quiz access

Designed to be easily extendable for JWT or OAuth

📌 API Highlights

POST /quiz/create – Create a new quiz

GET /quiz/{id} – Fetch quiz details

POST /quiz/attempt – Attempt a quiz

GET /quiz/qrcode/{id} – Generate QR code for quiz

🎯 Learning Outcomes

Hands-on experience with Spring Boot & REST APIs

Implemented MVC architecture in a real-world project

Worked with JSON-based persistence

Designed authentication mechanisms

Improved understanding of modular and scalable backend design

📈 Future Enhancements

🔹 Database integration (MySQL/PostgreSQL)

🔹 JWT-based authentication

🔹 Frontend UI (React / Angular)

🔹 Analytics dashboard for quiz performance

👨‍💻 Author

Rudraraju Dhanush Varma
📧 Email: R.Dhanush@iiitb.ac.in

🔗 LinkedIn: Rudraraju Dhanush Varma

🐙 GitHub: (add your GitHub link)
