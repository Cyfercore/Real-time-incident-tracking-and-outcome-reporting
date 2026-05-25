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
<img width="2220" height="1250" alt="Patient Outcome" src="https://github.com/user-attachments/assets/3e09f703-b7b0-4391-a27a-6643f5e4dc38" />


### Patient Outcomes — Key Insights
- **Total incidents:** **3,000** — steady demand across the window; no single‑day surge.  
- **Average response time:** **37.83 minutes** — acceptable overall but uneven by priority (Critical much faster than Medium/Low).  
- **SLA compliance:** **69.43%** — below target; investigate Medium and Low priority delays.  
- **Critical incidents:** **607** — sustained high‑risk caseload requiring clinical oversight.  
- **Top interventions:** **On‑site Assessment**, **De‑escalation Support**, **Emotional Counselling** — highest usage and primary drivers of resolved on‑site outcomes.  
- **Outcome mix:** Significant **Resolved On‑Site** and **Follow‑up Required**; non‑trivial **Referrals/Admissions** affecting capacity planning.  
- **Demographics:** Largest cohort **31–45**; age and gender splits useful for targeted outreach.  
- **Actionable callouts:** Flag SLA compliance < **80%** (7‑day rolling); triage Medium backlog; reallocate on‑site assessment resources when Critical > **10%** daily.

### What this dashboard shows

- **Performance KPIs:** Total Incidents, Average Response Time, Escalation Rate, Critical Incidents with short trend indicators.  
- **Outcome distribution:** Counts and proportions for Resolved On‑Site, Follow‑up Required, Referred to Hospital, Admitted for Observation, Escalated to Crisis Team, No Contact Made.  
- **SLA compliance:** Gauge showing percent of incidents meeting response time targets and a clear SLA target reference.  
- **Intervention usage and effectiveness:** Bar and matrix views for Intervention Types (On‑site Assessment, De‑escalation, Counselling, Medication Advice, Safeguarding Referral) and their outcome correlations.  
- **Patient profile and severity:** Age and Gender distributions; Patient Condition counts (Distressed, Critical, Stable, Unresponsive).  
- **Drilldowns and filters:** Filter by priority, region, team, and time window for operational follow‑up.  
- **Operational notes:** Data window: last 30 days; updated hourly. Last updated: **YYYY‑MM‑DD HH:MM**. Owners: On‑call Ops for SLA breaches; weekly review of intervention effectiveness.


**Extended description**

Data window: last 30 days; updated hourly.  
Key metrics: Total Incidents, Average Response Time, Escalation Rate, Critical Incidents.  
SLA targets: Critical ≤ 15 min; High ≤ 30 min; Medium ≤ 60 min; Low ≤ 120 min.  
Current SLA compliance: 69.43% (investigate Medium and Low priority delays).  
Top actions: On‑call Ops for SLA breaches; triage Medium backlog; review intervention effectiveness weekly.  
Last updated: 2026-05-25 10:22 BST

### 3. Regional Overview & Patient Performance

**Description**  
This dashboard provides a combined view of incident distribution across regions, patient status on arrival, outcomes by location type, and performance patterns that help identify hotspots, vulnerable groups, and operational improvement areas.

> Suggested use: For operational planning, resource allocation, and identifying high-risk areas.
<img width="1777" height="1000" alt="Regional Dashboard" src="https://github.com/user-attachments/assets/bfb06701-4a74-4edf-aa03-18679bdaa1b1" />

### Key Insights

- **Incident volume:** 3,000 total incidents, with major activity concentrated in large cities such as London, Birmingham, Manchester, Leeds, and Newcastle.  
- **Location type patterns:** Most incidents occur in **Homes (1,677)**, followed by **Public Areas (452)** and **Care Homes (360)**.  
- **Outcome distribution:** Strong mix of **Resolved On Site**, **Follow‑Up Required**, and **Referred to Hospital**, with smaller proportions of **Escalated**, **Admitted**, and **No Contact Made**.  
- **Patient status on arrival:** High number of **Distressed (1,340)** and **Critical (825)** cases, indicating significant frontline pressure.  
- **Vulnerable populations:** Care Homes show the highest vulnerability rate (**55%**), requiring targeted safeguarding and support.  
- **Response time by location:** Response times vary slightly by location type, ranging from **35.68 to 39.9 minutes**, with Care Homes experiencing the longest delays.  
- **Operational hotspots:** Regions with high incident density and high vulnerable‑person percentages should be prioritised for resource allocation.

---

### What This Dashboard Shows

- **UK regional incident map** with markers for major cities and hotspots.  
- **Total incidents** with monthly trend bars (Jan–Dec).  
- **Incidents by location type** (Home, Public Area, Care Home, Hospital, Workplace).  
- **Outcome by location type** including Follow‑Up Required, Resolved On Site, Referred to Hospital, Escalated, Admitted, and No Contact Made.  
- **Patient status on arrival** (Distressed, Critical, Stable, Unresponsive).  
- **Vulnerable person analysis** by location type, including counts and percentages.  
- **Response time by location type** showing average minutes per category.  
- **Filters** for Region, Dispatcher Name, Gender, and Priority Level.

---

**Last updated:** 2026‑05‑25 17:06

**Summary**  
Delivered a production‑grade real‑time incident tracking and outcome reporting system that turned fragmented manual logs into an automated analytics pipeline and operational dashboards. The work enabled faster, evidence‑based decisions for operations and clinical teams and produced measurable improvements in visibility and prioritisation.

---

### Key learnings

- **Prioritise by risk and vulnerability** — Care Homes and high‑density urban areas consistently drive the greatest operational risk and should be first for targeted interventions.  
- **Interventions drive outcomes** — On‑site Assessment and De‑escalation show the strongest association with resolved‑on‑site outcomes and reduced re‑contact.  
- **Leading indicators matter** — Re‑contact and follow‑up backlog are reliable early warnings for rising referrals and admissions.  
- **Data quality underpins trust** — Standardised intake and automated pipelines reduce manual errors and materially improve dashboard reliability for frontline decision‑making.  
- **Design for action** — Dashboards that pair concise insights with ownerable actions (who, when, threshold) increase the likelihood of operational follow‑through.

---

### Skills demonstrated

- **Data integration & ETL** — built automated pipelines (Forms → Power Automate → Google Sheets) to centralise incident, dispatch, and outcome data.  
- **Data modelling & validation** — designed schemas, implemented cross‑checks, and validated counts, timestamps, and vulnerable‑person flags.  
- **Dashboard design & visualization** — created multi‑page Looker Studio dashboards (maps, funnels, gauges, cohort tables) for operational and executive audiences.  
- **Operational analytics** — defined KPIs and leading indicators (response time, escalation rate, re‑contact) and linked them to actionable thresholds.  
- **Cohort analysis & clinical evaluation** — segmented by age, location, and incident type to identify high‑risk cohorts and evaluate intervention effectiveness.  
- **Stakeholder engagement & communication** — translated analytics into concise briefings, playbooks, and ownerable actions for Ops and Clinical leads.  
- **Quality assurance & iteration** — implemented validation tests and weekly feedback loops to refine visuals, thresholds, and annotations.

---

### Demonstrated impact (examples)

- **Resource reallocation:** used regional and vulnerability signals to justify shifting mobile units to high‑need localities during peak windows.  
- **Clinical prioritisation:** recommended targeted on‑site assessment training after observing its strong association with resolved‑on‑site outcomes.  
- **Process improvement:** introduced a daily triage for follow‑up backlog items, reducing re‑contact among targeted cohorts in pilot areas.  
- **Faster decision‑making:** replaced manual end‑of‑day reporting with hourly dashboards, enabling real‑time operational adjustments.

---

### Next steps to scale impact

- **Formalise a playbook** linking dashboard signals to operational actions and named owners.  
- **Track success metrics** (re‑contact rate, resolved‑on‑site rate, time‑to‑first‑follow‑up) to measure interventions.  
- **Automate alerts** for leading indicators (follow‑up backlog, rising re‑contact) to trigger predefined escalation workflows.  
- **Expand cohort analytics** to include social determinants and repeat‑caller case management.

---

**Role & contribution**  
Led end‑to‑end delivery: intake design, pipeline automation, data modelling, dashboard build, validation, and operational handover.

### Technologies Used

| **Tool / Technology** | **Purpose** | **Notes** |
|---|---|---|
| **Microsoft Forms** | Incident intake form | Structured frontline data capture |
| **Power Automate** | ETL / pipeline automation | Real‑time transfer from Forms to Sheets |
| **Google Sheets** | Centralised operational datastore | Schema, formulas, and lightweight modelling |
| **Looker Studio** | Interactive dashboards & reporting | Multi‑page dashboards, maps, funnels, gauges |
| **SQL / Google Sheets formulas** | Data modelling & aggregation | Derived metrics, cohort queries, validation checks |
| **Scripting (Apps Script / Python)** | Validation & automation tasks | Data quality checks and simple automations |
| **Notifications (Email / Slack)** | Alerts and operational notifications | Automated alerts for owners and thresholds |
| **Stakeholder tools** | Handover and collaboration | Playbooks, briefings, and weekly review notes |

9. How the System Works (Real Instructions)
Explain how someone could replicate or understand the workflow.

Example:

Submit a form → data flows into Sheets → dashboard updates automatically

This proves it’s a real system.

### Contact

**Primary contact**  
**Name:** Collins  
**Email:** **Collins@cyfercore.com**  
**LinkedIn:** **[https://www.linkedin.com/in/collins](https://www.linkedin.com/public-profile/settings/?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_self_edit_contact_info%3BJYYNbJ4lQQyixFn8AGLUBA%3D%3D)**  
**Location:** **Birmingham, United Kingdom**


