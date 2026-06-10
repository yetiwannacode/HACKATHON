# GistGenie  
Automate Meeting Insights & Follow-Ups with AI

GistGenie is a **no-code / low-code automation built in n8n** that turns Google Meet transcripts into **concise summaries, personalized to-do lists, and calendar reminders** — all triggered automatically from Google Drive.

---

## What It Does

Whenever a meeting transcript (for example, exported from **Tactiq**) is added to a designated Google Drive folder, GistGenie automatically:

1. **Triggers**  
   Google Drive detects a newly uploaded transcript file.

2. **Ingests Content**  
   The document is retrieved and its raw text is extracted.

3. **Generates AI Insights**  
   An AI agent summarizes the meeting and identifies:
   - Key discussion points  
   - Action items  
   - Ownership and follow-ups

4. **Creates Smart Outputs**
   - Saves meeting summaries in **Google Sheets**
   - Creates **personalized tasks** in Google Tasks
   - Schedules **follow-up events** in Google Calendar

No more post-meeting chaos — just instant clarity.

---

## Tech Stack

- **n8n** – Workflow orchestration  
- **Google Drive API** – Trigger for new transcripts  
- **Google Docs API** – Transcript content extraction  
- **OpenAI / Azure OpenAI** – AI-powered summarization & task extraction  
- **Google Sheets** – Summary storage  
- **Google Tasks** – Task creation  
- **Google Calendar** – Follow-up scheduling  

---

## Setup

### Prerequisites

- An **n8n instance** (self-hosted or cloud)
- Google API credentials for:
  - Drive
  - Docs
  - Sheets
  - Tasks
  - Calendar
- OpenAI or Azure OpenAI API key
- A Google Drive folder to collect transcript files (e.g., from Tactiq)

---

### How to Use

1. Clone this repository.
2. Import `gistgenie-workflow.json` into your n8n instance.
3. Configure credentials for:
   - Google services
   - OpenAI / Azure OpenAI
4. Specify the Google Drive folder to monitor in the Drive trigger node.
5. Run the workflow once manually to test.
6. Activate the workflow for continuous automation.

> **Bonus:**  
> The AI agent maintains contextual memory to ensure summaries and follow-ups remain relevant and accurate across meetings.

---

## Example Use Case

Imagine you just finished a 30-minute team sync and export the transcript via Tactiq.

GistGenie automatically:
- Generates a concise bullet-point summary
- Assigns *“Design dashboard UI”* to **Ayush** in Google Tasks
- Schedules a follow-up meeting reminder in Google Calendar for Friday

All in under a minute.

---

## Why GistGenie?

Meetings are essential — but follow-ups are often forgotten.

GistGenie acts as your **AI-powered meeting assistant**, ensuring:
- Clear summaries
- Actionable tasks
- Timely follow-ups  
without any manual effort.

---

## Future Enhancements

- Slack or Discord integration for sharing summaries
- Centralized dashboard for viewing summaries and task status
- Sentiment and tone analysis of meetings

---

## Author

**Ayush Mukherjee**
