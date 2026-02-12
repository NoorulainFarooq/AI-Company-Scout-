Scout.ai – AI Job & Company Scout

Scout.ai is an AI-powered job and company scouting web application that searches live job boards and extracts structured insights using automation and AI.
The frontend is built using Google AI Studio and deployed on Vercel, while the backend is powered by an n8n workflow that automates job search, data extraction, and AI-based summarization.

🚀 Features

🔍 Live job search from Indeed and global job boards
🧠 AI-powered extraction and summarization of job details
📊 Structured job listings with company profiles
🌐 Web-based UI for easy user interaction
⚙️ Fully automated backend workflow using n8n

🏗️ System Architecture

Frontend
Built using Google AI Studio
Deployed on Vercel
Accepts user search queries (e.g., web engineer)
Displays job results and market insights

Backend (n8n Workflow)
The backend is implemented as an n8n automation pipeline:

User Input (Webhook Trigger)
Receives the job keyword from the frontend.

Build Search Query
Formats the user input into a job search query.

Job Search API (SerpAPI)
Fetches live job listings from Indeed.

Pick Top 5 Jobs
Filters and selects the most relevant results.

Split Out & Loop Over Jobs
Iterates through each job posting.

HTTP Request (Job URL)
Scrapes the job description page.

HTML Extraction
Extracts readable content from the HTML page.

AI Agent (OpenAI Chat Model)
Uses AI to:
Summarize job descriptions
Extract company name, role, and key requirements
Generate structured insights

Respond to Webhook
Sends processed results back to the frontend.

🧰 Tech Stack
Frontend
Google AI Studio
HTML / CSS
Vercel (deployment)
Backend
n8n (workflow automation)
SerpAPI (job search)
OpenAI Chat Model
HTTP & HTML extraction nodes

Use Cases
Job seekers searching for live roles
Market research & hiring trend analysis
Company discovery
Lead generation for recruitment agencies

🔮 Future Improvements
Add location and salary filters
Save results to database (Postgres / Firebase)
User authentication
Email alerts for new jobs
Multi-platform job search (LinkedIn, Glassdoor, etc.)
