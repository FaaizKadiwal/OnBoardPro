# OnBoardPro – Employee Onboarding Management App

OnBoardPro is a **Model-Driven Application** built using **Microsoft Power Platform** to streamline and manage the employee onboarding lifecycle. It allows organizations to manage projects, tasks, equipment, and access rights while automating key administrative processes using Power Automate and Business Rules.

---

## 📌 Project Overview

- **Platform:** Microsoft Power Apps (Model-Driven App)
- **Automation:** Power Automate & Business Rules
- **Data Layer:** Dataverse Tables
- **Security:** Role-Based Access (Admin)
- **Reports & Dashboards:** Interactive insights via built-in components

---

## 🎯 Core Features

| Module           | Functionality                                                                 |
|------------------|-------------------------------------------------------------------------------|
| FK_Employee      | Manage employee records, joining dates, job roles, and related assignments   |
| FK_Project       | Assign onboarding projects with automated timelines and linked tasks         |
| FK_Task          | Define onboarding tasks with due dates auto-calculated by flows              |
| FK_Equipment     | Assign devices to employees with auto-filled issue dates                     |
| FK_AccessRights  | Manage system access credentials and notify users via email automation       |

---

## 🚀 Automations & Business Logic

- **Power Automate Flows:**
  - Auto-set `dueDate` (FK_Task) = project start date + 7 days
  - Auto-fill `joiningDate`, `issuedDate`, `endDate` with today/date logic
  - Email notification upon access rights assignment

- **Business Rules:**
  - Validate joiningDate is not in the past
  - Block past dueDate in tasks
  - Set default values dynamically

---

## 📊 Dashboards & Reports

- **Dashboard:** `OnBoardPro Overview`
  - Tasks by Status (Chart)
  - Projects by Department (Chart)
  - Equipment by Type (Chart)
  - Active Employees (List)

- **Report:** `Pending Tasks by Project`
  - Filterable and integrated via FK_Task

---

## 🧱 Data Modeling (ERD)

- One FK_Employee → Many FK_Projects
- One FK_Project → Many FK_Tasks
- One FK_Employee → Many FK_Equipments
- One FK_Employee → Many FK_AccessRights

---

## 🧩 Solution Architecture

- Built in Microsoft Dataverse
- Integrated Power Automate Flows
- Dashboards and Views for dynamic UX
- Modular design for reusability across departments

---

## ✅ Business Value

- **Improved Efficiency:** Automated form filling and scheduling reduce human error
- **Access Control:** Role-based and email-driven access assignment
- **Real-time Monitoring:** Dashboards help track KPIs and onboarding status
- **Reusability:** Modular architecture supports extension to other HR processes
- **User Notifications:** Email confirmations enhance communication

---

## 📁 Repository Contents

| File/Folder              | Description                                        |
|--------------------------|----------------------------------------------------|
| `/snapshots/`            | Screenshots of forms, dashboards, ERD, and flows   |
| `OnBoardPro_Export.zip`  | Full Power Platform solution file                  |
| `OnBoardPro_Report.pdf`  | Final project documentation                        |
| `OnBoardPro_Presentation.pptx` | Final slide deck                          |

---

## 📬 Contact

For queries or demo access, please reach out to:  
📧 faaiz12rahim@gmail.com  
🔗 [LinkedIn: faaiz-kadiwal](https://www.linkedin.com/in/faaiz-kadiwal-a872942b9/)  

---

