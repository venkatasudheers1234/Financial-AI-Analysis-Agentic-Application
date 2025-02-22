
**Financial AI Agent Application**

**Overview**

The Financial AI Agent Project is an AI-driven application designed for financial analysis and web search functionalities using Python. This project utilizes the phi library to create AI agents capable of accessing and analyzing financial data and conducting web searches. It integrates OpenAI's GPT models for generating natural language responses and employs YFinanceTools for financial data retrieval.

**Features**

Web Search Agent: An AI agent that searches the web for information using the DuckDuckGo tool, always including sources in its responses.

Financial AI Agent: An AI agent focused on financial data retrieval and analysis, providing information on stock prices, analyst recommendations, stock fundamentals, and company news.

Interactive Application: A user-friendly interface created using the Playground class, allowing for easy interaction with the AI agents.

**Environment Setup**

Ensure you have a .env file with the necessary API keys:

PHI_API_KEY=your_phi_api_key
OPENAI_API_KEY=your_openai_api_key

Load the environment variables:
python
from dotenv import load_dotenv
load_dotenv()

**Agents**

Web Search Agent

Name: Web Search Agent

Role: Search the web for information

Model: Groq

Tools: DuckDuckGo

Instructions: Always include sources, show tool calls, and use Markdown format



Financial AI Agent

Name: Finance AI Agent

Model: Groq

Tools: YFinanceTools (stock price, analyst recommendations, stock fundamentals, company news)

Instructions: Use tables to display data, show tool calls, and use Markdown format


**Usage**

Interact with the AI agents through the user-friendly interface provided by the Playground app. For example, use the financial AI agent to get stock information, analyst recommendations, and company news.

financial agent.py
This file demonstrates the creation of a multi-agent instance, combining the web search agent and financial AI agent, and provides an example of how to use the multi-agent for summarizing analyst recommendations and sharing the latest news for a specific stock.

**Technologies Used: **

 **Python 3.7+**
 
- **OpenAI GPT**: Language model used for generating natural language responses.
- 
- **phi**: Library used to create AI agents and manage interactions.
- 
- **YFinanceTools**: Tool used for financial data retrieval.
- 
- **DuckDuckGo**: Tool used for web search functionalities.
- 
- **dotenv**: Library for managing environment variables.

**Future Enhancements**

Adding more sophisticated financial analysis tools.

Integrating additional data sources for comprehensive financial insights.

Improving the user interface for better interaction and visualization of data.

