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
 
Phase 1 (coursework MVP) runs on a weekly schedule to the **Jan 2, 2027** submission deadline. Each item is tracked as a GitHub issue.

| Week | Date | Feature | Issues | Status |
|------|------|---------|--------|--------|
| - | - | Project scaffold + Maven/JavaFX setup, MVC restructure | #16-17 | ✅ Done |
| 1 | Oct 24 | Figma designs for all screens + Login screen UI | #1-9 | 🔄 In progress |
| 2 | Oct 31 | Registration, User model, BCrypt hashing, input validation | #10-13 | ⏳ Planned |
| 3 | Nov 7 | Home page + nav, local JSON storage, ticket submission | #14-15, #18-19 | ⏳ Planned |
| 4 | Nov 14 | Ticket lifecycle + ticket log, SMTP email notifications | #20-23 | ⏳ Planned |
| 5 | Nov 21 | Taylor's website scraper (JSoup) + data curation | #24-26 | ⏳ Planned |
| 6 | Nov 28 | FAQ page, chatbot UI + LangChain4j integration | #27-30 | ⏳ Planned |
| 7 | Dec 5 | Chatbot methods + RAG over scraped content (**core feature-complete**) | #31-33 | ⏳ Planned |
| 8 | Dec 12 | Integration testing | #34 | ⏳ Planned |
| 9 | Dec 19 | Bug fixing / catch-up buffer | #35 | ⏳ Planned |
| 10 | Dec 26 | Stretch (if ahead): role-based routing, admin tickets + FAQ CRUD, UI polish | #37-42 | ⏳ Planned |
| 11 | Jan 2 | Final polish, demo run-through, submission | #36 | ⏳ Planned |

**Phase 2 (portfolio extension, Jan 9 - Mar 27, 2027):** migrate to a full-stack app with a Spring Boot + PostgreSQL backend (Docker), JWT auth, REST endpoints for tickets and FAQs, and server-side chatbot calls (#43-66).
 
-------|---------|--------|
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