# Exposed Files and Sensitive Credentials Scanner | TAVARDT Australia

[![Exposed Files Scanner](https://img.shields.io/badge/TAVARDT-Attack%20Surface-5b3cf5.svg)](https://tools.tavardt.com/au/exposed-files-scanner/)
[![Jurisdiction](https://img.shields.io/badge/Jurisdiction-Australia-00C853.svg)](https://ag.tavardt.com/au/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

CLI attack surface scanner for automated discovery of environment files, database dumps, and credential leakage aligned with ACSC Essential Eight.

Developed and maintained by the offensive security and attack surface division of **[TAVARDT Australia](https://ag.tavardt.com/au/)**.

---

## Attack Surface Discovery Scope

* **Environment Secrets and API Keys**: Inspection for exposed `.env`, `.env.local`, and `.env.production` files.
* **Version Control Metadata**: Detection of accessible `/.git/HEAD` and `/.git/config` paths.
* **Database Backups and Dumps**: Discovery of sensitive database exports such as `backup.sql`, `dump.sql`, and `database.sql`.
* **Infrastructure Orchestration**: Verification of public `docker-compose.yml` assets and server disclosures via `phpinfo.php`.
* **Regulatory Alignment**: Designed in alignment with ACSC Essential Eight and Information Security Manual (ISM).

---

## Installation and Quick Start

Requires Python 3.8 or higher. Built strictly using the Python standard library with zero third-party packages.

```bash
git clone https://github.com/TAVARDT-Australia/exposed-files-scanner-au.git
cd exposed-files-scanner-au
python scanner.py enterprise.com.au
```

To export results in structured JSON format:

```bash
python scanner.py enterprise.com.au --json
```

---

## Online Web Diagnostics

For automated surface monitoring and detailed vulnerability analysis, access the official web diagnostic suite:

* **[Exposed Files and Secrets Scanner](https://tools.tavardt.com/au/exposed-files-scanner/)**
* **[TAVARDT Australia Corporate Portal](https://ag.tavardt.com/au/)**

---

## Enterprise Attack Surface Consulting

For penetration testing, vulnerability remediation, and zero-trust perimeter defense in Australia, contact **[TAVARDT Australia](https://ag.tavardt.com/au/contact/)**.
