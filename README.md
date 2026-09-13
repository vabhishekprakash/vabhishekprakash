## Hi, I'm Abhishek

Final-year CSE (AI & ML) student. I build tools that make opaque systems easier to understand, and I try to measure honestly how well they work.

I'm currently interning at AMIK Technologies, where I work on a RAG-based support assistant and diagnose charger faults from OCPP telemetry.

### Projects

- **[trust-aware-agent](https://github.com/vabhishekprakash/trust-aware-agent)**: a retrieval QA agent on a 3B local model that estimates the probability its own answer is right, then answers, asks, abstains or escalates based on that number. I preregistered the analysis and read the held-out split once. The result is negative and published as such: the confidence estimate did not transfer to the test split.
- **[ev-apm-agent](https://github.com/vabhishekprakash/ev-apm-agent)**: fault detection over OCPP telemetry from a 655-charger production fleet. Rule-based detectors cover 6 fault categories, and a per-connector Isolation Forest flags drift with a 3.62% false-positive rate on a chronological holdout. Built for the ET AI Hackathon 2026.
- **[rag-eval-system](https://github.com/vabhishekprakash/rag-eval-system)**: a fully local RAG pipeline (FAISS, Mistral 7B via Ollama) with a RAGAs harness that compares chunking strategies against a 28-question evaluation set I wrote over the OCPP specification, including five questions the document does not answer.
- **[Bail_Reckoner](https://github.com/vabhishekprakash/Bail_Reckoner)**: computes an undertrial prisoner's statutory entitlement to release under Section 479 of the BNSS, 2023. It walks six statutory gates in order and cites the provision behind each step, and its offence data is going through human review before any result is treated as verified.
- **[AegisMesh](https://github.com/cyber-del/AegisMesh)**: a two-person hackathon project where an LLM reads correlated traces, logs and token metrics over MCP and patches live service config through a guardrail engine. I built the three instrumented FastAPI services, the OpenTelemetry setup and the self-hosted SigNoz deployment.

### Currently working on

- Reading about training models with AI feedback: so far [Constitutional AI](https://arxiv.org/abs/2212.08073) (Anthropic, 2022) and [RLAIF](https://arxiv.org/abs/2309.00267) (Lee et al., 2023).

**Tools I use in these projects:** Python, FastAPI, scikit-learn, pandas, FAISS, LangChain, SQL, Docker, Unity, C#

[LinkedIn](https://www.linkedin.com/in/vallamalla-abhishek-prakash) · vabhishekprakash@gmail.com
