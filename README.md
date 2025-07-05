# Automated-SAP-Certificate-Management-with-Python-and-SQL

This project automates the full lifecycle of SAP HANA certificates—discovery, expiration tracking, CSR generation, certificate import, and logging—using Python and hdbcli.

---

## 📌 Features

- ✅ Scans SAP HANA in-database and file-based certificate stores (PSE, PEM, PKCS#12)
- 📅 Tracks certificate expiration dates and sends alerts
- 🔁 Generates Certificate Signing Requests (CSR) for renewal
- 🔒 Securely imports and activates new certificates via SQL
- 🧠 Optionally syncs metadata with Azure Blob Storage
- 📊 Designed for auditability, automation, and compliance

---

## 🧠 Tech Stack

- Python 3.x
- SAP HANA (`hdbcli`)
- SAP SQL Views (`SYS.CERTIFICATES`, `PSE_CERTIFICATES`)
- OpenSSL (for file-based cert parsing)
- Azure Blob (optional for storage)
- Crontab / Scheduler (for automation)

---

## 🚀 Getting Started

```bash
git clone https://github.com/mcharrison/sap-hana-cert-management.git
cd sap-hana-cert-management
pip install -r requirements.txt
