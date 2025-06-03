# Apollo Lead Enrichment – n8n Automation

This project automates the enrichment of company leads using the Apollo API, Apify scraping, and Google Sheets, all orchestrated with n8n.

## 🔧 Features
- Pulls companies from a Google Sheet, row-by-row
- Queries Apollo for verified marketing contacts
- Uses Apify to scrape additional email and contact data
- Updates a second sheet with enriched contacts
- Tracks enrichment status (`Collected: Yes`) per row
- Wait nodes included to avoid API rate limits

## 🛠️ Tools Used
- [n8n](https://n8n.io) – Automation engine
- [Apollo.io](https://apollo.io) – Verified email and contact data
- [Apify](https://apify.com) – Scraping framework
- Google Sheets – Source & output

## 🧪 How to Use
1. Import the provided JSON file into your n8n instance (click "Import").
2. Set up your Apollo and Apify API keys.
3. Connect your Google Sheets credentials.
4. Run the workflow manually or schedule it.

## 📂 Files
- `Apollo_Lead_Enrichment_Flow.json`: Main n8n workflow export

## 📈 Use Case
Ideal for lead generation from event/conference attendee lists, scraped company databases, or cold outreach targeting.

---

Built by [AlvLeoAI](https://www.linkedin.com/in/alvarolvazquez)

