# Apollo Lead Enrichment Flow (n8n)

This workflow automates the enrichment of company leads using Apollo, Apify, and Google Sheets. It fetches company data from a sheet, queries Apollo for matching organizations, enhances data with Apify scrapers, and writes the enriched info back into Google Sheets.

## 🔧 Tools Used

- **Apollo API** – Company and contact data enrichment
- **Apify** – Scrapes additional information
- **Google Sheets** – Source of raw leads and destination for enriched data
- **n8n** – Workflow automation platform

---

## 📁 Project Structure

- `Apollo_Lead_Enrichment_Flow_clean_public.json` – The cleaned and secure workflow file for n8n
- `.env.example` – Environment variable template
- `README.md` – You’re reading it

---

## ⚙️ Setup Instructions

1. **Clone the repository**
2. **Create a `.env` file** based on `.env.example`:
```bash
cp .env.example .env
```

3. **Fill in your environment variables** in `.env`:
```
APOLLO_API_KEY=your_apollo_api_key
APIFY_API_KEY=your_apify_api_key
GOOGLE_SHEETS_CREDENTIALS_JSON=path/to/your/service-account.json
```

4. **Import the JSON** into your n8n instance.

---

## 🧠 How It Works (Step-by-Step)

1. Fetch unprocessed rows from Google Sheets
2. Query Apollo for organization matches
3. Scrape extra data using Apify actor
4. Write enriched data into target Google Sheet
5. Update status column to prevent reprocessing

---

## 🚨 Important Notes

- **Never** commit your `.env` file or real credentials.
- Always keep service account JSON outside public repositories.
- Requires n8n instance with external credentials management.

---

## 👨‍💻 Author

AlvLeo X – Automation Specialist | Web3 | AI | Zapier/n8n/Make
