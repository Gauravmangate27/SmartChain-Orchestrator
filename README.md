# 🚀 Automated Supply Chain Analytics Project  

[![YouTube Demo](https://img.shields.io/badge/Watch-Demo-red?logo=youtube&style=for-the-badge)](https://youtu.be/0dJ89-65dLE?si=hAgE1VrwbsxWOHLn)

This project demonstrates a **fully automated supply chain analytics pipeline** powered by **n8n** for automation and **Quadratic AI** for intelligent insights.  

It connects your **email → PostgreSQL (Supabase) → AI Insights → Automated Reports**, enabling **real-time analytics** without manual intervention.  

---

## ✨ Features  

✅ Fetches new emails **every 1 minute**  
📎 Reads and extracts **CSV attachments**  
🧹 Cleans, parses, and validates incoming supply chain data  
📦 Stores structured data into **PostgreSQL (Supabase)**  
🧠 Generates AI-driven insights using **Quadratic AI** (via natural language prompts)  
📧 Sends out **automated supply chain reports** via email — every minute!  

---

## 🛠️ Tech Stack  

- **n8n** – Workflow automation  
- **Supabase (PostgreSQL)** – Cloud database  
- **Quadratic AI** – Natural language AI insights  
- **Email (IMAP/SMTP)** – Data ingestion + reporting  
- **CSV Parsing** – Automated file handling  

---

## 📂 Workflow Overview  

1. **Email Listener**: n8n checks inbox every minute  
2. **CSV Handler**: Reads, parses, and validates attached CSV files  
3. **Database Storage**: Uploads cleaned data into Supabase PostgreSQL  
4. **AI Insights**: Quadratic AI processes the data with natural language prompts  
5. **Report Sender**: Automatically emails insights back to stakeholders  

---

## ⚡ Demo  

🎥 Watch the live demo here:  
👉 [Automated Supply Chain Analytics Project (YouTube)](https://youtu.be/0dJ89-65dLE?si=hAgE1VrwbsxWOHLn)

---

## 📊 Example Use Cases  

- Real-time **supply chain monitoring**  
- Automated **inventory reports**  
- AI-powered **demand forecasting**  
- Zero-manual **data integration pipeline**  

---

## 🚀 Getting Started  

1. Clone this repository  
   ```bash
    git clone https://github.com/Gauravmangate27/SmartChain-Orchestrator.git
    cd SmartChain-Orchestrator
