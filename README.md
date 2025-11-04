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


<img width="975" height="661" alt="image" src="https://github.com/user-attachments/assets/b06dfec3-b9b9-4249-bde1-e42fbe3b5a9d" />

<img width="975" height="521" alt="image" src="https://github.com/user-attachments/assets/37e3884a-32a9-495b-8dc7-1eda0bca8d65" />

<img width="975" height="614" alt="image" src="https://github.com/user-attachments/assets/d3957f98-dcc0-4a50-84e9-a25766511dfa" />

<img width="975" height="588" alt="image" src="https://github.com/user-attachments/assets/b7a52b3b-b47c-4c47-8a71-d06f3d09bbb9" />

<img width="975" height="673" alt="image" src="https://github.com/user-attachments/assets/1c32d8e6-b374-45d0-a24d-4b8cc60dee10" />

<img width="975" height="541" alt="image" src="https://github.com/user-attachments/assets/9f7ef24e-bf09-46a9-ad2d-3550ac32190a" />




 

 
 
 

 
 










