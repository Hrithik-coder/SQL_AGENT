# SQL_AGENT
An autonomous AI Agent designed to interact with SQL databases using a ReAct (Reasoning and Acting) loop. This agent doesn't just run SQL.it validates intent, retrieves relevant schema context using a Vector Database

Intent Classification: Prevents off-topic queries or prompt injections.

Semantic Schema Retrieval: Uses Qdrant and Sentence-Transformers to provide the LLM with only the relevant table/column metadata.

Autonomous Loop: Powered by LangGraph, allowing the agent to perform multi-step tasks (e.g., "Update X and then show me the average of Y").


# Tech Stack
Language : Python 3.10+

LLM Orchestration : LangGraph & LangChain

LLM : Groq (openai/gpt-oss-20b)

Vector DB : Qdrant (In-memory)

Database : SQLite

Embeddings : HuggingFace (all-mpnet-base-v2)

# Table Details

"name": The full name of the employee which is unique

"designation": The job title or role

"department": The department name (AI, HR, Sales)

"salary": The numeric value representing annual pay

"id": The unique primary key


### 1. Prerequisites
Ensure you have Python 3.10+ installed. You will also need a **Groq API Key**.

### 2. Installation
```bash
# Clone the repository
git clone "[git repo](https://github.com/Hrithik-coder/SQL_AGENT.git)"

cd agentic-sql-analyst

# Install dependencies
pip install -r requirements.txt
