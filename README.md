# RAG-Guided-LLM-Rules
RAG-Guided LLM Rules – A Retrieval-Augmented Generation pipeline that teaches or enforces custom rules and guidelines for large language models. The system stores policies in a vector database and injects the most relevant rules into the model’s prompt at runtime, ensuring consistent, auditable responses without fine-tuning.

> **Teach or enforce rules for Large Language Models using Retrieval-Augmented Generation (RAG).**  
> Store your guidelines in a searchable knowledge base and dynamically retrieve them to steer model outputs.

---

## Overview
This project demonstrates how to **guide an LLM** to follow organization-specific rules or best practices **without fine-tuning**.

**Key Ideas**
- **Central rulebase:** Policies, style guides, or compliance requirements are stored as plain text or Markdown.
- **Retriever + Generator:** At query time, relevant rules are fetched from a vector database and injected into the prompt.
- **Auditable outputs:** Each response is traceable to the specific rules that influenced it.

---

## Features
- Framework-agnostic (LangChain, LlamaIndex, etc. compatible).
- Pluggable vector stores: FAISS by default; swap in Pinecone, Weaviate, or others.
- Configurable prompts, embedding models, and retrieval thresholds.

---

## Tech Stack
- **Language Model:** Llama3.2.
- **Vector DB:** FAISS
- **Python 3.9+** with standard scientific stack.

---
