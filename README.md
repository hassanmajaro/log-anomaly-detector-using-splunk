# Splunk Log Anomaly Detection System
This project is a complete Splunk-based anomaly detection solution that identifies suspicious behaviors using structured log data, lookup files, dashboards, and alerts.

## Features
-  Detect failed login surges by IP
-  Detect logins from new, unknown devices
-  Flag logins at unusual times
-  Visual dashboards for real-time monitoring
-  Reusable lookup tables for behavioral baselining
-  Alert rules for automated responses

---
## Project Structure
<pre>
  LOG_ANOMALY_DETECTOR/
    ├── alerts/ # Alert configuration guides
    ├── dashboards/ # Splunk XML dashboards
    ├── datasets/ # Sample datasets and lookup tables
    ├── docs/ # (Optional) Architecture diagrams or documentation
    ├── queries/ # SPL detection queries
    ├── .gitignore # Git exclusions
    ├── LICENSE # Project license (MIT recommended)
    └── README.md # Project overview and guide
</pre>

---

## Sample Datasets
|  Filename                |  Description                                              |
|--------------------------|-----------------------------------------------------------|
|  `dummydata.csv`         |  Simulated user logins, statuses, and messages            |
|  `known_user_ips.csv`    |  Lookup of known User IP pairs for device tracking        |
|  `train.csv`             |  Training or behavioral baseline data                     |
|  `sales_data.xlsx`       |  Transactional data for fraud analysis                    |
|  `addtotalsData.csv`     |  Aggregated log behavior data                             |
|  `homeworkdataset.csv`   |  Sample dataset for exercises                             |
|  `World_Airports.csv`    |  IP geolocation enrichment via airport/country mapping    |

---

##  Usage in Splunk
1.  **Upload Datasets**
    -  Go to *Settings > Add Data* in Splunk
    -  Upload datasets from the `/datasets` folder
2.  **Run Detection Queries**
    -  Copy `.spl` files from `/queries` into Splunk Search
    -  Run and analyze results
3.  **Set Up Alerts**
    -  Follow steps in `/alerts/*.md` to configure real-time alerts
4.  **Import Dashboards**
    -  Go to *Dashboards > Create New > Import XML*
    -  Paste content from `dashboards/anomaly_overview.xml`

---

##  Dependencies
-  Splunk Enterpries (or Splunk Cloud)
-  Search & Reporting App (default in Splunk)
-  Lookups enabled

---

##  Author
**Majaro Hassan**

Cybersecurity Enthusiast | Certified Information Security Consultant (CISC) | SOC & SIEM Analyst

---

## License
This project is licensed under the MIT License - see the `LICENSE` file for details.
