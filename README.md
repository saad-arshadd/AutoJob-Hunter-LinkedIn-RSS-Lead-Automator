# AutoJob Hunter – LinkedIn RSS Lead Automator

## 📌 Overview
AutoJob Hunter is an automated job search assistant built using **n8n**.  
It leverages LinkedIn job RSS feeds to automatically fetch new job postings, process them, and store the leads in Google Sheets.  
The workflow also integrates with AI to generate smart summaries or filters for each job post.

With AutoJob Hunter, you no longer have to manually scroll through LinkedIn jobs — the automation delivers them straight to your database with AI-enhanced descriptions, making your job hunt smarter and faster.

---

## ⚡ Features
- **Automated LinkedIn Job Fetching:**  
  Fetch the latest job listings from LinkedIn RSS feeds in real-time.
- **Lead Filtering & Processing:**  
  Limit the number of fetched posts to keep the feed relevant.
- **Google Sheets Integration:**  
  Automatically append or update job leads into a structured Google Sheet.
- **AI-Powered Insights:**  
  Pass job descriptions through an AI model to generate concise summaries or skill-matching notes.
- **Seamless HTTP Requests:**  
  Process job data efficiently using custom API calls.
- **Fully Customizable:**  
  Easily adjust the feed URL, filters, and AI prompt according to your job search needs.

---

## 🛠 Workflow Structure
1. **Trigger:**  
   Manual execution or scheduled automation (Cron can be added).
2. **RSS Read (LinkedIn):**  
   Pull latest job posts via LinkedIn RSS feed.
3. **Limit Node:**  
   Restrict to the desired number of jobs per run.
4. **HTTP Request:**  
   Send job data for processing or enrichment.
5. **Google Sheets Node:**  
   Append or update leads directly into your spreadsheet.
6. **Message a Model Node:**  
   Generate AI summaries, insights, or filters for each job.
7. **Optional Code Node:**  
   Apply custom data transformations before saving.

---

## 🚀 Usage
1. **Setup RSS Feed URL:**  
   Get your LinkedIn job RSS link for the relevant role or keywords.
2. **Connect Google Sheets:**  
   Link your Google account and specify the sheet for storing job leads.
3. **Configure AI Model:**  
   Add your API key (OpenAI, Gemini, etc.) to the `Message a Model` node.
4. **Run Workflow:**  
   Execute manually or set up a Cron job for periodic automation.

---

## 📂 Example Output in Google Sheets
| Job Title        | Company        | Location  | Date Posted | Summary by AI |
|------------------|---------------|-----------|-------------|---------------|
| Data Scientist   | XYZ Corp      | Remote    | 2025-08-13  | Great fit for ML/AI skills, remote-friendly |
| Backend Engineer | ABC Tech      | Berlin    | 2025-08-12  | Requires Node.js + AWS experience |

---

## 🔮 Future Enhancements
- Auto-email or Slack alerts for high-priority job postings.
- Skill-matching and scoring system.
- Direct application submission automation.

---

## 📜 License
This project is licensed under the MIT License — feel free to use and modify.
