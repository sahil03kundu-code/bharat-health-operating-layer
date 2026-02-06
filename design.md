# System Design – AI-Powered Healthcare Triage Layer

## 1. Design Overview
This system is designed as a voice-first, AI-assisted healthcare triage layer that operates between patients and the formal healthcare system. It focuses on continuous risk observation rather than one-time consultations, enabling early detection of worsening conditions and timely human intervention.

The architecture follows a layered approach that separates access, intelligence, and care delivery to ensure clarity, safety, and scalability. AI is intentionally constrained to assist with symptom structuring, risk assessment, and trend detection, while all medical decisions remain with human healthcare professionals.

The design prioritizes reliability, responsible AI use, and real-world deployment in rural and semi-rural Indian contexts, where literacy, language diversity, and connectivity constraints must be addressed.


## 2. High-Level Architecture
The system is structured into three clearly separated layers to ensure safety, explainability, and operational clarity.

1. Access Layer  
This layer handles all patient interactions. Patients connect via a phone call or mobile application and communicate using natural speech in their local language. The primary role of this layer is to capture symptoms, duration, severity, and basic patient context in a frictionless manner.

2. Intelligence Layer  
This layer converts raw voice input into structured medical signals. It includes controlled speech-to-structure conversion, AI-assisted risk scoring, and a trend analysis engine that compares current inputs with the patient’s historical data. This layer does not make medical decisions; it only surfaces risk indicators.

3. Care & Escalation Layer  
This layer routes cases based on risk levels. Low-risk cases are monitored, medium-risk cases are flagged for follow-up, and high-risk cases are escalated to human healthcare professionals or nearby facilities for intervention.


## 3. Layered System Design

### 3.1 Access Layer

### 3.2 Intelligence Layer

### 3.3 Care Layer

## 4. Data Flow & Continuity

## 5. Safety & Responsibility Principles

## 6. Scalability & Extensibility

## 7. Design Decisions & Trade-offs
