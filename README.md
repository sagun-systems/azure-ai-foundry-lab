# Azure AI Foundry Implementation Lab (`AI-901`)

Hands-on engineering lab covering the Microsoft AI-901 (Azure AI Fundamentals) technical curriculum, focusing on Azure AI Foundry administration, Azure Content Understanding, multimodal inference, and responsible AI governance.

---

## 📂 Laboratory Architecture

| Module | Core Azure Technology | Implementation Scope |
| :--- | :--- | :--- |
| **`01-responsible-ai-content-safety`** | Azure AI Content Safety | Severity filtering (Hate, Violence, Sexual, Self-Harm), prompt injection jailbreak detection, and protected material controls. |
| **`02-content-understanding-multimodal`** | Azure Content Understanding | Unified multimodal extraction across scanned invoices, technical PDFs, and audio streams. |
| **`03-azure-openai-completions`** | Azure OpenAI Service / SDK | Structured outputs (`Pydantic`), function calling / tool integration, system message boundaries, and hyperparameter tuning (`temperature`, `top_p`). |
| **`04-vector-search-embeddings`** | Azure AI Search & Embeddings | Text-embedding generation, HNSW vector indexing, hybrid search (dense + BM25), and RAG context injection. |
| **`05-prompt-flow-evals`** | Microsoft Foundry Prompt Flow | Automated evaluation flows benchmarking Groundedness, Relevance, Fluency, and Coherence. |

---

## ⚙️ Environment Setup

```powershell
# Create and activate virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1

# Install required dependencies
pip install --upgrade pip
pip install -r requirements.txt

# Configure secrets
Copy-Item .env.example .env
