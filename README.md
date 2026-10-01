# ThreatLens – AI-Powered Phishing Website Scanner

ThreatLens is a Chrome Extension that detects and blocks phishing websites using
Machine Learning and real-time URL analysis.

It protects users from credential theft, fake login pages, and malicious domains.

---

##  Features

-  Automatic website scanning on page load
-  AI-based phishing detection
-  Full-page phishing warning
-  Block phishing domains permanently
-  Allow website once (safe bypass)
-  Blocked sites management page
-  IP & country detection
-  Works in real-time

---

##  Tech Stack

### Frontend (Chrome Extension)
- HTML
- CSS
- JavaScript
- Chrome Extension Manifest V3

### Backend (Local Server)
- Python (Flask)
- Machine Learning model (model.pkl)
- URL & feature-based phishing detection

---

##  Project Structure

ThreatLens/
├── manifest.json
├── background.js
├── content.js
├── popup.html
├── popup.js
├── warning.html
├── warning.js
├── blocklist.html
├── blocklist.js
├── backend/
│ ├── app.py
│ ├── detector.py
│ ├── model.pkl
│ └── requirements.txt

yaml
Copy code

---

##  How to Run (Backend)

```bash
cd backend
pip install -r requirements.txt
python app.py
Server runs on:

cpp
Copy code
http://127.0.0.1:5000
 How to Load Extension in Chrome
Open chrome://extensions

Enable Developer mode

Click Load unpacked

Select the ThreatLens/ folder

Done..!!

## How It Works
Content script captures visited URL

Background script sends URL to backend

ML model analyzes phishing probability

If risky → redirect to warning page

User can:

Block domain permanently

Allow once

View & manage blocked sites



## Author
Mohammed Saud
Cybersecurity & Ethical Hacking Enthusiast
GitHub: https://github.com/Saud-Cyber

## Disclaimer
This project is for educational and research purposes only.
Do not use it for malicious or illegal activities.
