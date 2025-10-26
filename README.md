# AI-Powered Lead Generation & Outreach Workflow 🚀

## 🧠 Problem Statement
**Lead Generation Outreach Workflow for E2M**  

This project automates the process of fetching company leads, enriching them with online data, summarizing their websites, and generating personalized HTML outreach emails using AI.

---

## 📌 Objective
Design and implement a fully automated workflow to:
- Fetch leads using the Apify API.
- Enrich and summarize company data.
- Generate contextually relevant, human-like HTML outreach emails.
- Store all results in Google Sheets for easy management.

---

## 🎯 Workflow Steps

### Step 1: Lead Data Ingestion & Trigger Setup
- Fetch **100–500 leads** using the [Apify API](https://apify.com/).
- Import lead data automatically into a **Google Sheet**.
- Workflow triggers automatically on:
  - New rows added.
  - Existing rows updated.
    
---

### Step 2: Domain Name Extraction
For each lead:
- Use domain from the data if available.
- Otherwise, extract domain from email or website.
- If domain is missing, log the issue in an **Error Logs** tab.

---

### Step 3: Website Content Scraping & Summarization
- Identify the base URL for each valid domain.
- Scrape textual content from the homepage.
- Generate a **short business summary** (2–3 sentences).
- Save the summary in the Google Sheet.

**Screenshot: Business Summary in Sheet**  
![Business Summary](./screenshots/business_summary.png)

---

### Step 4: Personalized HTML Email Generation
- Use the lead data and summary to generate **personalized outreach emails** in HTML.
- Emails include:
  - Human-like context.
  - Proper headings, paragraphs, and buttons.
  - Limited emojis for visual appeal.
- Store HTML content in the Google Sheet.

**Screenshot: HTML Email Preview**  
![HTML Email Preview](./screenshots/email_preview.png)

---

## 🧪 Deliverables
1. **Workflow JSON file**: Exported from n8n automation tool.  
   - [workflow.json](./workflow.json)

2. **API Pricing & Justification Document**  
   - List of APIs used (free and paid).
   - Comparison and justification for any paid APIs.
   - Suggested plan and cost.

3. **Walkthrough Video (3–6 min)**  
   - Demonstrates lead fetching, workflow execution, and email generation.  
   - [Walkthrough Video](./walkthrough.mp4)

---

## 📎 Constraints
- Use **free APIs only** wherever possible.
- Document API choices and justifications.
- Workflow is clean, modular, and properly labeled.

---

## 💡 Bonus Features
- Basic error handling with logs.
- Summary tab to track:
  - Total leads processed.
  - Leads skipped.
  - Completed leads.

**Screenshot: Summary Tab**  
![Summary Tab](./screenshots/summary_tab.png)

---

## ⚡ Tech Stack
- **n8n**: Automation tool.
- **Apify API**: Fetch leads.
- **Google Sheets API**: Store and manage leads.
- **AI model** (OpenAI or free alternative): Generate summaries and emails.
- **HTML**: Email formatting.

---

## 📌 Usage Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/lead-generation-workflow.git
