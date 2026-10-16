# stock-market-ai-
## 📁 Project Structure

The project is divided into three main parts: **Frontend, Backend, and AI Service**.

```text
AI-Stock-Market/
│
├── frontend/                      # User interface
│   └── src/
│       ├── components/             # Reusable UI components
│       │   ├── Navbar.jsx
│       │   ├── StockCard.jsx
│       │   ├── StockChart.jsx
│       │   ├── NewsList.jsx
│       │   └── ChatInterface.jsx
│       │
│       ├── pages/                  # Main application pages
│       │   ├── Dashboard.jsx
│       │   ├── StockDetails.jsx
│       │   └── ResearchAssistant.jsx
│       │
│       ├── services/
│       │   └── api.js              # Connects frontend to backend
│       │
│       ├── App.jsx
│       └── main.jsx
│
├── backend/                        # Node.js and Express server
│   └── src/
│       ├── routes/                 # Defines API endpoints
│       │   ├── stock.routes.js
│       │   ├── news.routes.js
│       │   └── ai.routes.js
│       │
│       ├── controllers/            # Handles incoming requests
│       │   ├── stock.controller.js
│       │   ├── news.controller.js
│       │   └── ai.controller.js
│       │
│       ├── services/               # Handles API and business logic
│       │   ├── stock.service.js
│       │   ├── news.service.js
│       │   └── ai.service.js
│       │
│       ├── app.js
│       └── server.js
│
├── ai-service/                     # Python AI system
│   └── app/
│       ├── agents/
│       │   ├── stock_data_agent.py
│       │   ├── news_agent.py
│       │   ├── market_analysis_agent.py
│       │   └── research_agent.py
│       │
│       ├── orchestrator/
│       │   └── agent_orchestrator.py
│       │
│       ├── tools/
│       │   ├── stock_api.py
│       │   ├── news_api.py
│       │   └── llm_client.py
│       │
│       └── main.py
│
├── docs/                           # Project documentation
├── .gitignore                      # Files Git should ignore
└── README.md                       # Project overview
```

### 📌 Folder Description

| Folder/File | Purpose |
|---|---|
| `frontend/` | Displays stock data, charts, news, and AI responses. |
| `backend/` | Connects the frontend with external APIs and the AI service. |
| `routes/` | Defines the URLs used to access backend features. |
| `controllers/` | Handles requests and sends responses. |
| `services/` | Contains the main backend logic and API calls. |
| `agents/` | Contains individual AI agents for different tasks. |
| `orchestrator/` | Decides which agents to run and combines their results. |
| `tools/` | Contains reusable API and AI model connections. |
| `docs/` | Stores technical documentation. |
| `README.md` | Explains the project and how to use it. |

**Note:** This is the planned project structure. Files will be added as development continues.



## 📁 Project Structure and Purpose

The project is divided into three main parts: Frontend, Backend, and AI Service. Each part has a different responsibility.

### 1. Frontend — React.js

**Why is it used?**

The frontend is the part users see and interact with. It displays stock prices, charts, financial news, and AI-generated answers.

| File/Folder | Why is it used? |
|---|---|
| `components/` | Stores reusable UI elements. |
| `Navbar.jsx` | Provides navigation between pages. |
| `StockCard.jsx` | Displays important stock information. |
| `StockChart.jsx` | Shows stock price movements in a chart. |
| `NewsList.jsx` | Displays financial news articles. |
| `ChatInterface.jsx` | Allows users to ask questions about stocks. |
| `pages/` | Stores the main pages of the application. |
| `Dashboard.jsx` | Shows an overview of the stock market. |
| `StockDetails.jsx` | Displays details about a selected stock. |
| `ResearchAssistant.jsx` | Provides the interface for AI-based stock research. |
| `services/api.js` | Sends requests from the frontend to the backend. |
| `App.jsx` | Connects the main parts of the React application. |
| `main.jsx` | Starts the React application. |

### 2. Backend — Node.js and Express.js

**Why is it used?**

The backend connects the frontend with external APIs and the AI service. It receives requests, processes them, and sends responses to the frontend.

| File/Folder | Why is it used? |
|---|---|
| `routes/` | Defines the API endpoints of the application. |
| `stock.routes.js` | Defines endpoints for stock data. |
| `news.routes.js` | Defines endpoints for financial news. |
| `ai.routes.js` | Defines endpoints for AI-related requests. |
| `controllers/` | Handles incoming requests and prepares responses. |
| `stock.controller.js` | Handles stock-related requests. |
| `news.controller.js` | Handles news-related requests. |
| `ai.controller.js` | Handles requests for AI analysis. |
| `services/` | Contains the logic for working with APIs and other services. |
| `stock.service.js` | Fetches stock data from the selected API. |
| `news.service.js` | Fetches financial news. |
| `ai.service.js` | Connects the backend to the AI service. |
| `app.js` | Sets up Express and its middleware and routes. |
| `server.js` | Starts the backend server. |

### 3. AI Service — Python

**Why is it used?**

The AI service manages the different AI agents. Each agent performs a specific task, and the orchestrator coordinates their work.

| File/Folder | Why is it used? |
|---|---|
| `agents/` | Contains the individual AI agents. |
| `stock_data_agent.py` | Collects and organizes stock market data. |
| `news_agent.py` | Finds and summarizes financial news. |
| `market_analysis_agent.py` | Analyzes stock data and related news together. |
| `research_agent.py` | Combines the findings into a clear research report. |
| `orchestrator/` | Manages the workflow between the agents. |
| `agent_orchestrator.py` | Selects the required agents and combines their results. |
| `tools/` | Contains reusable tools for APIs and AI models. |
| `stock_api.py` | Handles communication with the stock market API. |
| `news_api.py` | Handles communication with the news API. |
| `llm_client.py` | Connects to the selected AI language model. |
| `main.py` | Starts the Python AI service. |

### 4. Other Important Files

| File/Folder | Why is it used? |
|---|---|
| `docs/` | Stores project documentation and design details. |
| `.gitignore` | Prevents unnecessary or sensitive files from being uploaded to GitHub. |
| `README.md` | Explains the project, its technologies, and how it works. |
| `requirements.txt` | Lists the Python packages needed for the AI service. |
| `package.json` | Lists Node.js dependencies and project scripts. |
| `.env` | Stores private settings such as API keys and configuration values. |

**Note:** This is the planned structure. These files will be created as the project develops. The actual structure should be updated to match the files implemented in the repository.
