🕵️‍♂️ Shadow Scout: AI Identity Exposure Auditor
"Hackers don't just break firewalls; they break people."

Shadow Scout is an AI-powered OSINT (Open Source Intelligence) tool designed to audit digital footprints. It scans the open web for a target's public information and uses Google Gemini 3 Flash to simulate how a social engineer could exploit that data.

📖 Overview
In the age of social media, our "Digital Footprint" is our biggest vulnerability. Traditional OSINT tools are complex and only list raw data. Shadow Scout bridges the gap by using Generative AI to provide Contextual Intelligence.

It doesn't just find data; it explains why that data is dangerous and generates a Vulnerability Report with theoretical attack scenarios (e.g., phishing pretexts) so users can proactively secure their identity.

✨ Key Features
🔍 Deep Web Scanning: Utilizes Google Custom Search JSON API to index scattered digital footprints (social media, forums, public records).

🧠 Agentic AI Analysis: Powered by Gemini 3 Flash, the AI filters out noise (unrelated namesakes) and connects the dots between isolated data points.

🛡️ Automated Threat Modeling: Generates a personalized "Attacker's Perspective" report, identifying specific social engineering risks.

⚡ Auto-Retry Architecture: Built-in resilience to handle API rate limits and network instability.

🔒 Privacy-First: Runs locally or on secure cloud instances; no data is stored permanently.

🛠️ Tech Stack
Frontend: Streamlit (Python)

AI Engine: Google Gemini 3 Flash (via google-generativeai)

Search Engine: Google Custom Search JSON API

Language: Python 3.10

🚀 Installation & Setup
Prerequisites
Python 3.8 or higher

Google Cloud Platform Account (for Search API)

Google AI Studio Account (for Gemini API)

1. Clone the Repository
Bash
git clone https://github.com/YourUsername/shadow-scout.git
cd shadow-scout

3. Install Dependencies
Bash
pip install -r requirements.txt

5. API Configuration
You will need three keys to run this tool:

   Google Search API Key: Enable "Custom Search JSON API" in Google Cloud Console.

   Search Engine ID (CX): Create a search engine at programmablesearchengine.google.com and enable "Search the entire web".

   Gemini API Key: Get it from aistudio.google.com.

4. Run the App
Bash
streamlit run shadow_scout.py
