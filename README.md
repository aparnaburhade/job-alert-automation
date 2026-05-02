# 🚀 Job Alert Automation System

An automated job tracking system built using self-hosted n8n that monitors job postings across multiple companies and sends real-time alerts for relevant roles.

---

## 🔧 Features

- Fetches job postings from multiple APIs (Greenhouse, Ashby)
- Filters roles based on keywords (Backend, AI, Entry-Level)
- Filters US-based roles
- Deduplicates jobs using Google Sheets (state management)
- Sends real-time alerts via Telegram
- Runs automatically using scheduled triggers

---

## 🏗️ Architecture

Schedule Trigger  
→ Fetch Jobs (API)  
→ Extract & Normalize Data  
→ Filter Relevant Roles  
→ Compare with Stored Jobs (Google Sheets)  
→ Send Alerts (Telegram)  
→ Store New Jobs  

---

## 🧰 Tech Stack

- n8n (self-hosted via Docker)
- Google Sheets (data persistence)
- Telegram Bot API (notifications)
- REST APIs (Greenhouse, Ashby)

---

## 📁 Project Structure

job-alert-automation/  
├── README.md  
├── workflows/  
│   └── job-alert-workflow.json  
├── sample-data/  
│   └── example-output.json  

---

## 💡 Why I Built This

Manually checking job portals was time-consuming and often led to missed opportunities.

This system:
- Automates job discovery  
- Filters only relevant roles  
- Sends alerts instantly  
- Ensures faster application turnaround  

---

## 🚀 How It Works

1. Fetch job listings from multiple company APIs  
2. Normalize job data (title, company, location, URL)  
3. Filter roles based on predefined criteria  
4. Check against stored jobs in Google Sheets  
5. Send Telegram alert if job is new  
6. Save job to prevent duplicates  

---

## 📌 Future Improvements

- AI-based job relevance scoring  
- Integration with additional ATS platforms (Workday, Lever)  
- Web scraping for companies without public APIs  
- Email + Slack notification support  

---

## ⭐ Summary

This project demonstrates:
- API integration  
- Workflow automation  
- Data filtering and transformation  
- Persistent state management  
- Real-time notification systems  

---
