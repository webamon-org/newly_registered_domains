# 📢 **Repository Has Moved**

⚠️ **IMPORTANT:** This project is no longer maintained on this platform.  
It has been **moved permanently** to **[https://codeberg.org/webamon/newly_registered_domains](https://codeberg.org/webamon/newly_registered_domains)**.  

Please update your bookmarks, scripts, and automation to pull from the new location.  
Future updates will **only** be available there.

---

# Daily Domain Updates from ICANN Centralized Zone Data Service (CZDS)

This repository provides a daily snapshot of newly registered and removed domains sourced from the [ICANN Centralized Zone Data Service (CZDS)](https://czds.icann.org). It aggregates data across all generic and new top-level domains (TLDs) and updates daily by **7.29 AM UTC** for the previous day's domain changes.

ICANN requires that TLD zone files be updated in CZDS by **7:00 AM UTC**, and this repository ensures responses within **<30 mins**.

---

## 🌍 Zone File Coverage

- **Total Zone Files in CZDS**: 1,132
- **Zone Files Webamon Has Access To**: 1055

This repository reflects only the TLDs for which Webamon has access to the zone files. Access to zone files is subject to the zone holders approval process.

---

## 📂 Directory Structure

The repository organizes data into directories and files for ease of access and granularity:

```
/root 
  ├── new_domains.txt # Aggregated list of all newly registered domains 
  ├── removed_domains.txt # Aggregated list of all removed domains 
  ├── summary.json # Aggregated metadata summary 
  ├── /<TLD>/ 
      ├── new_domains.txt # List of newly registered domains specific to the TLD 
      ├── removed_domains.txt # List of removed domains specific to the TLD 
      ├── summary.json # Metadata summary specific to the TLD 
  ├── /monitoring_output/
      ├── /<monitored_list>/ # Directory for monitored domain lists (e.g., f500_domains)
          ├── similarity_60.txt # Domains with similarity >= 60% and < 70% 
          ├── similarity_70.txt # Domains with similarity >= 70% and < 80% 
          ├── similarity_80.txt # Domains with similarity >= 80% and < 90% 
          ├── similarity_90.txt # Domains with similarity >= 90% and < 100% 
          ├── similarity_100.txt # Domains with similarity == 100% 
          ├── similarity_aggregated.txt # Aggregated results of all similarity thresholds
```





### **Key Files:**
1. **`new_domains.txt`**:
   - A complete list of newly registered domains for the respective scope (root for all TLDs, or specific TLD directory).
2. **`removed_domains.txt`**:
   - A list of domains that were removed from the zone file since the previous day.
3. **`summary.json`**:
   - Metadata summary including domain counts, newly added domains, and removed domains.
4. **`/monitoring_output/<monitored_list>/similarity_*.txt`**:
   - Contains similarity-based analysis results for monitored domains. Each similarity file corresponds to a specific threshold range.

---

## 🕒 Update Schedule

- **Frequency**: Updated daily by **7:29 AM UTC**.
- **Source**: ICANN CZDS, which updates TLD zone files by **7:00 AM UTC**.

---

## 🔧 Functionality

- **Aggregates All TLDs**:
  - Provides a comprehensive view of all domains and changes across all general and new TLDs.
- **Granular Insights Per TLD**:
  - Separate directories for each TLD, containing scoped data.
- **Track Domain Changes**:
  - Maintains detailed lists of new and removed domains for easy tracking and analysis.
- **Daily Automation**:
  - Fully automated updates ensuring timely data delivery.
- **True Source**:
  - No 3rd parties, parse current domains at the source zone file.

---

## 🌟 Usage

1. **Access the Aggregated Data**:
   - Navigate to the `/root` directory for the combined view of all domains and changes.
2. **Analyze Specific TLDs**:
   - Use the `/TLD/` directories for scoped domain insights.
3. **Review Metadata**:
   - Refer to `summary.json` for domain counts and update statistics.

---

## 🤝 Contributions

This repository is updated automatically and is not intended for manual updates. However, if you encounter any issues or have suggestions for improvements, feel free to open an [issue](https://codeberg.org/webamon/newly_registered_domains/issues).

---

## 📜 License

This project is open-source and available under the [Apache License 2.0](LICENSE).

---

## 📢 Why Not on GitHub?

In the past, malicious actors have successfully executed targeted campaigns to have this repository taken down on GitHub. These malicious actions were orchestrated by entities that profit from "Newly Registered Domains" monitoring services. Their goal was to suppress this open and free alternative, which is relied upon by security operations centers and threat intelligence analysts worldwide.

The disruptions caused by these takedowns severely impacted organizations and individuals who depend on the timely availability of this data. To ensure uninterrupted access to this critical resource, we have moved to Codeberg, a trusted open-source platform committed to transparency and freedom. 

This repository continues to provide faster, more reliable notifications of potentially malicious gTLD registrations, empowering the community to stay ahead of threats without the gatekeeping often associated with paid services.

---

## 🛠️ Acknowledgements

Data is sourced from the [ICANN CZDS](https://czds.icann.org). We adhere to ICANN's requirements and guidelines for data usage and updates.

