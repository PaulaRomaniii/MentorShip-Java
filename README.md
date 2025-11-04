# 🏖️ Vacation Tracking System (VTS)

## 📘 Vision

The main goal of this software is to **simplify HR operations** by minimizing non-core management activities and empowering employees to manage their own vacations efficiently.
It improves internal business processes, reduces HR workload, and speeds up vacation approvals by automating workflows that traditionally required multiple approvals.
The system primarily aims to:

* Save HR department time
* Decrease overall processing time for vacation requests
* Empower employees with self-service capabilities

---

## 👥 Domain

The **Vacation Tracking System (VTS)** operates within the **Human Resources domain**, specifically focusing on employee leave and attendance management.
It serves as a bridge between employees, managers, and HR personnel to handle leave requests, approvals, and balances through a centralized web-based system integrated with existing HR infrastructure.

---

## ⚙️ Functional Requirements

1. Managers can approve or reject employee vacation requests.
2. Employees can view previous requests (within 1 year) and make new requests up to 1.5 years in advance.
3. Automatic email notifications are sent to managers for approvals and to employees for status updates.
4. Supports **single sign-on (SSO)** authentication integrated with existing company systems.
5. Logs all system transactions and activities.
6. HR and Admin users can override actions (all overrides are logged).
7. Managers can award personal leave time to direct employees (within limits).
8. Provides an **API endpoint** for querying employee vacation summaries.
9. Displays multiple vacation categories for employee selection.
10. Allows employees to select vacation types within available balances.
11. Provides a **visual calendar** to select and compare vacation dates.
12. Employees must provide a short title and description with their request.
13. Validates input before submission, showing clear error messages if needed.
14. Integrates with existing HR systems to sync employee data and updates.
15. HR Clerks can add or remove records from the system.
16. HR employees with dual roles must log in using separate IDs.

---

## 🧩 Non-Functional Requirements

1. **Usability:** The system must be intuitive and user-friendly.
2. **Integration:** It will be implemented as an extension to the company’s existing intranet portal.
3. **Scalability:** The system should easily scale to add new features or integrate with related systems.
4. **Performance:** Uses existing company hardware and middleware to ensure reliability and efficiency.

---

## ⚖️ Constraints

* All employees work **8 hours per day**.
* Vacation requests must comply with **location-specific** and **company-wide** policies.
* Validation rules for requests are defined and maintained by the **HR department**.
* Employees cannot take more than **X consecutive days** of a certain vacation type.
* Some vacation types cannot be taken adjacent to official holidays.
* Vacation requests may be rejected if **minimum staffing levels** are not met.
* Certain dates or weekdays may be **restricted** for specific vacation types.

> 🔸 Note: Specific rules and constraints are detailed in the official HR policy documentation.

---

## 🧠 Assumptions

* All employees, managers, and HR staff have access to the company’s internal network.
* The existing company portal supports API and authentication integration.
* Email service is configured for notification functionality.
* HR data in legacy systems is accurate and synchronized.
