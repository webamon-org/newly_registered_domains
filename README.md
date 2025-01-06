# Daily Domain Updates from ICANN Centralized Zone Data Service (CZDS)

This repository provides a daily snapshot of newly registered and removed domains sourced from the [ICANN Centralized Zone Data Service (CZDS)](https://czds.icann.org). It aggregates data across all generic and new top-level domains (TLDs) and updates daily by **7.29 AM UTC** for the previous day's domain changes.

ICANN requires that TLD zone files be updated in CZDS by **7:00 AM UTC**, and this repository ensures responses within **<30 mins**.

---

## 🌍 Zone File Coverage

- **Total Zone Files in CZDS**: 1,132
- **Zone Files Webamon Has Access To**: 1051

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
```



### **Key Files:**
1. **`new_domains.txt`**:
   - A complete list of newly registered domains for the respective scope (root for all TLDs, or specific TLD directory).
2. **`removed_domains.txt`**:
   - A list of domains that were removed from the zone file since the previous day.
3. **`summary.json`**:
   - Metadata summary including domain counts, newly added domains, and removed domains.

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
  - No 3rd parties, parse current domains at the source zonefile.
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

This repository is updated automatically and is not intended for manual updates. However, if you encounter any issues or have suggestions for improvements, feel free to open an [issue](https://github.com/webamon-org/newly_registered_domains/issues).

---

## 📜 License

This project is open-source and available under the [Apache License 2.0](LICENSE).

---



## 🛠️ Acknowledgements

Data is sourced from the [ICANN CZDS](https://czds.icann.org). We adhere to ICANN's requirements and guidelines for data usage and updates.

