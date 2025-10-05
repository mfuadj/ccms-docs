---
layout: default
title: CCMS Basics
parent: Introduction
nav_order: 3
---

# CCMS Basics

This page is a dummy example to demonstrate headings, lists, tables, images, callouts, and links.

## What is CCMS?

The Clinical Care Management System (CCMS) helps care teams coordinate patient care, document interventions, and track outcomes.

> Note: Content on this page is sample text only.
{: .note }

## Key Concepts

- Patients
- Encounters
- Care Plans
- Tasks
- Alerts

### Roles

1. Care Manager
2. Clinician
3. Administrator

## Workflow at a Glance

1. Register patient
2. Triage using intake form
3. Create care plan
4. Assign tasks
5. Review outcomes

> Warning: Always validate patient identifiers before creating a new encounter.
{: .warning }

## Data Entities

| Entity      | Description                               | Example              |
|------------|-------------------------------------------|----------------------|
| Patient     | Person receiving care                     | Jane Doe             |
| Encounter   | Interaction between patient and provider  | Intake 2025-01-04    |
| Care Plan   | Structured plan of interventions          | Diabetes Mgmt Plan   |
| Task        | Action item assigned to a role            | Follow-up call       |

## Sample Snippets

JSON example:
```json
{
  "patientId": "P-12345",
  "encounterType": "intake",
  "priority": "high"
}
```

Shell example:
```bash
# This is illustrative, not a real endpoint
curl -H "Authorization: Bearer <token>" https://api.example.com/ccms/patients/P-12345
```

## Links

- See the [Overview]({{ '/docs/introduction/overview' | relative_url }})
- Jump to [Triage workflow]({{ '/docs/workflows/triage' | relative_url }})
- Browse the [Data Model]({{ '/docs/reference/data-model' | relative_url }})

## Images (optional)

![Placeholder diagram]({{ '/assets/images/placeholder-diagram.png' | relative_url }})

> Tip: Add your image under `assets/images/placeholder-diagram.png` and update the file name above.
{: .tip }

## Page Sections and Anchors

You can deep-link to any heading. For example, this section’s anchor is `#page-sections-and-anchors`. Link format:
`{{ '/docs/introduction/ccms-basics#page-sections-and-anchors' | relative_url }}`

## Next Steps

- Continue with [Getting Started]({{ '/docs/introduction/getting-started' | relative_url }})
- Or go back to the [Introduction]({{ '/docs/introduction/' | relative_url }})
