🛡️ RedDoc - Penetration Testing Report App

A Flutter application designed to help penetration testers organize security assessment projects, document vulnerabilities, manage evidence, and generate professional penetration testing reports.

📖 Overview

Writing a penetration testing report is one of the most important tasks after a security assessment. This application simplifies that process by providing a structured workspace where testers can manage projects, record findings, attach supporting evidence, and generate clear, organized reports.

🎯 Objectives

Create and manage penetration testing projects.
Record vulnerabilities with detailed descriptions.
Classify findings by severity.
Store screenshots and proof-of-concept evidence.
Generate professional penetration testing reports.
Demonstrate Flutter application architecture and local data management.

✨ Features

Project Management
    - Create, edit, and delete penetration testing projects.
    - Store target information, scope, tester name, assessment date, and project status.
    - View all projects from a centralized dashboard.

Vulnerability Management
    - Add, edit, and remove security findings.
    - Record vulnerability descriptions and remediation recommendations.
    Assign severity levels:
        - 🟢 Low
        - 🟡 Medium
        - 🟠 High
        - 🔴 Critical
    - Track finding status (Open, Fixed, Accepted Risk).

Evidence Management
    - Attach screenshots.
    - Save proof-of-concept notes.
    - Organize evidence for each vulnerability.

Report Generation
    - Generate a professional PDF report containing:
        - Executive Summary
        - Project Information
        - Vulnerability Findings
        - Severity Assessment
        - Remediation Recommendations
        - Supporting Evidence

🏗️ Technology Stack
Framework: Flutter
Language: Dart
Local Database: Hive
State Management: (To be determined)
PDF Generation: pdf
Image Handling: image_picker

📂 Project Structure
lib/
├── models/
├── data/
├── screens/
├── widgets/
├── services/
└── main.dart

🎓 Purpose

This project was developed as a university portfolio project to practice Flutter development while applying concepts commonly used in cybersecurity reporting. The focus is on improving documentation workflows rather than performing offensive security operations.

🚀 Future Improvements
    - CVE reference integration.
    - Report templates.
    - Search and filtering.
    - Team collaboration.
    - Cloud synchronization.
    - Dashboard analytics.
    - Dark mode.

⚠️ Disclaimer

This application is intended for educational purposes and authorized security assessments only. It does not include offensive security capabilities or automated vulnerability scanning. Users are responsible for ensuring that any penetration testing activities are performed with proper authorization.

👨‍💻 Author

Developed as a Flutter portfolio project to explore the intersection of mobile application development and cybersecurity reporting.