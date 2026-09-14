# GitHub – Projects Overview  
Kapischan Sriganthan | BSc Business Information Technology (FHNW)

🇩🇪 **Deutsche Fassung:** [Projektübersicht auf Deutsch](#github--projektübersicht) (weiter unten, zum Aufklappen)

This page serves as a **central entry point** to my software engineering, data science, and research-oriented projects.  
Each listed repository contains its **own detailed README** with technical explanations, setup instructions, and documentation.

The projects cover **LLM applications and retrieval, software architecture, backend systems, algorithms, machine learning, and client development**, spanning a personal AI engineering sprint, coursework, applied projects, and published research.

---

## Project Roll-up (English)

### 🗂️ hr-policy-assistant – RAG over Swiss Collective Labour Agreements
**Scope:** Personal project, eight-week AI engineering sprint (24 Aug – 18 Oct 2026), in progress<br>**Focus:** Retrieval-augmented generation, LLM gateway, measured evaluation

Question-answering system over public Swiss collective labour agreements (GAV) that cites its sources down to section number and page. Developed with AI assistance, every decision documented and re-measured against a fixed set of test questions after each change.

- ETL pipeline from PDF into a Chroma vector store: Unicode normalisation, header and footer removal by repetition count, chunking at section numbers with hierarchy path, tables rewritten row by row so every value keeps its column
- Local embeddings (`bge-m3`) and a local language model (`gemma3:12b`) via Ollama, nothing leaves the machine
- Own LLM gateway for every model call: one JSONL log line per call, retry with exponential backoff on connection errors, token and cost accounting
- Answers with numbered citations; prompt rules derived from measured failures, each documented with the measurement behind it
- Structured output with Pydantic, a FastAPI endpoint, and an evaluation set of 20 questions with a target answer fixed per hospital before the run, measured in a reproducible baseline
- Next in the sprint: LangGraph workflow with a critic role, agent loop for comparison, Docker and GitHub Actions CI

🔗 Repository:  
https://github.com/ksriganthan/hr-policy-assistant

---

### 📦 Software Engineering Portfolio
**Scope:** Aggregated coursework projects<br>**Focus:** Core software engineering fundamentals

Collection of multiple study projects covering:
- graph search and navigation algorithms
- REST-based backend systems
- cryptography implementations
- server-side architectures and system design

This repository acts as a **container for multiple smaller projects**, each documented individually.

🔗 Repository:  
https://github.com/ksriganthan/SoftwareEngineeringPortfolio

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
https://github.com/ksriganthan/software_architecture

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
**Scope:** Architecture-focused coursework<br>**Focus:** Microservices, REST, resilience

Implementation of a **microservice-based e-commerce system** consisting of:
- Catalog Service (REST API, persistence)
- Order Service (web UI, service integration)

Key aspects include:
- polyrepo microservice architecture
- Docker and Docker Compose
- resilience patterns and integration testing

🔗 Repository:  
https://github.com/ksriganthan/Agile_Application_Lifecycle_Management

---

### 🎮 Battleship Client (Android)
**Scope:** Client application<br>**Focus:** Mobile development & client–server interaction

Android client for a multiplayer **Battleship game**, focusing on modern mobile development practices.

Key aspects:
- Kotlin and Jetpack Compose
- MVVM architecture
- REST-based communication with a game server
- UI state and interaction management

🔗 Repository:  
https://github.com/ksriganthan/Battleship_Client

---

### 🤖 Machine Learning with Python
**Scope:** Data science & machine learning coursework<br>**Focus:** Python fundamentals and classical machine learning

Structured learning repository developed in the module **Business Analytics / Machine Learning with Python (FHNW)**.

Key aspects:
- Python fundamentals (data structures, file I/O, visualization)
- Supervised learning (k-NN, Decision Trees, Neural Networks)
- Unsupervised learning (Hierarchical Clustering)
- Model evaluation (Train/Test Split, Cross-Validation, HPO)
- Emphasis on understanding algorithms, not black-box usage

🔗 Repository:  
https://github.com/ksriganthan/MLwithPython

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

Die Projekte decken **LLM-Anwendungen und Retrieval, Backend-Systeme, Softwarearchitektur, Algorithmen, Machine Learning und Client-Entwicklung** ab.

---

## Projekt-Roll-up (Deutsch)

### 🗂️ hr-policy-assistant – RAG über Schweizer Gesamtarbeitsverträge
**Umfang:** Eigenprojekt, achtwöchiger AI-Engineering-Sprint (24.08.–18.10.2026), in Arbeit<br>**Schwerpunkt:** Retrieval-Augmented Generation, LLM-Gateway, gemessene Evaluation

Frage-Antwort-System über öffentliche Schweizer Gesamtarbeitsverträge (GAV), das seine Quellen bis auf Ziffer und Seite belegt. Entwickelt mit AI-Unterstützung, jede Entscheidung dokumentiert und nach jeder Änderung an einem festen Satz Testfragen gemessen.

- ETL-Strecke vom PDF in einen Chroma-Vektorstore: Unicode-Normalisierung, Kopf- und Fusszeilen über ihre Wiederholung entfernt, Schnitt an Gliederungsziffern mit Hierarchiepfad, Tabellen zeilenweise umgeschrieben, sodass jeder Wert seine Spalte behält
- Lokale Embeddings (`bge-m3`) und lokales Sprachmodell (`gemma3:12b`) über Ollama, nichts verlässt den Rechner
- Eigenes LLM-Gateway für jeden Modellaufruf: eine JSONL-Zeile pro Aufruf, Wiederholung mit exponentiellem Backoff bei Verbindungsfehlern, Token- und Kostenzählung
- Antworten mit nummerierten Belegstellen; Prompt-Regeln aus gemessenen Fehlern abgeleitet, jede mit der Messung dahinter dokumentiert
- Strukturierte Ausgabe mit Pydantic, FastAPI-Endpunkt und ein Eval-Set mit 20 Fragen und vor dem Lauf festgelegter Sollantwort je Haus, in einem reproduzierbaren Baseline-Lauf gemessen
- Als Nächstes im Sprint: LangGraph-Workflow mit Kritik-Rolle, Agent-Loop zum Vergleich, Docker und GitHub-Actions-CI

🔗 Repository:  
https://github.com/ksriganthan/hr-policy-assistant

---

### 📦 Software Engineering Portfolio
**Umfang:** Aggregierte Studienprojekte<br>**Schwerpunkt:** Software-Engineering-Grundlagen

Sammlung mehrerer Projekte aus dem Studium, u. a.:
- Navigations- und Suchalgorithmen
- REST-basierte Backend-Systeme
- Kryptografie-Implementierungen
- Server-Architekturen und Systementwurf

Dieses Repository dient als **Container für mehrere kleinere Projekte**, jedes einzeln dokumentiert.

🔗 Repository:  
https://github.com/ksriganthan/SoftwareEngineeringPortfolio

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
https://github.com/ksriganthan/software_architecture

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
**Umfang:** Architekturorientiertes Studienprojekt<br>**Schwerpunkt:** Microservices, REST, Resilience

Umsetzung eines **Microservice-basierten E-Commerce-Systems**, bestehend aus:
- Catalog Service (REST-API, Persistenz)
- Order Service (Weboberfläche, Service-Integration)

Schwerpunkte:
- Polyrepo-Microservice-Architektur
- Docker und Docker Compose
- Resilience-Patterns und Integrationstests

🔗 Repository:  
https://github.com/ksriganthan/Agile_Application_Lifecycle_Management

---

### 🎮 Battleship Client (Android)
**Umfang:** Client-Applikation<br>**Schwerpunkt:** Mobile Entwicklung und Client–Server-Interaktion

Android-Client für ein Multiplayer-**Battleship-Spiel** mit Fokus auf moderne Praktiken der Mobile-Entwicklung.

Schwerpunkte:
- Kotlin und Jetpack Compose
- MVVM-Architektur
- REST-basierte Kommunikation mit einem Spielserver
- Verwaltung von UI-Zustand und Interaktion

🔗 Repository:  
https://github.com/ksriganthan/Battleship_Client

---

### 🤖 Machine Learning with Python
**Umfang:** Studienprojekt in Data Science und Machine Learning<br>**Schwerpunkt:** Python-Grundlagen und klassische ML-Verfahren

Strukturiertes Lern-Repository aus dem Modul **Business Analytics / Machine Learning with Python (FHNW)**.

Schwerpunkte:
- Python-Grundlagen (Datenstrukturen, Datei-Ein- und -Ausgabe, Visualisierung)
- Supervised Learning (k-NN, Decision Trees, Neuronale Netze)
- Unsupervised Learning (Hierarchisches Clustering)
- Modellbewertung (Train/Test-Split, Cross-Validation, Hyperparameter-Optimierung)
- Verständnis der Algorithmen statt Black-Box-Nutzung

🔗 Repository:  
https://github.com/ksriganthan/MLwithPython

---

## Zweck dieser Übersicht

Diese Übersicht dient:
- als **Profil-README**
- als Navigationspunkt über alle Projekte
- als Einstieg für Dozierende, Recruiter und Reviewer

</details>
