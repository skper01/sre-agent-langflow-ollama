# sre-agent-langflow-ollama

This project demonstrates a base model of an SRE Agent built with Langflow 1.5.13 and local Ollama models.
The agent can answer questions strictly from uploaded documents, avoiding hallucinations and providing a reliable foundation for building specialized DevOps/SRE assistants.

⚡️ This is just a base model — the sky is the limit. You can extend it with orchestration, monitoring integrations, IaC generation, and persistent memory.

🚀 Features

File ingestion: Upload files → processed and stored in ChromaDB.

No hallucinations: Prompt is designed so the agent only answers based on available knowledge.

Local AI models: Uses Ollama with openchat for conversational flow and deepseek for technical reasoning.

Multilingual: Ask in English or Spanish — the agent responds based on loaded documents.

Extendable: Add orchestration, monitoring, IaC generation, CI/CD automation, or persistent memory (Redis).

🛠️ Requirements

Langflow 1.5.13

Python 3.10+

Ollama installed locally

Download Ollama

After installation, pull the required models:

ollama pull openchat
ollama pull deepseek

ChromaDB (installed as Python package or containerized)



▶️ Usage

Import flow.json into Langflow 1.5.13.

Upload your documents (PDF, TXT, etc.).

Ask your questions in English or Spanish.

The agent will only answer based on the uploaded content.


🌐 Example Use Case

Upload your SRE runbooks or incident postmortems.

Ask: “What were the top root causes of outages last year?”

The agent replies only using the uploaded documentation.


🔮 Next Steps

This base model can be extended into:

Monitoring Agent: integrate with New Relic or PagerDuty.

IaC Agent: generate Terraform or Ansible configs.

CI/CD Agent: connect with GitHub Actions for automated deployments.

Persistent Memory: add Redis or Memory nodes so it remembers past conversations.


📖 References

Langflow Documentation

Ollama

New Relic Service Levels
