# 📌 SOC Automation Toolkit

## 🚀 Overview
The **SOC Automation Toolkit** is a collection of scripts, playbooks, and integrations designed to **enhance the efficiency of Security Operations Centers (SOCs)** by automating repetitive tasks, improving threat detection, and accelerating incident response. This toolkit enables SOC teams to automate their workflows, reduce alert fatigue, and improve investigation accuracy.

### ✨ Key Benefits
- **Faster Incident Response**: Automate analysis and response actions to reduce MTTR.
- **Reduced Alert Fatigue**: Filter and enrich security alerts to focus on critical threats.
- **Enhanced Threat Detection**: Correlate data across multiple security platforms for deeper insights.
- **Seamless Integration**: Easily connect with SIEMs, EDRs, firewalls, and other security tools.

## 🎯 Features
### 🔍 Threat Intelligence Enrichment
- Automate IOC lookups via:
  - **VirusTotal**
  - **AbuseIPDB**
  - **AlienVault OTX**
  - **MISP (Malware Information Sharing Platform)**
  - **Shodan API**
- Correlate IOCs against real-time logs and alerts.

### 🔥 SOC Playbooks & Automation
- Predefined workflows for:
  - **Phishing email triage**
  - **Malware analysis automation**
  - **Suspicious login investigation**
  - **Insider threat detection**
- Automated alert correlation and response.

### 📊 SIEM & EDR/XDR Automation
- **SIEM Integration**: Splunk, ELK Stack, Microsoft Sentinel.
- **Endpoint Security Automation**: CrowdStrike, SentinelOne, Palo Alto Cortex XDR.
- **Firewall & IDS/IPS Integration**: Palo Alto, Cisco Firepower, Suricata.
- **Email Security Automation**: Microsoft Defender for O365, Proofpoint.

### 📩 Email & Phishing Analysis
- Extract and analyze:
  - Email headers
  - Attachments
  - Embedded URLs
- Automated sandbox detonation and reputation analysis.

### ⚙️ API Integrations
- **Splunk API** for automated log queries and alerting.
- **CrowdStrike Falcon API** for EDR automation.
- **Shodan API** for reconnaissance and asset discovery.
- **AWS Security Hub** for cloud security automation.

## 📁 Project Structure
```plaintext
SOC-Automation-Toolkit/
│── scripts/              # Automation scripts for SOC workflows
│── playbooks/            # Incident response playbooks
│── integrations/         # API integrations with security tools
│── logs/                 # Sample log files for testing
│── docs/                 # Documentation and usage guides
│── config/               # Configuration files (API keys, settings, etc.)
│── requirements.txt      # Dependencies for Python scripts
│── README.md             # Project overview and details
```
## 🛠️ Installation & Setup
### Prerequisites
- **Python 3.x**
- **pip** package manager
- API keys for integrated services (VirusTotal, MISP, etc.)

### Installation Steps
1️⃣ **Clone this repository:**  
```bash
git clone https://github.com/jiaming-sec/SOC-Automation-Toolkit.git
cd SOC-Automation-Toolkit
```
2️⃣ **Install dependencies:**  
```bash
pip install -r requirements.txt
```
3️⃣ **Configure API keys** in `.env` or `config/config.yaml`.

## 🚀 Usage
### Running a script
Execute a specific script using:
```bash
python scripts/threat_intelligence.py --ioc 192.168.1.1
```
Run an automation playbook:
```bash
python playbooks/email_analysis.py --email suspicious@phishing.com
```
