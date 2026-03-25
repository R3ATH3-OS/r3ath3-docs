# R3@TH3 OS – Model Layer Overview

The Model Layer provides the intelligence resources used by agents in R3@TH3 OS.  
It includes local LLMs, embeddings, vector databases, and connectors to external models when explicitly allowed.

## Components of the Model Layer

1. **Local LLMs**  
   GPU‑accelerated models running on the RTX 4060.  
   Used for reasoning, planning, summarization, and agent decision-making.

2. **Embedding Models**  
   Lightweight models used for semantic search, memory retrieval, and vector-based reasoning.

3. **Vector Store**  
   A local database that stores embeddings for documents, logs, workflows, and agent knowledge.

4. **External Model Connectors (Optional)**  
   Only used when explicitly permitted.  
   Examples: Perplexity Compute, ChatGPT, or other remote inference endpoints.

## Model Selection Principles

- Local-first  
- Privacy-preserving  
- Explainable  
- Efficient on consumer hardware  
- Modular and replaceable  

## How Models Interact with Agents

- Agents request reasoning or generation from local LLMs  
- Agents store and retrieve embeddings from the vector store  
- Coordinators use models to plan multi-step workflows  
- Observer agents use models to classify anomalies or patterns  
- Interface agents use models to communicate with the user  

## Why This Layer Matters

The Model Layer gives R3@TH3 OS:

- fast, private, GPU-accelerated intelligence  
- the ability to run multiple agents in parallel  
- semantic memory and long-term context  
- the foundation for explainable, local-first AI  
