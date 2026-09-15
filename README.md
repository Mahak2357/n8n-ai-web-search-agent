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

AI Web Search Agent – Workflow Explanation

1. Chat Trigger – Entry Point
   
   • The workflow starts with the "When Chat Message Received" node.
   
   • It acts as the entry point of the workflow.
   
   • Whenever the user sends a message, the Chat Trigger receives the user's input.
   
   • The user's message is then passed to the AI Agent.

3. AI Agent – Core Decision Maker
   
   • The AI Agent is the central component of the workflow.
   
   • It understands the user's intent and decides how the request should be handled.
   
   • It can either answer the user directly or use one of the connected tools.
   
   • This makes the workflow agentic because the agent can autonomously select the appropriate tool based on the user's request.

5. OpenAI Chat Model – Language Intelligence
   
   • The OpenAI Chat Model is connected to the AI Agent.
   
   • It helps the agent understand natural-language queries and generate responses.
   
   • It also helps the agent reason about which tool should be used for a particular task.

8. Simple Memory – Conversation Context
   
   • Simple Memory is connected to the AI Agent to maintain conversation context.
   
   • It allows the agent to remember previous messages within the conversation.
   
   • This makes the interaction more conversational instead of treating every message as a completely new request.

10. Calculator – Mathematical Tool
    
   • The Calculator is connected to the AI Agent as an external tool.
   
   • When the user asks a mathematical question, the agent can automatically select the Calculator.
   
   • For example, for "Calculate 9876 × 543", the agent can use the Calculator and then return the result to the user.

12. Google Search with SerpAPI – Web Search Tool
    
   • Google Search through SerpAPI is connected to the AI Agent as another external tool.
   
   • The agent can use this tool when the user needs current, latest, recent, or web-based information.
   
   • The Search Query is configured as "Defined automatically by the model".
   
   • This means the search query is generated dynamically based on the user's request instead of using a hardcoded query.
   
   • For example, if the user asks "What are the latest AI developments?", the agent can automatically generate an appropriate search query and send it to SerpAPI.

14. System Instructions – Agent Behavior
    
   • A system instruction is provided to guide the AI Agent's behavior.
   
   • It tells the agent to use Google Search for current, latest, live, recent, or web-based information.
   
   • For general questions that do not require web access, the agent can answer directly using the language model.

16. Automatic Tool Selection
    
   • The main feature of the workflow is automatic tool selection.
   
   • The user does not have to manually select or execute a tool.
   
   • The AI Agent analyzes the request and decides which tool is appropriate.
   
   • For example:
       → Mathematical query → Calculator
       → Latest/current information → Google Search
       → General knowledge → OpenAI Chat Model

18. Complete Workflow
    
   • User sends a message.

   • Chat Trigger receives the message.
   
   • The message is passed to the AI Agent.
   
   • The AI Agent understands the user's intent.
   
   • The Agent decides whether a tool is required.
   
   • If required, it automatically calls the appropriate tool.
   
   • The tool returns the required information.
   
   • The AI Agent processes the result.
   
   • The Agent generates the final response.
   
   • The response is returned to the user through the chat interface.
   

21. Why This Is an AI Agent
    
   • Unlike a basic chatbot, the system does not only generate text responses.
   
   • It can understand the user's intent, make a decision, select an appropriate tool, execute the tool, use its result, and generate the final response.
   
   • Therefore, the workflow demonstrates concepts such as AI tool calling, dynamic tool selection, memory, API integration, and workflow orchestration.

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
