# GitHub – Projects Overview  
Kapischan Sriganthan | BSc Business Information Technology (FHNW)

This repository serves as a **central entry point** to my software engineering, data science, and research-oriented projects.  
Each listed repository contains its **own detailed README** with technical explanations, setup instructions, and documentation.

The projects cover **software architecture, backend systems, algorithms, machine learning, AI-supported applications, and client development**, spanning coursework, applied projects, and published research.

---

## Project Roll-up (English)

### 📦 Software Engineering Portfolio
**Scope:** Aggregated coursework projects  
**Focus:** Core software engineering fundamentals

Collection of multiple study projects covering:
- graph search and navigation algorithms
- REST-based backend systems
- cryptography implementations
- server-side architectures and system design

This repository acts as a **container for multiple smaller projects**, each documented individually.

🔗 Repository:  
https://github.com/ksriganthan/SoftwareEngineeringPortfolio.git

---

### 🧠 Adaptive Phishing Awareness Training (LLM-based)
**Scope:** Research & publication  
**Focus:** AI, cybersecurity awareness, human-centered learning

Research-driven project on **interactive phishing awareness training**, evolving from a rule-based chatbot to an **LLM-supported adaptive learning environment**.

- Proof of Concept → research prototype
- Focus on the human factor in cybersecurity
- Peer-reviewed IEEE publication (RTSI 2025)
- Clear connection between academic research and implementation

🔗 Repository:  
https://github.com/ksriganthan/Adaptive-Phishing-Awareness-Training-Environment-with-LLM-Interactive-Learning.git

---

### 🏗️ Software Architecture – Integration Cases
**Scope:** Six connected module cases (FHNW)<br>**Focus:** Process orchestration, rule engines, messaging, ESB, stream processing

Six cases around one question: how do systems talk to each other, and who decides what happens next? Each case answers it with a different mechanism, and each one exposes the limits of the previous.

- Camunda BPMN processes driven by external task workers (Java, Spring Boot)
- Rule-based shipping decisions via Drools and a decision table maintained in Excel
- Message-based job dispatch over ActiveMQ, using JMS topics and queues deliberately
- MuleSoft ESB integrating a SOAP service into the messaging layer, with content-based routing and a dead letter queue
- Kafka Streams pipeline detecting delivery delays in a continuous GPS event stream
- Customer lookup worker with failure classified into business errors, technical errors, and fallback

🔗 Documented overview:
[https://github.com/ksriganthan/software-architecture-cases](https://github.com/ksriganthan/software_architecture)

---

### ⚖️ PackOps – Industrial Weighing Machine Simulation
**Scope:** Five-person team project (FHNW, IT-Projekt)<br>**Focus:** Client-server architecture, discrete simulation, full-stack development

Software simulation of a **Newtec Weighing Machine 2008PCM** with memory pans. The core is a combination problem: out of a continuous stream of portions with varying weights, the machine has to form packages that land as close as possible to a target weight — within tolerance, and without individual portions getting stuck in the system.

- Simulation engine over **8 parallel channels**, each with buffer, weighing and two memory buckets; a scheduled tick advances material by pull principle, searches for the best cross-channel weight combination, and retires portions that repeatedly fail as deadlocks
- Spring Boot backend (Java 21) with a layered architecture and an isolated simulation package
- React 19 / TypeScript frontend with a live dashboard, product catalog, statistics and user management
- JWT authentication with three roles (admin, operator, viewer) and resource-level authorization
- Trilingual (DE / EN / FR) down to product names and backend status messages, via relational translation tables
- Containerized with Docker Compose: backend, Nginx-served frontend and PostgreSQL
- Tested on three levels: unit, integration and 8 Playwright end-to-end cases

**My contribution:** process handling (overview, details, live status), product catalog, user management, validation and logging.

🔗 Documented overview:
https://github.com/ksriganthan/packops

🔗 Backend:
https://github.com/ksriganthan/packops-backend

---

### 🛒 Agile Application Lifecycle Management – Microservices
**Scope:** Architecture-focused coursework  
**Focus:** Microservices, REST, resilience

Implementation of a **microservice-based e-commerce system** consisting of:
- Catalog Service (REST API, persistence)
- Order Service (web UI, service integration)

Key aspects include:
- polyrepo microservice architecture
- Docker and Docker Compose
- resilience patterns and integration testing

🔗 Repository:  
https://github.com/ksriganthan/Agile_Application_Lifecycle_Management.git

---

### 🎮 Battleship Client (Android)
**Scope:** Client application  
**Focus:** Mobile development & client–server interaction

Android client for a multiplayer **Battleship game**, focusing on modern mobile development practices.

Key aspects:
- Kotlin and Jetpack Compose
- MVVM architecture
- REST-based communication with a game server
- UI state and interaction management

🔗 Repository:  
https://github.com/ksriganthan/Battleship_Client.git

---

### 🤖 Machine Learning with Python
**Scope:** Data science & machine learning coursework  
**Focus:** Python fundamentals and classical machine learning

Structured learning repository developed in the module **Business Analytics / Machine Learning with Python (FHNW)**.

Key aspects:
- Python fundamentals (data structures, file I/O, visualization)
- Supervised learning (k-NN, Decision Trees, Neural Networks)
- Unsupervised learning (Hierarchical Clustering)
- Model evaluation (Train/Test Split, Cross-Validation, HPO)
- Emphasis on understanding algorithms, not black-box usage

🔗 Repository:  
https://github.com/ksriganthan/MLwithPython.git

---

## How to Use This Overview

- Use this page as a **high-level profile**
- Follow the links to access **project-specific READMEs**
- Each repository is self-contained and documents its goals, architecture, and implementation

---

## Contact
Kapischan Sriganthan  
kapischan.sriganthan@outlook.com

---
<details>
<summary><b>Projektübersicht auf Deutsch</b></summary>

# GitHub – Projektübersicht  
Kapischan Sriganthan | BSc Wirtschaftsinformatik (FHNW)

Dieses Dokument dient als **zentraler Einstiegspunkt** zu meinen Projekten in den Bereichen Software Engineering, Machine Learning und angewandter Forschung.  
Jedes verlinkte Repository enthält eine **eigene ausführliche README** mit technischen Details und Dokumentation.

Die Projekte decken **Backend-Systeme, Softwarearchitektur, Algorithmen, Machine Learning, KI-nahe Anwendungen und Client-Entwicklung** ab.

---

## Projekt-Roll-up (Deutsch)

### 📦 Software Engineering Portfolio
**Umfang:** Aggregierte Studienprojekte  
**Schwerpunkt:** Software-Engineering-Grundlagen

Sammlung mehrerer Projekte aus dem Studium, u. a.:
- Navigations- und Suchalgorithmen
- REST-basierte Backend-Systeme
- Kryptografie-Implementierungen
- Server-Architekturen

🔗 Repository:  
https://github.com/ksriganthan/SoftwareEngineeringPortfolio.git

---

### 🧠 Adaptive Phishing Awareness Training (LLM-basiert)
**Umfang:** Forschung & Publikation  
**Schwerpunkt:** KI und Security Awareness

Forschungsprojekt zur **interaktiven Phishing-Awareness-Schulung**, von einem Proof of Concept bis zu einem **LLM-basierten Forschungsprototyp**.

- Fokus auf den menschlichen Faktor
- Enge Verbindung von Theorie und Implementierung
- IEEE-Publikation (RTSI 2025)

🔗 Repository:  
https://github.com/ksriganthan/Adaptive-Phishing-Awareness-Training-Environment-with-LLM-Interactive-Learning.git

---

### 🏗️ Software Architecture – Integration Cases
**Umfang:** Sechs aufeinander aufbauende Modul-Cases (FHNW)<br>**Schwerpunkt:** Prozessorchestrierung, Regel-Engines, Messaging, ESB, Stream Processing

Sechs Cases rund um eine Frage: Wie sprechen Systeme miteinander, und wer entscheidet, was als Nächstes passiert? Jeder Case beantwortet sie mit einem anderen Mechanismus – und jeder zeigt, wo der vorherige an seine Grenze kommt.

- Camunda-BPMN-Prozesse, angetrieben von External Task Workern (Java, Spring Boot)
- Regelbasierte Versandentscheidungen über Drools und eine in Excel gepflegte Entscheidungstabelle
- Nachrichtenbasierte Auftragsdisposition über ActiveMQ, mit bewusst gewählten JMS-Topics und -Queues
- MuleSoft-ESB, der einen SOAP-Service in die Messaging-Schicht integriert, mit inhaltsbasiertem Routing und Dead Letter Queue
- Kafka-Streams-Pipeline, die Lieferverzögerungen in einem kontinuierlichen GPS-Eventstrom erkennt
- Customer-Lookup-Worker, der Fehler in fachliche, technische und Fallback-Fälle trennt

🔗 Dokumentierte Übersicht:
[https://github.com/ksriganthan/software-architecture-cases](https://github.com/ksriganthan/software_architecture)

---

### ⚖️ PackOps – Simulation einer industriellen Wiegemaschine
**Umfang:** Fünfköpfiges Teamprojekt (FHNW, IT-Projekt)<br>**Schwerpunkt:** Client-Server-Architektur, Simulation, Full-Stack-Entwicklung

Softwareseitige Simulation einer **Newtec Weighing Machine 2008PCM** mit Memory Pans. Im Kern steht ein Kombinationsproblem: Aus einem laufenden Strom von Portionen unterschiedlichen Gewichts muss die Anlage Packungen bilden, die möglichst nahe an einem Zielgewicht liegen – innerhalb der Toleranz und ohne dass einzelne Portionen im System hängen bleiben.

- Simulationskern über **8 parallele Kanäle** mit Buffer-, Weighing- und je zwei Memory-Buckets; ein zeitgesteuerter Tick schiebt Material nach dem Pull-Prinzip weiter, sucht kanalübergreifend die beste Gewichtskombination und führt dauerhaft erfolglose Portionen als Deadlock zurück
- Spring-Boot-Backend (Java 21) mit geschichteter Architektur und gekapseltem Simulations-Package
- React-19-/TypeScript-Frontend mit Live-Dashboard, Produktkatalog, Statistiken und Benutzerverwaltung
- JWT-Authentifizierung mit drei Rollen (admin, operator, viewer) und ressourcenbezogener Berechtigungsprüfung
- Dreisprachig (DE / EN / FR) bis hinunter zu Produktnamen und Statusmeldungen des Backends, über relationale Übersetzungstabellen
- Containerisiert mit Docker Compose: Backend, Frontend hinter Nginx und PostgreSQL
- Auf drei Ebenen getestet: Unit, Integration und 8 Playwright-End-to-End-Fälle

**Mein Beitrag:** Prozessverwaltung (Übersicht, Details, Live-Status), Produktkatalog, Benutzerverwaltung, Validierung und Logging.

🔗 Dokumentierte Übersicht:
https://github.com/ksriganthan/packops

🔗 Backend:
https://github.com/ksriganthan/packops-backend

---

### 🛒 Agile Application Lifecycle Management – Microservices
**Umfang:** Architekturprojekt  
**Schwerpunkt:** Microservices & REST

Umsetzung eines **Microservice-basierten E-Commerce-Systems** mit klarer Service-Trennung und Containerisierung.

🔗 Repository:  
https://github.com/ksriganthan/Agile_Application_Lifecycle_Management.git

---

### 🎮 Battleship Client (Android)
**Umfang:** Client-Applikation  
**Schwerpunkt:** Mobile Entwicklung

Android-Client für ein Multiplayer-Battleship-Spiel mit Fokus auf moderne UI-Architektur und Client–Server-Kommunikation.

🔗 Repository:  
https://github.com/ksriganthan/Battleship_Client.git

---

### 🤖 Machine Learning with Python
**Umfang:** Data Science & Machine Learning  
**Schwerpunkt:** Grundlagen und klassische ML-Verfahren

Strukturiertes Lern-Repository aus dem Modul **Business Analytics / Machine Learning with Python**.

Schwerpunkte:
- Python-Grundlagen
- Supervised & Unsupervised Learning
- Modellbewertung und Hyperparameter-Tuning
- Verständnis der Algorithmen statt Black-Box-Nutzung

🔗 Repository:  
https://github.com/ksriganthan/MLwithPython.git

---

## Zweck dieser Übersicht

Diese Übersicht dient:
- als **Profil-README**
- als Navigationspunkt über alle Projekte
- als Einstieg für Dozierende, Recruiter und Reviewer

</details>
---

## Weitere Repositories mit Übungen und Mini-Projekte auf GitLab
https://gitlab.fhnw.ch/dashboard/projects

## Kontakt
Kapischan Sriganthan  
kapischan.sriganthan@outlook.com
