---
layout: default
title: Introduction & Implementation of SystmOne
parent: Introduction
nav_order: 1
---

# CHAPTER 1: SYSTMONE IMPLEMENTATION DOCUMENTATION  Ver 1.0

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

A dedicated workstation/server PC with adequate storage (for image archiving).
[image]

Orthanc software (open-source) installed on Windows OS.

Integrated with existing clinic infrastructure via GITN network, ensuring secure connectivity between Radiology and other clinical units.

### 4.3 Data Security and Privacy

Orthanc offers robust access control, audit logging, and user-level permission settings to restrict and monitor access to imaging data.

Only authorized personnel are allowed to access, view, or retrieve radiology studies.

The server is hosted entirely on-premise at KK Bandar Maharani, ensuring no cloud storage or third-party data sharing, in full alignment with the Ministry of Health’s ICT Security Policy (Version 5).

Orthanc also supports encryption at rest and in transit and can be configured to comply with international security standards.
[image]

Notably, Orthanc is compliant with the DICOM (Digital Imaging and Communications in Medicine) standard and is HIPAA-ready when configured appropriately, supporting essential requirements for healthcare data confidentiality, integrity, and auditability.
[image]

### 4.4 🌐 Network Integration

Orthanc PACS runs entirely over the GITN-provided ISP, with all clinic units connected via the same secure LAN network.

This design allows clinicians across different units to easily view imaging data in real time using browser-based access.

### 4.5 Stability and Impact

Since its implementation, the system has been operating stably with minimal issues.

It has significantly improved workflow in the Radiology Unit and reduced reliance on manual film distribution, supporting KKM’s broader digitalisation goals.

This Orthanc PACS project stands as a successful local innovation, reflecting KK Bandar Maharani’s proactive approach in modernizing clinical services through scalable, cost-effective technology solutions.

## Section 5.0 – ECG Recording Integration 🫀

Klinik Kesihatan Bandar Maharani has also begun the digitalization of ECG recording workflows.

Two ECG machines in the clinic are equipped with Wi-Fi capabilities, allowing them to send ECG traces via local FTP server directly to a central ECG PC.

From there, the staff in charge convert the ECG data into PDF format and upload the files into each patient’s profile in SystmOne.

While the process is not fully integrated within the CCMS ecosystem, this approach eliminates the need to print physical ECG records.

Clinicians can access the digital ECG as an attachment within the patient's SystmOne record, promoting paperless documentation and faster review.

## Section 6.0 – Staff Training & Capacity Building

As part of the SystmOne implementation, training and capacity-building efforts were conducted to ensure smooth adoption and confident use of the system across all units of Klinik Kesihatan Bandar Maharani.

Training included registration staff, nurses, medical assistants, doctors, and allied health personnel. Sessions covered clinical documentation, template usage, e-prescription, and workflow optimization.

Note: Detailed training logs, session dates, and participant records are maintained in a separate documentation file titled “CCMS Training Records – KKBM”.

### 6.1 Competency Tracking Status

Current Status: No formal competency evaluation yet.

Future Plan: Development of a structured competency checklist for different staff categories is under discussion among the clinic management team.

### 6.2 Ongoing Support & Digital Resources

Training guides, template examples, and Reten references are being organized under a separate documentation module for staff reference and future onboarding.

## Section 7.0 🌐 Internet & Network Infrastructure Expansion for CCMS

Prior to August 2023, Klinik Kesihatan Bandar Maharani operated with a conventional local area network (LAN) setup with only one LAN port available in each room. There was no Wi-Fi coverage, and connectivity was limited to wired access, restricting multi-user environments—especially in shared spaces like consultation rooms, procedure rooms, and registration counters.

The introduction of CCMS necessitated dedicated PC or laptop access for each staff member, creating an urgent need to expand internet access through wireless networking.

### 7.1  Early Network Review and Recommendations

On 12 September 2023, the JKNJ Unit Pengurusan Maklumat visited the clinic and recommended the installation of Access Point (AP) routers to enable wireless access where LAN ports were insufficient.

### 7.2  Deployment Timeline & Device Setup

Sept 2023: First AP Router installed — Ruijie EW1800-GX Wi-Fi 6 deployed near Room 1 OPD

Jan 2024: Second Ruijie Wi-Fi 6 Router installed near Bilik 21 (KKIA Unit) to cover KKIA and nearby Fever Unit.

### 7.3  Network Optimization Phase 🛜

Due to weak signal stability in the KKIA and Fever Unit zones

A Tenda Nova MX3 Mesh system (2 units) was installed in Bilik 22 & 25 to enhance coverage.

A dedicated Tenda AC1200 router was later installed exclusively for the Fever Unit.

The second Ruijie router is currently planned to be repositioned to serve the Registration Counter (B01–B08) and surrounding area for stable front-desk operations.

### 7.4  Backup Internet Service 🌐

A free backup internet line (Unifi) was installed in the server zone, provided by Telekom Malaysia (TM) Muar), to ensure service continuity during GITN service interruptions.

### 7.5  Security Controls and MAC Whitelisting 🔑

To protect CCMS bandwidth and prevent unauthorized access:

Each router uses MAC address whitelisting — Only pre-registered clinic devices are allowed to access Wi-Fi.

This ensures that even with password knowledge, non-whitelisted devices cannot access the network, preserving bandwidth integrity and service quality for CCMS usage.

This network upgrade strategy ensured comprehensive connectivity for all CCMS-enabled devices while maintaining security, stability, and centralized access throughout the clinic's departments.

## Section 8.0 ⚙️ Customizations Done

The following key customizations were implemented to align SystmOne with Klinik Kesihatan Bandar Maharani’s clinical, operational, and audit needs:

### 8.1  Clinical Templates

Customized templates created for major clinic services: NCD, TB Clinic, Fever Clinic, KKIA (Antenatal), and Health Screening.

Templates designed according to CPG standards & JKN requirements

Mandatory fields enforced for complete documentation.

### 8.2  Reten and Data Reporting 📈

Reten forms created within SystmOne for monthly and quarterly MOH data reporting.

While the BKD and TPP teams have developed clinical Reten reports at the national (MOH) level, the clinic also faces requirements for additional reports tailored specifically to the needs of the State Health Department (JKN) and District Health Office (PKD).

These local-level reporting needs include service-specific performance metrics, targeted patient group statistics, and operational audit indicators that are not always captured in national reports. To address this, KKBM has developed supplemental custom forms within SystmOne to fulfill district and state audit requirements:

NCD clinical reporting: diabetes, hypertension, dyslipidemia, mental health etc.

Health screening reporting: BSSK, NHSI, peka b40 etc
Special services reporting: Quit Smoking Clinic retens, Virtual Consultation retens etc.

### 8.3  Workflow Design 🔁

Auto-allocation rules at registration (e.g., OPD, KKIA).

Custom patient flow protocols for TB, Methadone, and NCD.

Workflow design mainly involved restructuring and upgrading the clinic’s existing patient flow to be aligned with the system usage & requirements of SystmOne.

Many of the previous workflows were built around paper-based or hybrid systems and required significant adaptation to fully utilize the benefits of a centralized electronic medical record (EMR) platform.

The goal was to design streamlined, unit-specific processes that facilitate seamless documentation, minimize duplication, and improve service efficiency.

This redesign was particularly essential in units such as NCD, KKIA, special services, wound care and TB clinics where documentation and follow-up are complex.

For detailed breakdowns of the redesigned patient journey, refer to the separate documentation on Patient Flow Optimization at KKBM.

### 8.4  Protocol-Based Alerts 🚨

Automatic and protocol-based alerts have been developed to support proactive clinical management. These include:

Overdue NCD Follow-ups: Alerts for diabetic patients who have not received an HbA1c test within the past 6 months.

Screening Reminders: Automated reminders for erectile dysfunction (ED) screening in eligible male patients and prompts for comprehensive health screenings.

Vital Sign Abnormalities: Real-time alerts for abnormal blood pressure and heart rate readings.

Travel-Based Fever Alerts: Triggers based on travel history to flag potential cases of dengue, MERS-CoV, and other febrile illnesses.
Pediatric Medication Protocols: Protocol-based calculators have been implemented for common pediatric medications to ensure correct dosage and documentation.

Workflow and SOP Adherence: Protocols are also used to enforce SOP compliance, guide clinicians through standardized workflows, and ensure alignment with national clinical practice guidelines.

### 8.5 📊 Real-Time Dashboards

Summary of visualisation and dashboard created:

Summary for maternal health condition during antenatal and postnatal

Summary for child routine assessment in the clinic

Summary dashboard of screening & procedure metrics done in the clinic

Summary of specific maternal screening done during antenatal period

Individual health screening summary done for each patient

NCD Management progress and monitoring

### 8.6 📄 Custom Word Templates

Built-in printable documents include:

Health Screening Summary Letter

Methadone Programme Agreement

TB Notification Report

STD/HIV Risk Report

These enhancements allow the clinic to maintain high standards in digital documentation, audit readiness, and structured service delivery.

## Section 9.0 🔍 Limitation and Current Challenges

Despite the successful implementation of SystmOne and CCMS at Klinik Kesihatan Bandar Maharani, several limitations and challenges remain:

iLAB System Integration Pending:

Full integration of laboratory data into SystmOne is still under pilot phase and not yet fully operational.

Current state: staff manually insert laboratory data into SystmOne to ensure accurate clinical reporting, enable effective data analysis, and support better patient management decisions.

Manual Workflow for ECG Uploads:

While ECG recordings are digitalized, the upload process remains semi-manual, requiring staff to transfer and attach PDFs manually into SystmOne.

The clinic can currently manage with this setup as it is not overly burdensome for staff; however, a more integrated solution would be ideal in the future to improve efficiency.

No Formal Competency Evaluation Yet:

Although internal training has been conducted, there is currently no formal system to certify or assess staff competency in SystmOne usage.

Orthanc PACS Backup:

The current PACS server is locally hosted without external cloud backup.

To strengthen data resilience, there are plans to implement a secondary local Orthanc backup server within the clinic itself.

No migration to cloud-based backup is planned at this stage.

Internet Stability in Peripheral Areas: Some peripheral zones (e.g., Fever Unit, external consultation rooms) still experience occasional instability despite Wi-Fi expansion.

Continuous Staff Turnover:

One of the most impactful challenges faced during the SystmOne implementation was the reassignment of trained personnel.

In January 2025, approximately 6–8 senior Medical Officers who had been trained extensively over more than a year were transferred out of the clinic under instructions from PKD Muar. These Medical Officers also served as the heads of their respective clinical units, and their presence was significant in sustaining daily operations and digital workflows. They played critical roles not only in system usage but also in designing efficient workflows aligned with SystmOne documentation standards.

Their sudden departure significantly disrupted the progress and momentum that had been built, especially as KKBM serves as the pioneer CCMS clinic in the district. This situation underscores the need for stronger communication and coordination between administrative authorities and implementation teams. Ensuring continuity of trained personnel is vital to safeguard the integrity and effectiveness of digital health transformation efforts at the clinic level.

E-Prescription Partial Implementation:

While MOH aims for a fully paperless e-prescription workflow, KKBM currently implements a semi-paperless system.

For acute cases with no follow-up, prescriptions are handled fully paperless within SystmOne.

However, for chronic cases requiring long-term medication monitoring, physical slips are still printed for continuity of care and medication review purposes.

Aging ICT Hardware Infrastructure: A significant portion of ICT assets used to support CCMS functions at Klinik Kesihatan Bandar Maharani consists of older hardware. Many desktop PCs, network devices, and peripherals have reached or are approaching end-of-life status. This affects system speed, reliability, and user experience. Upgrading and replacing these assets has become one of the clinic’s most pressing challenges, requiring dedicated budget allocation and procurement support to ensure sustainable CCMS operations.

Acknowledging these limitations allows the clinic to continuously plan for improvements and risk mitigation to enhance system maturity and operational resilience.

## Section 10.0 🚀 Future Plans and Roadmap

Moving forward, Klinik Kesihatan Bandar Maharani is committed to further enhancing the robustness, efficiency, and scalability of the SystmOne and CCMS implementation. Planned initiatives include:

iLAB System Full Integration: Completion of the pilot project and direct integration of laboratory results into SystmOne to allow seamless lab reporting.

Secondary Local Orthanc PACS Server: Setting up a backup PACS server within the clinic to strengthen data security and ensure high availability.

Formal Competency Assessment Framework: Development and implementation of structured competency checklists for different staff categories to standardize and evaluate CCMS usage skills.

Continuous System Refinement: Ongoing optimization of templates, workflows, and data analytics dashboards based on user feedback and audit findings.

Expanded Digitalization Efforts: Incorporation of additional digital records such as wound care documentation, procedure photography, and physiotherapy assessments.
[image]

Enhanced Training and Refresher Programs: Regular CME sessions, internal refreshers, and onboarding programs for new staff to maintain high competency levels.

Network and Infrastructure Enhancement: Further reinforcement of Wi-Fi coverage in peripheral zones and evaluation of backup internet system upgrades.

These planned actions demonstrate the clinic’s commitment to maintaining high standards of digital healthcare delivery, ensuring sustainability, and supporting national digital health transformation goals.

## Section 11.0 📦 ICT Asset & System Infrastructure Reference

To support SystmOne operations, Klinik Kesihatan Bandar Maharani maintains a complete inventory of ICT hardware and networking assets including:

Desktop PCs and Laptops for each clinical room

Orthanc PACS server hardware

GITN-connected routers and AP systems

ECG machines (Wi-Fi enabled)

The full inventory with asset IDs, location tags, and technical specifications is maintained in a separate document titled “KKBM ICT Asset Register”.

## Section 12.0 🛠️ Helpdesk and Support System

### 12.1 🏢 Central Support from BKD & TPP (MOH Level)

At the central level, support for CCMS and SystmOne implementation is coordinated by the Digital Health Division (BKD) and TPP Malaysia team. Currently, there is no dedicated website, formal helpdesk portal, or ticketing system established for technical support.

Instead, support is actively managed through a dedicated "CCMS Helpdesk" WhatsApp group, where each Klinik Kesihatan has designated representatives.

Through this group:

Clinic staff can raise system issues, questions, and enhancement requests.

BKD and TPP officers respond either directly in the group or via personal messaging or phone calls.

All troubleshooting, feedback, and system support activities are conducted remotely.

While the use of a WhatsApp-based support system reflects a practical and immediate-response approach, it is acknowledged that future developments may benefit from a more structured ticketing or reporting platform as CCMS expands nationwide.

The current support framework emphasizes rapid communication and direct engagement, aligning with the cloud-based nature of the CCMS platform.

### 12.2 🏥 Internal Support System at Klinik Kesihatan Bandar Maharani (Local Level)

Recognizing the need to complement the national-level support system with a formal local mechanism, Klinik Kesihatan Bandar Maharani has developed an internal helpdesk platform: “Muar ICT Helpdesk” (developed using AppSheet).

#### 🌟 Key Features of Muar ICT Helpdesk:

Multiple Submission Options: Users can submit issues either through Google Form (linked to the app) or directly within the AppSheet mobile application.

Formal Report Tracking: Reports are categorized by issue type, criticality level, and assigned root cause. Staff can update progress status and resolution notes directly in the app.

Notifications and Feedback: Email notifications are automatically sent to users after report submission.

Monthly and Individual Reporting: Users can generate comprehensive monthly helpdesk reports or individual incident reports in PDF format.

Report & Ticketing ID: Each report submitted through the Muar ICT Helpdesk system is automatically assigned a unique Report or Ticketing ID. This ensures traceability, allows for efficient tracking of progress and follow-up & supports audit readiness through unique case referencing.

Knowledge Base Initiatives: An FAQ and User Guide section has been recently introduced (currently under expansion) to facilitate self-help for common issues.

ISO Audit Alignment: The helpdesk system was developed in response to internal ISO audit recommendations highlighting the need for better documentation and traceability of ICT and system-related issues.

Through this system, Klinik Kesihatan Bandar Maharani ensures that all technical concerns, system issues, and improvement requests are systematically documented, tracked, and managed — supporting a culture of continuous improvement and operational excellence.
