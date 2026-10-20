# Salesforce Enterprise Case Management & Support Hub

##  Project Overview
This project simulates an enterprise-grade Customer Service and IT Helpdesk implementation on the Salesforce Platform. The solution is designed to streamline customer support operations, automate case routing based on priority, and provide leadership with real-time operational metrics via custom reports and dashboards.

---

##  Architecture & Data Model
* **Core Standard Objects:** Accounts, Contacts, Cases, and Assets.
* **Custom Objects:** 
  * `IT Equipment Request__c` (Tracks internal hardware and software deployment requests).
* **Data Relationships:** Master-Detail and Lookup relationships connecting requests and assets directly to customer Accounts and individual Contacts.

---

##  Security & Access Control
* **Profiles & Permission Sets:** Configured granular access separating standard support agents from IT administrators and executive managers.
* **Role Hierarchy:** Established a reporting structure ensuring regional support teams only view cases relevant to their specific business units.
* **Sharing Rules:** Implemented criteria-based sharing rules to securely expose sensitive hardware asset data to authorized internal personnel.

---

##  Process Automation & Flow Builder
* **Automated Case Assignment:** Created a record-triggered Flow to automatically assign incoming high-priority IT requests to the Senior Support Queue.
* **SLA Alerts:** Configured scheduled paths within Flow Builder to trigger automated warning emails to case owners if a critical issue remains unresolved after 4 hours.
* **Status Updates:** Automated field updates to stamp closure timestamps whenever a case moves to the "Closed-Resolved" stage.

---

##  Reporting & Analytics
* **Support Dashboard Metrics:**
  * *Open Cases by Priority* (Donut chart tracking High, Medium, and Low urgency items).
  * *Average Resolution Time by Agent* (Performance metric tracking efficiency).
  * *First-Contact Resolution Rate* (KPI tracking initial resolution success).

---

##  Skills Demonstrated
* Salesforce Administration & Declarative Development
* Custom Data Modeling & Relationship Architecture
* Advanced Process Automation (Flow Builder)
* Declarative Security (Profiles, Roles, and Sharing Rules)
* Business Intelligence (Reports & Dashboards)
