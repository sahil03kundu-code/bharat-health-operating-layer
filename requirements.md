# AI-Powered Rural Healthcare Triage System – Requirements

## 1. Problem Statement
India’s healthcare system faces a critical imbalance between patient demand and available medical professionals, especially in rural and semi-rural regions. While national programs and physical infrastructure exist, access to timely care remains inconsistent due to delayed detection, fragmented follow-up, and overburdened frontline health workers and doctors.

Most rural patients seek care only when symptoms become severe, not because services are unavailable, but because the system lacks a mechanism to continuously observe risk and guide escalation over time. Healthcare interactions are episodic, data is siloed, and patients often disappear between visits, leading to preventable complications and unnecessary hospital load.

The core problem is not the absence of doctors or schemes, but the absence of a continuous triage and coordination layer that can monitor patient risk over time, prioritize attention, and ensure early intervention without overwhelming limited medical resources.


## 2. Objective
The objective of this system is to provide a voice-first, AI-assisted healthcare triage layer that continuously tracks patient symptoms over time and supports timely escalation to appropriate human care. The system is designed to structure symptom input, assess risk conservatively, and ensure follow-up without performing diagnosis or prescribing treatment. By acting as a coordination and risk-visibility layer between patients, frontline health workers, and doctors, the system aims to reduce delayed care while optimizing limited medical resources.


## 3. Target Users
The primary users of the system include individuals from rural and semi-rural communities who face barriers to timely healthcare access, particularly due to distance, language, or literacy limitations.

Secondary users include caregivers and family members who often make healthcare decisions on behalf of patients in the Indian context.

Tertiary users include frontline health workers such as ASHA and ANM staff, as well as doctors at PHC and CHC levels, who receive structured, prioritized cases for review and intervention.


## 4. System Scope
The system provides a voice-first interface for capturing patient-reported symptoms and relevant contextual information, converts this input into structured data, and applies AI-assisted triage logic to assess risk and determine appropriate follow-up or escalation.

The system maintains patient continuity by tracking symptom changes over time and triggering follow-up actions when risk increases or when expected responses are missed.

The system supports escalation workflows to frontline health workers or doctors by presenting prioritized cases with summarized history and symptom trends.

The system does not perform medical diagnosis, prescribe medication, or replace clinical judgment. All medical decisions and treatments remain the responsibility of qualified healthcare professionals.


## 5. Functional Requirements
1. The system shall allow patients, caregivers, or family members to initiate a healthcare interaction through a voice-based interface, such as a phone call or mobile application.

2. The system shall support symptom input through free speech and convert it into structured data fields, including symptom type, duration, severity, and relevant contextual indicators.

3. The system shall ask structured follow-up questions to complete missing or unclear information required for triage.

4. The system shall generate a risk category for each interaction using conservative triage logic, categorizing cases into monitoring, frontline health worker review, or doctor escalation.

5. The system shall store patient interactions with timestamps and track symptom changes over time to identify trends and deterioration.

6. The system shall automatically trigger follow-up interactions based on predefined rules, including symptom persistence, worsening trends, or missed responses.

7. The system shall escalate cases to ASHA or ANM workers when risk thresholds are met or when patient data confidence is low.

8. The system shall escalate cases to doctors at PHC or CHC levels when high-risk conditions or worsening trends are detected.

9. The system shall present escalated cases to healthcare workers with a summarized patient history and symptom trend view.

10. The system shall allow human healthcare workers to review, override, or act upon AI-generated triage suggestions.


## 6. Non-Functional Requirements
1. The system shall prioritize patient safety by using conservative escalation logic and avoiding autonomous medical decision-making.

2. The system shall ensure high availability and reliability to support continuous follow-up and time-sensitive escalations.

3. The system shall support multilingual voice interactions and be designed to extend to additional regional languages without architectural changes.

4. The system shall maintain patient data privacy by collecting only the minimum information required for care continuity and triage.

5. The system shall provide transparency by distinguishing deterministic safety rules from probabilistic AI-assisted assessments.

6. The system shall allow human healthcare workers to override AI-generated triage outputs at any stage.

7. The system shall be designed to function in low-connectivity environments with graceful degradation.


## 7. Out of Scope
The system does not perform medical diagnosis, recommend treatments, or prescribe medications.

The system does not replace qualified healthcare professionals or make final clinical decisions.

The system does not store or process biometric identifiers or government-issued identity documents.

The system does not provide emergency response services such as ambulance dispatch.


## 8. Success Metrics
