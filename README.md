**Author:** Emmanuel E. Imoriafe  
**Date:** 2024-10-11  
**Category:** System Deployment / Digital Transformation  

---

## 1. Objective  

**LabReq Power App** digitizes the laboratory specimen collection process for health assessments, ensuring transparency, automation, and role-based accountability across medical, finance, and laboratory teams.

---

## 2. Value Proposition  

| Key Impact | Outcome |
|-------------|----------|
| Reduced manual processing | 80% faster turnaround for specimen requests |
| Enhanced accuracy | Automated data validation eliminates entry errors |
| Secure user management | Azure AD & RBAC ensure compliance and confidentiality |
| Audit-ready | Automated logs and Power BI reports support oversight |

---

## 3. Architecture Summary  

- **Front-End:** Power Apps Canvas App  
- **Data Tier:** SharePoint List (scalable to Dataverse)  
- **Automation:** Power Automate Flow (Logic + Email Routing)  
- **Web Tier:** Azure Web Services (App Service, Logic Apps)  
- **Security:** Azure AD Single Sign-On (SSO) with Role-Based Access Control (RBAC)  


graph LR
    Doctor -->|Submit Request| PowerApp
    PowerApp -->|Write Data| SharePoint
    PowerApp -->|Trigger Flow| PowerAutomate
    PowerAutomate -->|Email Notification| Finance
    Finance -->|Verify Payment| SharePoint
    PowerAutomate -->|Authorize| SpecimenTeam
    SpecimenTeam -->|Complete Task| SharePoint
    SharePoint -->|Sync Reports| ProgramManager

<img width="853" height="637" alt="image" src="https://github.com/user-attachments/assets/aa8390ba-7cb4-460e-bc96-6fa9bcae087d" />

<img width="804" height="395" alt="image" src="https://github.com/user-attachments/assets/d48b4c82-daad-418e-ae8c-ae1386deb266" />

<img width="837" height="677" alt="image" src="https://github.com/user-attachments/assets/704ef856-2b99-4c37-8ea5-0b59f13539ff" />

<img width="911" height="548" alt="image" src="https://github.com/user-attachments/assets/e7ff2843-f15e-46ec-aaed-a5d0b096647e" />









