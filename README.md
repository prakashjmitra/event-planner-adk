**Event Planner AI Chatbot**

This is an AI-powered event planning assistant built using Google's Agent Developer Kit (ADK) and Gemini 2.0, designed to help users seamlessly organize events through intelligent task delegation, real-time decision-making, and multi-agent coordination.

## Features

- **Venue Finder Agent** – Recommends and checks availability for venues
- **Catering Agent** – Helps arrange catering based on preferences, budget, and size
- **Budget Agent** – Generates a structured event budget and mock Google Sheet
- **Social Media Agent** – Crafts promotional content for platforms with hashtags and CTAs
- **Proposal Agent** – Compiles a full event proposal with timeline, logistics, and risk plans
- **Root Agent** – Coordinates all sub-agents to execute a full planning workflow

## Tech Stack

- **Python 3.12**
- **Google ADK**
- **Gemini 2.0 (via Vertex AI or public endpoint)**
- **FastAPI**
- **Google Cloud Services**
- **dotenv** for secure config management

## Project Structure
event-planner-adk/
├── event-planner-agent/ # Main codebase with agent setup
│ ├── .env # Environment variables (not tracked in Git)
│ ├── agent.py # Main runner with all agent definitions
│ └── ..
├── venv/ # Virtual environment (excluded from Git)
├── README.md
└── .gitignore


## Setup Instructions

1. Clone the Repository
   ```bash
   git clone https://github.com/your-username/event-planner-agent.git
   cd event-planner-agent
2. Create Virtual Environment
   python3 -m venv venv
   source venv/bin/activate
3. Install Dependencies
   pip install -r requirements.txt
4. Create a .env file in the root directory with this code:
   GOOGLE_API_KEY=your_api_key
   GOOGLE_CLOUD_PROJECT_ID=your_project_id
   GOOGLE_CLOUD_LOCATION=your_location
   GOOGLE_GENAI_USE_VERTEXAI=true
5. Run the Web Interface(via ADK): adk web

Built by: Prakash Mitra 
   
