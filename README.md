# Clara AI Automation Intern Screening - Mansi Singh

## 🎥 Project Demonstration
**[Watch the Video Demonstration Here](https://drive.google.com/file/d/1vSRQt0fwXjNpYCf-XFmdEh6veNpM8322/view?usp=sharing)**

---

## 🛠️ System Architecture
This project is an idempotent automation system built using **n8n** and **Google Gemini 2.5 Flash**. It manages the transition of client data from an initial Demo (v1) to a finalized Onboarding state (v2).



### Key Engineering Principles
* **Zero-Cost Implementation**: The system is built entirely on free-tier tools. It utilizes local file management via the `.n8n-files` directory to avoid cloud storage costs.
* **No-Hallucination Protocol**: I implemented strict prompting rules to ensure the AI flags unknown data (e.g., business hours not mentioned in the demo) rather than inventing information.
* **Idempotent Updates**: Pipeline B identifies existing records in the Google Sheet and updates them with new "Onboarding" truth, preventing duplicate entries.
* **Audit Trail**: Every update from v1 to v2 generates a specific `changelog` field to maintain transparency and data integrity.


---

This project reflects my interest in building secure, efficient, and transparent AI-driven automations.
