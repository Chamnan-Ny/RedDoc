# Recon_Manager
Flutter_Project

🕵️ Recon Manager
A Flutter-based reconnaissance management tool designed for penetration tester and cybersecurity learners to organize and structure recon data during security assessments.

🚀 Overview
Recon Mananger helps security professionals and students organize:
- 🌐 Domains & Subdomains
- 🖥 IP Addresses
- 📝 Recon Notes
- 📁 Project-based engagements
instead of using scattered notes or spreadsheets, this app provides a structured way to manage reconnaissance data during ethical hacking and penetration testing labs.

🎯 Features
📁 Project Management
- Create multiple penetration testing projects
- Organize recon per engagement
🌐 Domain Tracking
- Store target domains
- Add subdomains per project
🖥 IP Address Management
- Record discovered IPs
- Attach descriptions (web server, DB, etc.)
📝 Notes System
- Store findings from tools like Nmap, Gobuster, etc.
- Tag and organize notes
🔍 Search System
- Search across projects, domains, and notes
💾 Local Storage
- Offline-first using SQLite database

📱 Screenshots (Add later)
Home Screen
Project List
Project Details
Notes View

🧱 Tech Stack
Layer	            Technology
Frontend	        Flutter
Language	        Dart
Database	        SQLite (sqflite)
State Management	Provider (or setState for beginner version)

🏗 Project Structure
    lib/
    ├── models/        # Data models
    ├── screens/       # UI pages
    ├── services/      # Database logic
    ├── widgets/       # Reusable components
    └── utils/         # Helpers & constants

🧠 Learning Goals
This project demonstrates: 
- Flutter UI development
- State Management
- Local Data Handling (SQLite)
- CRUD Operations
- Data Structuring
- Cybersecurity workflow understaning 

🔐 Cybersecurity Relevance
This app reflects real penetration testing workflow: 
Reconnaissance Phase: 
- Identify domain 
- Map subdomains
- Collect IP addresses 
- Document findings
It helps simulate how professional penetration testers organize reconnaissance data during engagements.

🛠️ Installation
git clone https://github.com/Chamnan-Ny/Recon_Manager.git
cd recon_manager
flutter pub get
flutter run

📌 Future Improvements
- 🔐 Firebase authentication
- ☁️ Cloud sync
- 📸 Screenshot evidence upload
- 📊 Recon analytics dashboard
- 📄 PDF report generation
- 🌙 Dark mode

📸 Demo
(Add GIF or video here later)

👨‍💻 Author
Name: Chamnan Ny , Saknora Song 
Role: Cybersecurity Student
Goal: Penetration Tester 

📄 License
This project is for educational purposes.
