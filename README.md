<img width="1672" height="582" alt="image" src="https://github.com/user-attachments/assets/3289b2e1-169b-44f0-aa1b-a0b446909e7a" />



# 🤖 AI Web Search Agent

An AI-powered general-purpose assistant built with n8n that can intelligently use different tools based on the user's request.

## 🚀 Features

- 💬 Conversational AI through Chat Trigger
- 🔍 Automatic web search using SerpAPI
- 🧮 Calculator tool for mathematical operations
- 🧠 Conversation memory
- 🤖 AI-powered tool selection
- 🌐 General-purpose web search for current and latest information

## 🛠️ Tech Stack

- n8n
- OpenAI
- SerpAPI
- AI Agent
- Simple Memory

## ⚙️ Workflow

User Message  
↓  
Chat Trigger  
↓  
AI Agent  
↓  
├── OpenAI Chat Model  
├── Simple Memory  
├── Calculator  
└── Google Search (SerpAPI)

## 💡 Example Queries

The agent can automatically decide when to use a tool.

- "What is the current weather in New Delhi?"
- "What are the latest AI developments?"
- "Calculate 9876 × 543"
- "What are the latest React features?"
- "Who is the current Prime Minister of India?"


## 📸 Screenshots

### n8n Workflow
<img width="1672" height="582" alt="Screenshot 2026-09-15 100406" src="https://github.com/user-attachments/assets/a8e83fe5-4c2a-43b6-97ad-cd20c5dfb2a9" />


### AI Agent in Action
<img width="1670" height="850" alt="Screenshot 2026-09-15 105616" src="https://github.com/user-attachments/assets/3dfedbed-6774-462f-a161-37d67f74484d" />


### Tool Execution
<img width="1903" height="922" alt="Screenshot 2026-09-15 094832" src="https://github.com/user-attachments/assets/793d29ef-cffa-4a8e-8696-2a9125d45da1" />


## 🔐 Security

API keys and credentials are not included in this repository.

## 📌 Project Status

Completed — first n8n AI Agent project.
