---
layout: default
title: Introduction & Implementation of SystmOne
parent: Introduction
nav_order: 1
---

# CHAPTER 1: SystmOne Implementation Documentation  `Ver 1.0`{: .label }
{: .no_toc }

<details open markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

KK Bandar Maharani CCMS Documentation & Protocol

Created by: DR. MUHAMMAD FUAD BIN JAAFAR (PKDMUAR), Last Update: 15 May 2025 22:58

This chapter outlines the full implementation journey of SystmOne (CCMS) at Klinik Kesihatan Bandar Maharani, including planning, system rollout, staff engagement and custom configuration done to suit clinic workflows.


## Section 1.0 Introduction to SystmOne

SystmOne is a comprehensive clinical computer system developed by TPP (The Phoenix Partnership), a UK-based healthcare IT company. It has been in use in the United Kingdom since the early 2000s and is widely deployed across general practices, community services, mental health services, and hospitals. As of 2024, SystmOne is used by approximately 40% of GP practices in England, playing a major role in integrated care delivery within the NHS. Its cloud-based architecture enables seamless sharing of patient information across different healthcare providers, promoting continuity of care.

### 1.1 Introduction to Cloud-Based Clinic Management System (CCMS)

The Cloud-Based Clinic Management System (CCMS) project is an initiative under the Ministry of Health Malaysia (MOH), driven by the Digital Health Division (Bahagian Kesihatan Digital - BKD) and the Health Informatics Centre (Bahagian Pengurusan Kesihatan Awam - BPKA). The CCMS aims to modernize clinic management through cloud technology, offering centralized data access, real-time patient management, and secure information handling.

The CCMS project commenced in early 2023, with Klinik Kesihatan Sg Chua and Klinik Kesihatan Botanik selected as pioneer sites. Following the success of the pilot phase, the project expanded around August-September 2023 to 50 more Klinik Kesihatan nationwide. In Johor, five clinics were selected, including Klinik Kesihatan Bandar Maharani (KKBM), making it one of the earliest adopters of SystmOne under the CCMS program.

### 1.2 🌟 Importance and Benefits of CCMS Implementation

The implementation of CCMS represents a major milestone in digitalizing Malaysia's primary healthcare services. Its key benefits include:

Centralized and Real-Time Access: Enables healthcare providers to access and update patient records instantly, improving coordination and reducing duplication of care.

Enhanced Patient Safety: Standardized documentation, automated alerts, and structured workflows help reduce errors and ensure adherence to clinical guidelines.

Improved Operational Efficiency: Streamlines registration, consultation, investigation, and follow-up processes, leading to shorter patient wait times and faster service delivery.

Data Security and Compliance: Strengthens data protection through cloud-based secure storage, role-based access, and audit trails in line with national ICT security policies.

Scalability and Integration: Supports future integration with other health information systems (e.g., iLAB, PHIS), ensuring a sustainable digital health ecosystem.

### 1.3 🧩 Holistic Patient Management Under CCMS

The Cloud-Based Clinic Management System (CCMS) supports an integrated approach to patient care by unifying multiple clinical processes into a single system. Key components include:

Patient Registration: Basic demographic details are recorded only once at the point of first registration. This eliminates the need for repeated data entry across different units or visits, ensuring continuity and data consistency throughout the patient’s care journey.
[image]

Consultation & Treatment Records: Every patient encounter is documented in a structured format that includes presenting complaint, history, diagnosis, management, and outcome.

Laboratory & Radiology Integration: Lab and imaging results are directly linked to the patient's record, providing clinicians with timely access to investigations.

Service-Based Registration: Patients are registered according to the type of service they require (e.g., KKIA, NCD, TB).

E-Prescription Integration (PHIS): Medication prescriptions are processed electronically and synced with the Pharmacy Information System (PHIS).

Appointment Management: Appointments are managed digitally, allowing for scheduling, tracking, and reminders.

Data Analytics, Reten & Reporting: Automated generation of clinical and service statistics for audit and reporting.

Data Standardization via SNOMED CT and ICD-10 Integration: SystmOne uses SNOMED CT codes mapped to ICD-10 for consistent, internationally recognized documentation across all units. SNOMED CT is applied comprehensively across all aspects of patient data documentation within SystmOne — including diagnoses, symptoms, procedures, assessments, and clinical observations. This ensures structured, interoperable data that supports high-quality patient care, accurate coding, and compatibility with national and international health data systems. The use of SNOMED CT not only aligns with Malaysia’s digital health vision but also supports future integration with global data analytics and research platforms.

## Section 2.0 – Scope of Implementation 🏥

SystmOne was fully implemented across all major clinic units:

Jabatan Pesakit Luar (JPL) – Outpatient

Maternal & Child Health (MCH) Unit

NCD Unit (Diabetes, Hypertension, Asthma, Mental Health)

TB Clinic

Methadone Clinic

Quit Smoking Clinic

STD and HIV Clinic

Health Screening and Wound Care

Radiology (X-Ray) Unit (linked indirectly; images stored in Orthanc PACS)
[image]

Laboratory Unit (in progress: iLAB integration)

Other special services: Dietitian, Nutritionist, Physiotherapy

## Section 3.0 – CCMS/SystmOne Implementation Timeline at KK Bandar Maharani

### 3.1 🧭 Pre-Implementation Milestones (Aug–Sept 2023)

29 Aug 2023 – Initial CCMS briefing by BKD & JKN Johor at Klinik Kesihatan Muar, joined by MOIC KK Maharani, Dr Zurina and Dr Fuad.

12 Sept 2023 – Site readiness visit by JKNJ Unit Pengurusan Maklumat to assess network, asset readiness & infrastructure.

18 Sept 2023 – System implementation & on-site training at KKBM conducted by BKAD & SystmOne UK (2-day session).

27 Sept 2023 – Visit to pioneer clinic KK Sg Chua, Selangor to observe real-world CCMS operation.

### 3.2 🧩 Internal Phase-by-Phase Implementation (Sept 2023 – Ongoing)

19 Sept 2023 – CCMS activated in: Registration Counters, OPD Doctor Rooms, NCD, FMS Rooms, Procedure & Dressing Rooms.

Oct–Nov 2023 – X-ray unit digitalized using Orthanc PACS Server.

Feb 2024 – ECG, Fever Clinic, KKIA Unit, KBM Methadone services onboarded.

Mar–May 2024 – Reten forms for Primary Care & NCD audits standardized and implemented in SystmOne.

May 2024 – Integration of PHIS–CCMS for e-prescription (effective 21 May 2024).

June 2024 – Workflow updates in KKIA & OPD; planning integration with other special service units.

Sep–Nov 2024 – Pilot integration project with iLAB system initiated at KKBM.

This timeline highlights a structured and progressive rollout of CCMS at Klinik Kesihatan Bandar Maharani, balancing rapid implementation with training, service-specific onboarding, and integration with existing health IT infrastructure.

## Section 4.0 – Orthanc PACS Implementation at Klinik Kesihatan Bandar Maharani

One of the significant milestones achieved during digital transformation at KK Bandar Maharani is the successful implementation of the Orthanc PACS (Picture Archiving and Communication System) for managing radiology images. This initiative was spearheaded by Dr. Fuad following consultation with YM Dr. Zurina and Pn Noraini (Head Radiographer, PKD Muar) to enhance X-ray data access and promote cost-saving through in-house PACS infrastructure.
[image]

### 4.1 Implementation Background

Initiated in Oct–Nov 2023, this PACS system was configured and deployed internally by Dr. Fuad.
[image]

Implementation was supported by official Orthanc documentation, online forums, and open-source community guidance.

The system enables all X-ray images to be stored, retrieved, and reviewed digitally without reliance on physical films or third-party cloud services.
[image]

### 4.2 Hardware & Infrastructure Requirements

A dedicated workstation/server PC with adequate storage (for image archiving
