DeepSec: Hybrid AI-Powered Security Auditor
DeepSec is an advanced security auditing platform that combines Static Application Security Testing (SAST) with the reasoning power of Llama 3.3 (Large Language Models). It is designed to scan local source code and GitHub repositories to identify vulnerabilities listed in the OWASP Top 10:2025.

##  Features at a Glance

| Feature | Description |
| :--- | :--- |
| **Hybrid Analysis** | Combines fast Regex patterns with Deep AI reasoning. |
| **GitHub Integration** | Automatically clones and audits remote repositories. |
| **Multilingual** | Full support for **English**, **Русский**, and **O'zbek**. |
| **PoC Generation** | AI generates Proof-of-Concept exploits for confirmed bugs. |
| **Smart Reporting** | Generates interactive HTML reports with remediation steps. |

GitHub README fayli uchun ushbu qismni yanada tushunarli va tayyor buyruqlar (copy-paste) bilan boyitilgan holda tayyorladim. Bu foydalanuvchiga terminaldan chiqmasdan sozlash imkonini beradi.

 How to Get and Configure your API Key
To enable the AI-powered audit (Llama 3.3), you must obtain a free API key from Groq Cloud. Follow these steps:

<img src="./searchapi.png" alt="Audit Report" width="600"/>
1. Obtain the Key
Visit the Groq Cloud Console.

Sign up or Log in using your account.

On the left sidebar, navigate to "API Keys".

Click the "Create API Key" button.

<img src="./addapi.png" alt="Audit Report" width="600"/>


Give it a descriptive name (e.g., DeepSec-Auditor).

<img src="./addapikey.png" alt="Audit Report" width="600"/>


Copy the generated key immediately (it won't be shown again).

2. Configure via Terminal
You can quickly set up your environment by running one of the following commands in your project root:





# Create a .env file and add your key
```bash
echo 'GROQ_API_KEY="your_api_key_here"' > .env
# Verify the file was created

cat .env
```

## 🛠️ Installation & Setup

Follow these terminal commands to prepare your environment:

```bash
# 1. Clone the repository
git clone [https://github.com/TheDeepopc/deepsec.git](https://github.com/TheDeepopc/deepsec.git)
cd deepsec

# 2. Set up a Virtual Environment
python3 -m venv venv

# 3. Activate the Environment

source venv/bin/activate

# 4. Install Dependencies
pip install -r requirements.txt # if not works use command with --break-system-packages

# 5. Install Dependencies
python deepsec-l1.py
```


# 🛡️ DeepSec: AI-Powered Security Auditor

DeepSec is a high-performance security auditing platform that combines **Static Application Security Testing (SAST)** with the reasoning power of **Llama 3.3 (AI)**.

---
## 📋 System Requirements

Ensure your environment meets these minimum specifications:

| Component | Requirement |
| :--- | :--- |
| **Operating System** | Linux (Ubuntu/Kali), macOS, or Windows (WSL recommended) |
| **Python Version** | Python 3.9 or higher |
| **Tools** | Git (for cloning repositories) |
| **Connectivity** | Internet access (only for AI analysis via Groq API) |

---




##  Vulnerability Coverage Matrix 

The engine is specifically tuned to detect the following security risks as defined by the latest OWASP standards:

| Category | Description | Detected Patterns |
| :--- | :--- | :--- |
| **A01:2025** | **Broken Access Control** | Unauthorized header redirects, session role manipulation, IDOR patterns. |
| **A02:2025** | **Security Misconfiguration** | Enabled debug modes (PHP/Django/Flask), hardcoded secrets, exposed .env files. |
| **A05:2025** | **Injection** | Remote Code Execution (RCE), SQL Injection, LFI, Path Traversal, and XSS. |
| **A08:2025** | **Software & Data Integrity Failures** | Unsafe Deserialization in Python (Pickle/Marshal), PHP, and Java. |
| **A10:2025** | **Mishandling Exceptions** | Information disclosure through system stack traces and verbose error messages (die/exit). |


---

## 🛠️ Supported Languages & Ecosystems

DeepSec is designed to handle a diverse range of programming environments. The engine automatically detects the language and applies specific security rulesets.

| Language | Extension | Security Analysis Coverage |
| :--- | :--- | :--- |
| **PHP** | `.php` | RCE, SQLi, LFI, XSS, and Session Security. |
| **Python** | `.py` | Insecure Deserialization, Subprocess RCE, and OS Injection. |
| **JavaScript** | `.js` | Client-side XSS, Prototype Pollution, and Node.js security. |
| **Java** | `.java` | XXE, ObjectInputStream vulnerabilities, and Spring flaws. |
| **Go** | `.go` | Command Injection and Unsafe pointer usage. |
| **C#** | `.cs` | ASP.NET security configurations and ActiveRecord SQLi. |
| **Rust** | `.rs` | Memory safety checks and Unsafe block auditing. |
| **Ruby** | `.rb` | Rails-specific vulnerabilities and YAML deserialization. |



---

## 📜 License

This project is licensed under the **MIT License**. This means you are free to use, modify, and distribute the software, provided that the original copyright notice and permission notice are included. 

See the [LICENSE](LICENSE) file for the full legal text.

---

## 🛡️ Responsible Disclosure
If you find a security bug in this tool itself, please open an issue or contact the developer. This tool is intended for **Ethical Security Auditing** and **Educational Purposes** only.

---

### Developed with Precision by **[TheDeepOpc](https://thedeep.uz)**




