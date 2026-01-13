# Email Pipeline (Gmail → JSON → Themed Clean JSON → PDF)

This repo contains **three independent scripts** that form a simple pipeline:

1) **Gmail → JSON**  
   Connect to Gmail using an **App Password**, scrape emails for a **time range**, export to JSON.

2) **JSON → Cleaned JSON (by theme)**  
   Use the **OpenAI API** to normalize/clean/label the extracted emails by theme.

3) **JSON → PDF**  
   Convert JSON data into a readable PDF report.

Each script is independent by design (single responsibility).

---

## Requirements

- Python 3.10+
- A Gmail account with **2FA enabled** (required for App Passwords)
- An **App Password** generated in Google Account settings
- (Script 2) An OpenAI API key

---

## Setup

### 1) Clone & install
```bash
git clone <your-repo-url>
cd email-pipeline
python -m venv venv
source venv/bin/activate  # Linux/Mac
# venv\Scripts\activate   # Windows PowerShell
pip install -r requirements.txt
