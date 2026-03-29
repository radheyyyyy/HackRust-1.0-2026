# Powered Phishing Detection System

## Hackathon Details

* **Event:** HackRust 1.0
* **Date:** 28–29 March 2026
* **Location:** DCRUST, Sonipat, Haryana
* **Team Name:** Hakuna Matata

---

## Team Members

* **Rajyavardhan Radhey**
  3rd Year, CSE-AI
  CSJMU, Kanpur

* **Bhumika**
  2nd Year, MEE
  CSJMU, Kanpur

---

## Project Overview

This project is a **real-time phishing detection system** that combines **Machine Learning, rule-based analysis, and domain intelligence** to detect malicious URLs.

It consists of:

* **Chrome Extension** → Real-time protection while browsing
* **Backend (Node.js)** → Decision engine
* **ML Model (Python)** → Pattern detection
* **React Frontend** → URL analysis dashboard

---

## How It Works

Our system uses a **hybrid detection approach**:

### 1. Rule-Based Engine (45–55%)

Detects:

* Suspicious keywords (login, verify, secure)
* Unicode & homograph attacks
* Punycode (`xn--`)
* IP-based URLs
* Suspicious TLDs (.tk, .xyz, .zip, etc.)
* Brand impersonation

---

### 2. Machine Learning Model (25–30%)

Uses **35+ features**, including:

* URL length & structure
* Special character count
* Digit ratio
* Entropy (randomness detection)
* Domain patterns

---

### 3. Domain Intelligence

* **WHOIS Lookup** → Domain age detection
* **Traffic Rank** → Popular vs unknown sites
* **Tranco List** → Trusted top domains

---

### Final Decision

The system calculates a **final risk score** and classifies URLs as:

* 🟢 Safe
* 🟡 Suspicious
* 🔴 Phishing

---

## Features

* ✅ Real-time phishing detection
* ✅ Chrome extension with live scanning
* ✅ Automatic blocking of phishing sites
* ✅ Explainable AI (shows reasons)
* ✅ Confidence score display
* ✅ Unicode & homograph attack detection
* ✅ Hybrid ML + Rule-based system

---

## Tech Stack

* **Frontend:** React (Vite)
* **Backend:** Node.js, Express
* **ML Model:** Python, Scikit-learn
* **Extension:** Chrome Extension APIs

---

##  Installation & Usage

### 1. Clone Repository

```bash
git clone <your-repo-link>
cd HackRust-1.0
```

---

### 2. Backend Setup

```bash
cd Backend
npm install
node server.js
```

Server runs on:

```
http://localhost:5000
```

---

### 3. ML Model Setup

Make sure Python dependencies are installed:

```bash
pip install joblib scikit-learn pandas
```

Ensure:

* `model.pkl`
* `scaler.pkl`

are correctly placed.

---

### 4. React Frontend

```bash
cd phishing-frontend
npm install
npm run dev
```

Open:

```
http://localhost:5173
```

---

### 5. Chrome Extension

1. Go to:

```
chrome://extensions/
```

2. Enable **Developer Mode**
3. Click **Load Unpacked**
4. Select extension folder

---

##  How to Use

### Manual Testing (Frontend)

* Enter any URL
* Click **Scan**
* View:

  * Result (Safe / Suspicious / Phishing)
  * Score
  * Reasons

---

### Real-Time Protection (Extension)

* Open any website
* Extension automatically scans URL
* Shows popup:

  * 🟢 Safe
  * 🟡 Suspicious
  * 🔴 Blocks phishing sites

---

## Limitations

* WHOIS lookup may fail for some domains
* Traffic rank is currently simulated
* Requires backend to be running locally

---

## Future Improvements

* Real traffic rank API integration
* Advanced deep learning model
* Cloud deployment
* Browser support beyond Chrome
* Threat intelligence integration

---

## Conclusion

This project demonstrates a **scalable, real-time phishing detection system** combining **AI + cybersecurity principles** to enhance user safety while browsing.

---

## Acknowledgment

Built during **HackRust 1.0** with the aim of creating a practical and deployable cybersecurity solution.
