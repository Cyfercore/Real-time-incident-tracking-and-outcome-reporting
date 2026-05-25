# Real-time-incident-tracking-and-outcome-reporting
A real‑time emergency incident analytics system with automated data pipelines and interactive dashboards for monitoring response performance, patient outcomes, and operational efficiency.
This project implements a real-time emergency incident tracking and outcome reporting system for HealthResponse Ltd. It automates data collection using Microsoft Forms and Power Automate, stores structured incident logs in Google Sheets, and visualises operational performance through Looker Studio dashboards.

## ⚠️ Operational Problem

HealthResponse Ltd needed a reliable way to track emergency incidents from the moment they were reported to the moment the patient outcome was recorded. The existing workflow relied on a mix of manual logging, delayed updates, and disconnected tools, which created several operational issues:

- **Incident data was being captured manually**, often across different systems, leading to delays and inconsistencies.  
- **No real-time visibility** existed for managers to monitor active incidents, response times, or team performance.  
- **Patient outcomes were not tracked in a structured way**, making it difficult to analyse the effectiveness of interventions.  
- **Reporting was slow and reactive**, requiring manual aggregation at the end of the day or week.  
- **Operational decisions were being made without live data**, limiting the ability to allocate resources efficiently during peak demand.  

These gaps made it difficult for HealthResponse to maintain high response standards, monitor service quality, and identify trends that could improve patient care.


## 📦 Deliverables

This project produced a fully operational, end‑to‑end incident tracking and reporting system designed to support real‑time decision‑making at HealthResponse Ltd. The key deliverables include:

### 1. Real-Time Incident Intake Form (Microsoft Forms)
A structured digital form used by responders to log emergency incidents consistently and accurately at the point of contact.

### 2. Automated Data Pipeline (Power Automate)
A workflow that transfers submitted incident data directly into a centralised Google Sheets database, eliminating manual entry and ensuring real-time updates.

### 3. Centralised Incident Database (Google Sheets)
A live, structured dataset that stores all incident records, outcomes, timestamps, and operational details used for reporting and analysis.

### 4. Multi‑Page Looker Studio Dashboard
A set of interactive dashboards providing real-time visibility into:
- Incident volumes and trends  
- Response performance  
- Patient outcomes  
- Regional activity  
- Intervention effectiveness  
- SLA compliance  

### 5. KPI Monitoring Framework
Defined and implemented key operational metrics such as response time, escalation rate, priority distribution, and outcome categories to support performance tracking.

### 6. Operational Reporting Layer
A unified reporting environment enabling managers to monitor live incidents, identify bottlenecks, and make informed decisions during peak demand.


## 🏗️ System Architecture

The system is built as a lightweight, real‑time operational pipeline that connects data collection, automation, storage, and reporting into a single workflow. The architecture ensures that incident data flows seamlessly from frontline responders to management dashboards without manual intervention.

Microsoft Forms  
        ↓  
Power Automate (Automated Workflow)  
        ↓  
Google Sheets (Centralised Real‑Time Database)  
        ↓  
Looker Studio (Interactive Dashboards & Reporting)
### 🔍 Component Breakdown

**1. Microsoft Forms – Incident Intake**  
Frontline responders submit incident details through a structured digital form, ensuring consistent and accurate data capture.

**2. Power Automate – Data Pipeline Automation**  
An automated workflow processes each form submission and writes the data directly into Google Sheets in real time.

**3. Google Sheets – Operational Data Store**  
Acts as the centralised, always‑up‑to‑date database for all incident records, outcomes, timestamps, and operational fields.

**4. Looker Studio – Real‑Time Dashboards**  
Dashboards connect directly to the live dataset, providing managers with instant visibility into incident activity, response performance, patient outcomes, and regional trends.

## 📺 Dashboards

The reporting layer is built in Looker Studio and is organised into multiple pages to support different operational views.

### 1. Executive Overview – Dashboard Summary

This **Executive Overview** dashboard provides a real‑time snapshot of emergency incident activity and operational performance. It highlights overall workload, response efficiency, case severity, and team performance so decision‑makers can understand system pressure at a glance and also shows the high‑level view of overall incident activity, response metrics and escalation.

> Suggested use: For managers and leadership to monitor live performance and identify pressure points.



<img width="1878" height="1056" alt="executive dashboard" src="https://github.com/user-attachments/assets/047ffc6d-e9c6-4508-966a-e4ecd99d16f5" />

### Key Insights
- **Total Incidents: 3,000** — steady activity across all months, showing consistent service demand.
- **Average Response Time: 37.83 minutes** — strong performance on **Critical** cases (14 mins), but delays on **Low** (89 mins) and **Medium** (49 mins) priorities.
- **Critical Incidents: 607** — sustained high‑risk workload indicating clinical pressure.
- **Escalation Rate: 36.43%** — over one‑third of cases required higher‑level support, signalling rising case complexity.
- **Incident Types** — Mental Health Crisis and Panic Attacks are the most common categories, each reaching 503 cases.
- **Priority Mix** — High (1.1K) and Medium (996) priorities dominate the workload.
- **Response Modes** — Field Visits (32.5%) and Ambulance Dispatch (29.4%) are the most used, showing reliance on physical deployment.
- **Team Performance** — Most teams respond within 30–40 minutes, with noticeable variation that highlights optimisation opportunities.

### What This Dashboard Shows
- **[Incident Trends](ca://s?q=Explain_incident_trends_chart)** — workload patterns over time  
- **[Priority Distribution](ca://s?q=Explain_priority_distribution)** — severity mix and risk levels  
- **[Incident Types](ca://s?q=Explain_incident_types_breakdown)** — dominant categories driving demand  
- **[Response Time by Team](ca://s?q=Explain_team_response_time_chart)** — operational bottlenecks  
- **[Response Modes](ca://s?q=Explain_response_modes)** — resource allocation and deployment mix  
- **[Performance Summary](ca://s?q=Summarise_dashboard_performance)** — leadership‑ready insights  




### 2. Patient Outcomes

Focuses on interventions, patient condition, and outcome categories to understand the effectiveness of responses and support quality-of-care reviews.

> Suggested use: For clinical leads and quality teams to review outcomes and trends.

### 3. Regional & Location Performance

Highlights incident distribution by region and location type, response times, and vulnerable population metrics.

> Suggested use: For operational planning, resource allocation, and identifying high-risk areas.

### 4. Incident Types & Trends

Breaks down incident categories (e.g. mental health crisis, panic attack, welfare check) and shows how demand changes over time.

> Suggested use: For understanding demand patterns and planning staffing or specialist support.



## 📊 Key Metrics & Insights

The dashboards provide real-time visibility into emergency incident activity, operational performance, and patient outcomes. Below are the core metrics and insights derived from the live dataset:

### 🔹 Incident Volume & Trends
- **3,000 total incidents** recorded during the reporting period.
- Activity remained steady across all months, with noticeable peaks during high‑demand periods.
- **Critical incidents: 607**, indicating sustained clinical pressure on response teams.

### 🔹 Response Performance
- **Average response time: 37.83 minutes** across all incident types.
- Critical cases were handled fastest at **14 minutes**, reflecting strong prioritisation.
- Low‑priority incidents experienced delays, averaging **89 minutes**, highlighting potential resource constraints.

### 🔹 Escalation & Case Complexity
- **Escalation rate: 36.43%**, showing over one‑third of incidents required higher‑level support.
- High escalation levels correlate with increased mental‑health‑related incidents.

### 🔹 Incident Types & Patterns
- Top categories:
  - **Mental Health Crisis: 503**
  - **Panic Attack: 503**
  - **Welfare Check: 488**
  - **Suicide Risk: 378**
- Mental‑health‑related incidents represent a significant portion of operational demand.

### 🔹 Patient Outcomes & Interventions
- Most used interventions:
  - **On‑site Assessment: 641**
  - **Emergency Transport: 569**
  - **De‑escalation Support: 548**
- Patient condition on arrival:
  - **Distressed: 1,340**
  - **Critical: 825**
  - **Stable: 593**
  - **Unresponsive: 242**

### 🔹 Regional & Location Insights
- Highest incident locations:
  - **Home: 1,677**
  - **Public Area: 452**
  - **Care Home: 360**
- Vulnerable population highest in **Care Homes (55%)**.
- Response times vary by location type, ranging from **35.68 to 39.9 minutes**.

### 🔹 SLA Compliance
- **69.43% SLA compliance**, indicating improvement opportunities in response consistency and resource allocation.

These insights support operational decision‑making, highlight areas requiring intervention, and provide a data‑driven foundation for improving service quality and patient outcomes.



7. What You Learned / Skills Demonstrated
This is where you show your growth.

Examples:

Building automated workflows

Designing real-time dashboards

Structuring operational data

Communicating insights to stakeholders

Understanding emergency response metrics

This section is gold for recruiters.
9. How the System Works (Real Instructions)
Explain how someone could replicate or understand the workflow.

Example:

Submit a form → data flows into Sheets → dashboard updates automatically

This proves it’s a real system.

10. Contact Section
Add your:

LinkedIn

Email

This makes it easy for recruiters to reach out.
