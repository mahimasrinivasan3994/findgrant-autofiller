# 🔍 FindGrant Smart Auto-Filler System

> **AI-powered grant discovery, matching, and form autofill tool**
> Built as capstone project | George Brown College | Jan – Apr 2025

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![GPT-4o](https://img.shields.io/badge/GPT--4o-412991?style=for-the-badge&logo=openai&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Problem Statement

Grant applicants — especially small nonprofits, students, and entrepreneurs — spend **hours** manually:
- Researching which grants they qualify for across dozens of platforms
- Re-typing the same personal/organisational information into each application
- Missing deadlines due to the sheer volume of manual work

**There was no intelligent, automated solution for end-to-end grant application management.**

---

## 💡 Solution

An end-to-end ML-powered system with three integrated components:

```
┌─────────────────┐     ┌──────────────────────┐     ┌─────────────────────┐
│  Web Scraper    │────▶│  NLP Recommendation  │────▶│  Browser Extension  │
│  4,000+ URLs    │     │  Engine (GPT-4o)      │     │  Auto-Fill Forms    │
└─────────────────┘     └──────────────────────┘     └─────────────────────┘
```

### Component 1 — Grant Discovery (Web Scraping)
- Scraped and structured **4,000+ grant website URLs**
- Assessed each for application readiness (open/closed, eligibility criteria, deadline)
- Built a structured database of grant metadata for matching

### Component 2 — NLP Recommendation Engine
- Powered by **GPT-4o** for intelligent user-to-grant matching
- Analyses user profile (location, type, field, funding need) against grant criteria
- Returns ranked recommendations with match confidence scores

### Component 3 — Browser Extension (Autofill)
- Captures user profile data once
- Auto-populates PDF and web-based grant forms intelligently
- Handles field mapping across different form structures

---

## 📊 Results

| Metric | Value |
|--------|-------|
| Efficiency improvement | **92%** reduction in application time |
| Grant sources structured | **4,000+** URLs |
| Application time | From hours → minutes |

---

## 🏗️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Data Collection | Python, BeautifulSoup, Scrapy |
| NLP & Matching | GPT-4o, LangChain |
| Backend | Python (Flask) |
| Browser Extension | JavaScript, Chrome Extension API |
| Storage | JSON / SQLite |

---

## 📁 Project Structure

```
findgrant-autofiller/
│
├── scraper/
│   ├── grant_scraper.py        # Web scraping pipeline
│   └── url_processor.py        # URL structuring & readiness assessment
│
├── recommender/
│   ├── nlp_engine.py           # GPT-4o recommendation logic
│   └── user_profile.py         # User profile schema
│
├── extension/
│   ├── manifest.json           # Chrome extension config
│   ├── content.js              # Form detection & autofill logic
│   └── popup.html              # Extension UI
│
├── data/
│   └── grants_database.json    # Structured grant metadata
│
├── requirements.txt
└── README.md
```

---

## 🚀 How to Run

```bash
# Clone the repo
git clone https://github.com/mahimasrinivasan3994/findgrant-autofiller.git
cd findgrant-autofiller

# Install dependencies
pip install -r requirements.txt

# Run the scraper
python scraper/grant_scraper.py

# Start the recommendation engine
python recommender/nlp_engine.py

# Load the browser extension:
# Chrome → Settings → Extensions → Load Unpacked → select /extension folder
```

---

## 👩‍💻 Author

**Mahima Srinivasan**
[LinkedIn](https://www.linkedin.com/in/mahimasrinivasan3994) · [Email](mailto:mahima.s3994@gmail.com)

---

*⭐ If you found this useful, give it a star!*
