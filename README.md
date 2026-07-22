RedDoc 
A Penetration Testing Report Management Application

RedDoc is a Flutter-based penetration testing report management application designed to help penetration testers organize, document, and manage vulnerability findings during security assessments. The application provides a centralized platform for creating penetration testing projects, recording vulnerabilities, attaching evidence screenshots, and tracking reports in the cloud.

RedDoc uses Firebase Authentication for secure user registration and login, Cloud Firestore for cloud-based data storage, and Firebase Storage for storing vulnerability evidence. The application follows a layered architecture using models, repositories, services, and UI components to demonstrate clean software engineering practices.

This project is developed as an educational cybersecurity mobile application for the Mobile Development in Cybersecurity course. It demonstrates Flutter development, Firebase integration, CRUD operations, image upload, repository architecture, and secure management of penetration testing reports.

Note: The current version focuses on the Report Designer module. The Manager review workflow is planned as a future enhancement.

+ Project Direction

Cybersecurity Application — Penetration Testing Report Management

RedDoc assists penetration testers in documenting and organizing security assessment results throughout the penetration testing process. Rather than generating traditional PDF reports, the application provides a cloud-based workspace where findings and supporting evidence can be managed digitally.

+ Key Features
- Firebase Authentication
User registration
Email & Password login
Secure logout
- Project Management

Users can:

Create penetration testing projects
View project information
Edit project details
Delete projects
Search projects
- Vulnerability Findings Management

Users can:

Add vulnerability findings
Edit findings
Delete findings
Assign severity levels
Write vulnerability descriptions
Add remediation recommendations
- Evidence Upload

Users can upload supporting evidence such as:

Burp Suite screenshots
Browser screenshots
Request/Response captures
Proof-of-concept images

Evidence is stored securely in Firebase Storage.

☁️ Cloud Database

Project information and vulnerability findings are synchronized using Cloud Firestore.

- Search, Filter & Sort

Users can:

Search projects
Search findings
Filter findings by severity
Sort findings alphabetically
Sort findings by creation date
- Layered Architecture

The project follows the course architecture using:

models/
data/
repositories/
services/
ui/screens/
ui/widgets/
- Data Managed in RedDoc

The application manages penetration testing information including:

Projects
Vulnerability findings
Severity levels
Recommendations
Evidence screenshots
Project metadata
🛠️ Main Technologies
Technology	Purpose
Flutter	Mobile application framework
Dart	Programming language
Firebase Authentication	User authentication
Cloud Firestore	Cloud database
Firebase Storage	Image storage
image_picker	Upload evidence screenshots
Stateful Widgets	State management
Repository Pattern	Data access layer
- Current User Role
Report Designer

The current version of RedDoc is designed for penetration testers who create and manage security assessment reports.

Responsibilities:

Create penetration testing projects
Manage project information
Add vulnerability findings
Edit vulnerability findings
Delete vulnerability findings
Upload evidence screenshots
Search projects
Search findings
Filter findings
Sort findings
📱 App Screens
1. Splash Screen

Checks authentication status and redirects users to the appropriate screen.

2. Login Screen

Allows existing users to sign in using Firebase Authentication.

3. Register Screen

Allows new users to create an account.

4. Dashboard Screen

Displays project statistics and recently created projects.

5. Create Project Screen

Allows users to create a new penetration testing project.

6. Project Detail Screen

Displays project information and a list of vulnerability findings.

7. Finding Form Screen

Allows users to add or edit vulnerability findings.

8. Finding Detail Screen

Displays complete vulnerability information including:

Severity
Description
Recommendation
Evidence screenshots
9. Profile Screen

Allows users to view profile information and log out.

Basic User Flow
Open App
    ↓
Splash Screen
    ↓
Login / Register
    ↓
Firebase Authentication
    ↓
Dashboard
    ↓
Create Project
    ↓
Project Detail
    ↓
Add Finding
    ↓
Upload Evidence
    ↓
Save Finding
    ↓
View / Search / Filter / Sort Findings
📂 Project Structure
lib/
│
├── models/
│   ├── user_model.dart
│   ├── project_model.dart
│   ├── finding_model.dart
│   └── evidence_model.dart
│
├── data/
│   ├── repositories/
│   │   ├── auth_repository.dart
│   │   ├── project_repository.dart
│   │   ├── finding_repository.dart
│   │   └── storage_repository.dart
│   │
│   └── services/
│       ├── firebase_auth_service.dart
│       ├── firestore_service.dart
│       ├── storage_service.dart
│       └── image_picker_service.dart
│
├── ui/
│   ├── screens/
│   │   ├── auth/
│   │   ├── dashboard/
│   │   ├── project/
│   │   ├── finding/
│   │   └── profile/
│   │
│   ├── widgets/
│   └── theme/
│       └── app_theme.dart
│
├── firebase_options.dart
└── main.dart
+ Model Classes
UserModel

Represents the authenticated user.

uid
name
email
ProjectModel

Represents a penetration testing project.

projectId
title
target
scope
createdAt
FindingModel

Represents a vulnerability finding.

findingId
projectId
title
severity
description
recommendation
createdAt
EvidenceModel

Represents uploaded vulnerability evidence.

evidenceId
findingId
imageUrl
note
+ Cloud Firestore Collections
users

Stores authenticated user information.

projects

Stores penetration testing projects.

findings

Stores vulnerability findings.

evidence

Stores uploaded evidence metadata.

+ Severity Levels
Critical
High
Medium
Low
Informational
+ Security Notes

RedDoc is designed to securely manage penetration testing reports.

Security principles include:

Firebase Authentication securely manages user accounts.
Cloud Firestore stores project and finding data.
Firebase Storage securely stores uploaded evidence.
Authentication is required before accessing project data.
🚀 Project Setup
Prerequisites
Flutter SDK
Dart SDK
Android Studio or Visual Studio Code
Firebase Project
FlutterFire CLI
Installation
1. Clone the repository
git clone https://github.com/yourusername/reddoc.git
cd reddoc
2. Install dependencies
flutter pub get
3. Configure Firebase

Enable the following Firebase services:

Authentication (Email & Password)
Cloud Firestore
Firebase Storage

Run:

flutterfire configure
4. Verify Flutter setup
flutter doctor
5. Run the application
flutter run
📦 Required Packages
Main Packages
firebase_core
firebase_auth
cloud_firestore
firebase_storage
image_picker
intl
uuid
Development Packages
flutter_lints
🚀 Future Improvements

The following features are planned for future versions:

+ Manager Module
Manager authentication
Manager dashboard
Report review workflow
Approval and rejection system
Revision requests
Review comments
Report status tracking
Role-Based Access Control (RBAC)
+ Additional Features
PDF report generation
CVSS score calculator
Push notifications
Email notifications
Activity history
Team collaboration
Report templates
Dark mode
Multi-language support
👥 Contributors

Prepared By: Ny Chamnan , Song Saknora

Course: Mobile Development in Cybersecurity

Lecturer: Mr. Ronan Ogor

Department: Telecom and Networking, Cyber Security

Institution: Cambodia Academy of Digital Technology (CADT)

📄 License

This project is developed for educational purposes as part of the Mobile Development in Cybersecurity course at CADT.

                                        Export Report
