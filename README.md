# Smart Task Manager Agent

## 🎯 Objective
This project is an AI-powered agent that automates task scheduling. It listens for tasks sent via email, uses an LLM to understand the request, and intelligently adds them to a Google Calendar.

## 🛠️ Tech Stack
- **Automation:** n8n
- **AI/NLP:** OpenAI (GPT-4.1-MINI)
- **Services:** Google Calendar API, Gmail API

## ⚙️ How It Works
The project uses a three-step n8n workflow:
1.  **Gmail Trigger:** The workflow starts when an email is received with the subject `#task`.
2.  **AI Processing:** The email content is sent to an OpenAI model to extract the event title, date, and time into a structured JSON format.
3.  **Google Calendar Action:** The structured data is used to create a new event in Google Calendar, with the start and end times correctly formatted.

## 📸 Screenshots

### The n8n Workflow
![My n8n Workflow]<img width="994" height="556" alt="image" src="https://github.com/user-attachments/assets/ce640a4a-eb56-4068-bc4c-5be028b1dfd0" />

### Sample Calendar Event
![Sample Event](<img width="1520" height="757" alt="image" src="https://github.com/user-attachments/assets/9d88139d-fe7f-4a8b-97d0-ca84bd60a876" />
)

---

