# Gmail to JSON — Email Scraper (App Password)

This repository contains **one single Python script** whose only responsibility is:

 **Connect to Gmail using an App Password, scrape emails for a given time range, and export them to a JSON file.**

No OpenAI.  
No PDF.  
One script. One job.

---

## What this script does

- Connects to Gmail via **IMAP**
- Authenticates using a **Gmail App Password**
- Fetches emails between two dates
- Extracts:
  - message id
  - date
  - from
  - to
  - subject
  - plain text body (when available)
- Exports all emails into a structured **JSON file**

---

## Requirements

- Python **3.10+**
- A Gmail account with **2-Factor Authentication enabled**
- A **Gmail App Password** (required — normal password will NOT work)

---

## Gmail App Password setup

1. Go to your **Google Account**
2. Enable **2-Step Verification**
3. Open **App passwords**
4. Create a new password for:
   - App: Mail
   - Device: Other
5. Copy the **16-character password** (no spaces)

---
