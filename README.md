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

**Screenshot: Lead Data in Google Sheet**  
<img width="1387" height="199" alt="image" src="https://github.com/user-attachments/assets/70f91744-b14b-424b-b702-53b186673f70" />

---

### Step 2: Domain Name Extraction
For each lead:
- Use domain from the data if available.
- Otherwise, extract domain from email or website.
- If domain is missing, log the issue in an **Error Logs** tab.

**Screenshot: Error Logs Example**  
<img width="1797" height="190" alt="image" src="https://github.com/user-attachments/assets/eff9cb5c-4600-4919-a2d6-cade8caa0452" />

---

### Step 3: Website Content Scraping & Summarization
- Identify the base URL for each valid domain.
- Scrape textual content from the homepage.
- Generate a **short business summary** (2–3 sentences).
- Save the summary in the Google Sheet.

**Screenshot: Business Summary in Sheet**  
<img width="1568" height="190" alt="image" src="https://github.com/user-attachments/assets/9607b133-b6fd-4e05-b4cf-d74252a1a6c6" />

---

### Step 4: Personalized HTML Email Generation
- Use the lead data and summary to generate **personalized outreach emails** in HTML.
- Emails include:
  - Human-like context.
  - Proper headings, paragraphs, and buttons.
  - Limited emojis for visual appeal.
- Store HTML content in the Google Sheet.

**Screenshot: HTML Email Preview**  
<img width="1696" height="187" alt="image" src="https://github.com/user-attachments/assets/fbf4db2c-9b94-425b-be90-374e0ed7a043" />

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
2. Import the workflow JSON into n8n.
3. Set up Google Sheets API credentials.
4. Run the workflow or trigger by adding/updating leads.
5. Check the Google Sheet for processed summaries and HTML emails.

---

Author: Prins Ambaliya

Email: prinsambaliya66@gmail.com

Project: AI-Powered Lead Generation & Outreach Workflow
