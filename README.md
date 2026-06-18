<div align="center">

# 🎓 CampusPal
 
### AI-Powered Student Helpdesk Desktop Application
 
*Helping students get answers anytime, even when the helpdesk is closed.*
 
![Status](https://img.shields.io/badge/Status-In%20Development-orange?style=for-the-badge)
![Java](https://img.shields.io/badge/Java-21%20LTS-007396?style=for-the-badge&logo=openjdk&logoColor=white)
![JavaFX](https://img.shields.io/badge/JavaFX-21.0.2-1E90FF?style=for-the-badge&logo=java&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-3.9.15-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)
![License](https://img.shields.io/badge/License-Academic-blue?style=for-the-badge)
 
</div>

---
 
## 📖 About
 
**CampusPal** is a desktop helpdesk application built for university students who need academic and administrative support, but can't always wait for office hours.
 
Whether it's a student overseas dealing with visa issues, someone with class clashes or just a 2am question about exam timetables, CampusPal gives them somewhere to ask, find answers and get help.
 
> 🎯 This is my coursework project for **ITS66704 Advanced Programming** at **Taylor's University Malaysia**, built as part of my Bachelor of Computer Science (Honours)
 
---
 
## ✨ Features
 
| Feature | What it does |
|---------|-------------|
| 🔐 **Authentication** | Secure login and registration with role-based access (Student / Admin) |
| 🎫 **Support Tickets** | Submit, track, update, and resolve issues end-to-end |
| 📧 **Email Notifications** | Automated SMTP updates when ticket status changes |
| 📚 **FAQ Knowledge Base** | Searchable common questions, manageable by admins |
| 🤖 **AI Chatbot** | LangChain4j-powered assistant for 24/7 instant support |
| 💾 **Offline-First** | Local JSON storage - works without internet, no external DB needed |
 
---
 
## 🛠️ Tech Stack
 
**Core**
- Java 21 LTS
- JavaFX 21
- FXML + Scene Builder
- Maven
**Architecture**
- Model-View-Controller (MVC)
- Service layer
- Local JSON persistence
**Integrations**
- LangChain4j
- Jakarta Mail (SMTP)
- BCrypt

---
 
## 🏗️ Project Structure
 
```
campuspal/
├── src/main/
│   ├── java/com/campuspal/
│   │   ├── App.java                  ← JavaFX entry point
│   │   ├── controller/               ← UI logic (button clicks, form handling)
│   │   ├── model/                    ← Data classes (User, Ticket, FAQ)
│   │   ├── service/                  ← Business logic (Auth, Tickets, Email)
│   │   └── util/                     ← Helpers (JSON storage, hashing)
│   └── resources/com/campuspal/      ← FXML view files
├── pom.xml                           ← Maven configuration
└── README.md
```
 
---
 
## 🚀 Getting Started
 
### Prerequisites
 
| Tool | Version | Purpose |
|------|---------|---------|
| **JDK** | 21 (LTS) | Java runtime + compiler |
| **Maven** | 3.9+ | Build & dependency management |
| **Scene Builder** | Latest (Gluon) | Visual FXML editor |
 
### Run locally
 
```bash
# Clone the repo
git clone https://github.com/sabinshamsul/campuspal.git
cd campuspal
 
# Build and launch
mvn clean javafx:run
``` 
---
 
## 🗺️ Development Roadmap
 
| Stage | Feature | Status |
|-------|---------|--------|
| 1 | Project scaffold + Maven/JavaFX setup | ✅ Done |
| 2 | MVC structure + Login screen UI | 🔄 In progress |
| 3 | Registration + JSON user storage + BCrypt hashing | ⏳ Planned |
| 4 | Home page + navigation + role-based routing | ⏳ Planned |
| 5 | Support tickets (full lifecycle) | ⏳ Planned |
| 6 | FAQ page + admin CRUD | ⏳ Planned |
| 7 | LangChain4j AI chatbot integration | ⏳ Planned |
| 8 | SMTP email notifications + UI polish | ⏳ Planned |
 
---
 
## 📐 System Design
 
The application follows **MVC architecture**:
 
- **Model** - Domain entities (User, Ticket, FAQ, ChatBot, Email) handled via JSON serialisation
- **View** - JavaFX scenes defined in FXML and designed visually in Scene Builder
- **Controller** - Java classes that handle UI events and bridge the View with the Model/Service layers
 
---
 
## 🙏 Acknowledgements
 
- **Ts. Dr. Steve Teoh Chee Hooi** - Course tutor, ITS66704 Advanced Programming
- **Taylor's University Malaysia** - School of Computer Science
- **Lai Jhoon Sern** - Project partner

---
 
## 📄 License
 
This repo is an academic coursework. Code is shared publicly for portfolio purposes. Please respect Taylor's University's academic integrity policies if you're a student *(do not copy this for your own assignment)*.