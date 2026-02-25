# Market Oracle: AI-Driven Intelligence System

![Project Banner or System Screenshot]([Link to your screenshot - Recommended: A snapshot of the HTML report or the Landing page])

## 🚀 Overview

**Market Oracle** is a cloud-native, serverless intelligence platform designed to automate personalized financial market analysis. By leveraging Large Language Models (LLMs) and event-driven architecture, the system scans market data and news sentiment to deliver high-precision stock insights directly to users.

**Live Demo:** [https://markets-oracle.com/market-oracle/](https://markets-oracle.com/market-oracle/)

---

## ✨ Key Features

- **Automated Market Scanning**: Scheduled intelligence reports triggered by **Amazon EventBridge**.
- **AI Sentiment Analysis**: Powered by **Google Gemini 2.5 Flash** with custom grounding prompts for real-time news analysis.
- **Serverless Efficiency**: Built on **AWS Lambda** for high scalability and cost-effective execution.
- **Dynamic Watchlists**: User-specific stock monitoring with state management handled via **DynamoDB**.
- **Professional Delivery Engine**: Automated HTML report generation and dispatch via **AWS SES**.

---

## 🏗 System Architecture

The system is built on an **Event-Driven, Serverless Architecture**:

1.  **Trigger Layer**: `Amazon EventBridge` handles scheduled cron jobs; manual requests are processed via API triggers.
2.  **Logic Layer**: `AWS Lambda` (Python) orchestrates the core workflow—fetching user data, normalizing tickers, and calling AI services.
3.  **Intelligence Layer**: Integration with `Google Gemini API` for deep sentiment analysis and market scanning.
4.  **Storage Layer**: `Amazon DynamoDB` manages user subscriptions, watchlists, and batch analysis caching.
5.  **Communication Layer**: `AWS SES` delivers responsive, professional-grade HTML reports to the end-user.

> **[Optional: Insert an Architecture Diagram here - You can use tools like Lucidchart or Excalidraw]**

---

## 🛠 Tech Stack

- **Language**: Python 3.x
- **Cloud (AWS)**: Lambda, EventBridge, DynamoDB, SES
- **AI/ML**: Google Gemini 2.5 Flash API (LLM Grounding)
- **Data Handling**: Pandas, Ticker Normalization Logic

---

## 🔧 Quick Start (UI Preview)

This repository showcases the **Frontend UI** and **System Architecture** of the project. Please note that the core backend logic (AWS Lambda) and API credentials are kept private for security and proprietary reasons.

### 1. Clone the repository

```bash
git clone [TBD]
cd [TBD]

```

### 2. View the UI Locally

The frontend is designed as a lightweight implementation and does not require complex environment setups or backend dependencies to preview the interface.

- **Option 1: Direct Open**
  Simply locate and double-click `index.html` in your file explorer to open it in your default web browser.
- **Option 2: Local Server (Recommended)**
  If you have Python installed, run the following command in the project directory to ensure all resources and styles load correctly:

```bash
python3 -m http.server 8000

```

---

## 📈 Optimization & Challenges

- **API Latency**: Implemented a **Batch Analysis Cache** in DynamoDB to avoid redundant LLM calls for popular tickers.
- **Data Consistency**: Developed a normalization layer to ensure ticker symbols remain consistent across different news sources and market APIs.
- **Cost Management**: Utilized AWS Free Tier and Serverless components to maintain near-zero operational costs for the current user base.

---

## 👨‍💻 Author

**Yu-Wei Lin** Software Engineer | Backend | Data & AI  
[LinkedIn](https://www.linkedin.com/in/yu-wei-lin-821891179/) | [Portfolio](https://yuwei610.github.io)
