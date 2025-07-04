# End-to-End AI Agent Chatbot

This project is an AI Agent Chatbot that allows users to interact with powerful LLMs (Groq LLaMA3, OpenAI GPT-4) via a web interface, with optional web search capabilities.

## Features
- Chat with LLMs (Groq, OpenAI)
- Optional web search tool
- Streamlit frontend
- FastAPI backend

## Setup Instructions

1. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   (Run this command in the project root directory.)

2. **Set up environment variables**
   - Create a `.env` file in the project root with your API keys:
     ```env
     GROQ_API_KEY=your_groq_api_key
     OPENAI_API_KEY=your_openai_api_key
     TAVILY_API_KEY=your_tavily_api_key
     ```

## Running the Application

### 1. Start the FastAPI Backend
From the project root, run:
```bash
python -m uvicorn main:app --reload --port 8000
```
- The backend will be available at http://localhost:8000

### 2. Start the Streamlit Frontend
In a new terminal, from the project root, run:
```bash
streamlit run frontend/app.py
```
- The frontend will be available at http://localhost:8501

## Usage
- Use the Streamlit UI to select the model provider, model, system prompt, and enable/disable web search.
- Enter your message and chat with the AI agent!
