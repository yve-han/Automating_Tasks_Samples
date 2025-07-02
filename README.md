# Work Sample Repository: Semiconductor Manufacturing Analytics

This repository showcases three real-world Python + SQL projects used to extract, transform, and analyze manufacturing data in a high-volume semiconductor foundry. These scripts were originally developed for production use in automated reporting and decision support systems.

---

## 🔍 Project 1: Key Material Track Against Commit
**Goal:** Estimate cycle time remaining for in-process materials (=lots), and align them with upcoming commit deadlines.

- Extracts active work-in-progress data from PyUber SQL connector
- Filters and calculates total planned cycle time per material
- Identifies the current operation for each material
- Outputs Power BI–ready summary of upcoming risks to commitments

---

## 📊 Project 2: Material Velocity History
**Goal:** Analyze and benchmark DPML (days per mask layer) across materials.

- Pulls and aggregates historical throughput data using CTEs in SQL
- Computes statistics like mean, median, and 95th percentile for DPML
- Generates a formatted DataFrame for visualization in Power BI
- Useful for fab efficiency and variability monitoring

---

## 📬 Project 3: Static Material Sniffer + Email Alerts
**Goal:** Automatically detect and notify engineers of materials on hold or in abnormal states.

- SQL logic captures held materials or with exceptions
- Python automates report formatting (HTML tables) and sends emails
- Dynamic grouping based on material owner or categorized reasoning
- Supports proactive material disposition and engineering ownership

---

## 🔧 Technologies Used

- Python (pandas, numpy, smtplib, logging)
- SQL (PostgreSQL-style queries via PyUber)
- Power BI (downstream data consumption)
- Email automation via SMTP
- Manufacturing domain logic (cycle time, hold states, DPML)

---

## 📁 Repo Structure

work_sample_repository/
<pre> ```text work_sample_repository/ ├── key_material_track_against_commit.py ├── material_velocity_history.py ├── static_material_sniffer.py └── README.md ``` </pre>

---

## 👩‍💻 Author

Yve Youjung Han  
📧 yve.y.han@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/yvehan)
🔗 [GitHub](https://github.com/yvehan)

---

> **Note:** All queries have been anonymized to protect company-sensitive information. Business logic and structure have been retained to reflect real-world usage.

