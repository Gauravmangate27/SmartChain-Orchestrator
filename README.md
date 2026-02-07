# SmartChain-Orchestrator

A fully automated supply chain analytics pipeline using n8n for workflow orchestration and Quadratic AI for intelligent data insights.

This project creates an end-to-end, real-time data pipeline that ingests supply chain information from email attachments, stores it in a PostgreSQL database (Supabase), generates AI-powered insights, and delivers automated reports — all without manual intervention.

Live Demo Video: [Automated Supply Chain Analytics Project](https://youtu.be/0dJ89-65dLE?si=hAgE1VrwbsxWOHLn)  
Repository: https://github.com/Gauravmangate27/SmartChain-Orchestrator

## Overview

The system automates the entire supply chain data lifecycle:

- Monitors email inbox for new messages (checked every 1 minute)  
- Extracts and processes CSV attachments containing supply chain data  
- Cleans, validates, and structures the data  
- Stores records in Supabase (PostgreSQL)  
- Uses Quadratic AI to analyze data via natural language prompts and generate actionable insights  
- Automatically emails summarized reports to stakeholders  

**Important Note**  
This project is designed for demonstration, learning, and prototyping purposes. Production use should include proper security hardening, error handling, rate limiting, and compliance checks (especially for email and data privacy).

## Features

- Automatic email polling every 60 seconds (IMAP)  
- Extraction and parsing of CSV attachments  
- Data cleaning, validation, and transformation  
- Persistent storage in cloud-hosted PostgreSQL (Supabase)  
- Natural language–driven AI analysis using Quadratic AI  
- Automated email delivery of insight reports (SMTP)  
- No-code/low-code implementation via n8n workflows  

## Tech Stack

| Component              | Technology/Tool              | Purpose                              |
|------------------------|------------------------------|--------------------------------------|
| Workflow Automation    | n8n                          | Orchestrates the entire pipeline     |
| Database               | Supabase (PostgreSQL)        | Structured data storage              |
| AI Insights            | Quadratic AI                 | Natural language data analysis       |
| Email Integration      | IMAP / SMTP                  | Data ingestion and report delivery   |
| File Processing        | Built-in n8n nodes + parsing | CSV handling and validation          |

## Workflow Steps

1. **Email Listener** — n8n polls the inbox at 1-minute intervals for new messages with CSV attachments.  
2. **Attachment Processing** — Downloads, reads, parses, cleans, and validates CSV data.  
3. **Data Storage** — Inserts cleaned records into Supabase PostgreSQL tables.  
4. **AI Analysis** — Quadratic AI queries the database and generates insights based on predefined natural language prompts.  
5. **Report Generation & Delivery** — Compiles insights into a formatted report and sends it via email to designated recipients.

## Example Use Cases

- Real-time monitoring of supply chain KPIs (inventory levels, delays, stockouts)  
- Automated daily/ hourly inventory and performance reports  
- AI-assisted demand forecasting and anomaly detection  
- Zero-touch data integration from suppliers/vendors via email  

## Getting Started

### Prerequisites

- n8n instance (self-hosted or cloud)  
- Supabase project with PostgreSQL database  
- Quadratic AI account (free tier available at https://www.quadratichq.com/)  
- Email account credentials with IMAP/SMTP access  

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/Gauravmangate27/SmartChain-Orchestrator.git
   cd SmartChain-Orchestrator
