# 🌍 AI Trip Planner Agent 🚀

An intelligent travel planning system that uses **Agentic AI** to generate fully customized trip plans with real-time contextual awareness. This agent is built using **LangGraph**, **LangChain**, and deployed with **Streamlit** and **Uvicorn** — providing seamless integration between advanced reasoning, dynamic tool usage, and rich visual UI.

---

## ✨ Key Features

✅ Real-time **weather updates**  
✅ Personalized **tourist attractions & activities**  
✅ Estimated **hotel/accommodation costs**  
✅ Live **currency conversion**  
✅ Full **itinerary generation** (day-wise)  
✅ Breakdown of **total expenses**  
✅ Executive **trip summary**

> Ask: *“Can you plan a 5-day trip to Goa?”*  
> Get: A full, data-informed, AI-curated travel experience in seconds.

---

## 🧠 Architecture Overview

The system is driven by an **Agentic Reasoning Framework** powered by **LangGraph**, where:

- Each **Node = Function** (e.g., weather fetch, attraction finder, etc.)
- Agent decides based on **Reasoning → Action → Tool Call**
- Final output is constructed via **Tool Chaining + Dynamic Execution**

### 🗂️ Component Breakdown

| Component        | Description                                            |
|------------------|--------------------------------------------------------|
| **LangGraph**    | Core orchestration engine for agent reasoning flow     |
| **LangChain**    | LLM integration and tool routing logic                 |
| **Tools**        | Modular functions: weather, places, currency, etc.     |
| **FastAPI**      | Backend API layer for inference endpoints              |
| **Streamlit**    | Rich and interactive UI for travel request input/output|
| **Uvicorn**      | ASGI server for serving backend over cloud             |
| **Cloud Infra**  | Full deployment on cloud (Azure/GCP/AWS supported)     |

---

## 🛠️ Tools & Technologies

| Category           | Stack                                               |
|--------------------|-----------------------------------------------------|
| **Language**       | Python                                               |
| **Agentic AI**     | LangGraph, LangChain                                 |
| **Frontend**       | Streamlit                                            |
| **Backend/API**    | FastAPI, Uvicorn                                     |
| **Deployment**     | Cloud-native (Docker, GitHub Actions, CI/CD enabled)|
| **Visualization**  | Matplotlib/Graphviz (for graph-based flow rendering)|

---

## 🧭 How It Works

```mermaid
graph LR
  A[User Query] --> B[LLM Agent]
  B --> C[Reasoning & Planning]
  C --> D[Tool Calls (Weather, Places, Currency)]
  D --> E[Node Graph Execution (LangGraph)]
  E --> F[Itinerary + Cost Summary]
  F --> G[Streamlit UI Output]
