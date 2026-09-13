## Hi, I'm Abhishek

Final-year CSE (AI & ML) student. I build tools that make opaque systems easier to understand, from fault detection on EV charging networks to evaluating RAG pipelines.

I'm Currently interning at AMIK Technologies, where I worked on a RAG-based support assistant and diagnosed charger faults from OCPP telemetry.

### Projects

- **[ev-apm-agent](https://github.com/vabhishekprakash/ev-apm-agent)**: fault detection over OCPP telemetry from a 655-charger production fleet. Rule-based detectors cover 6 fault categories, and a per-connector Isolation Forest flags drift with a 3.62% false-positive rate on a chronological holdout. Built for the ET AI Hackathon 2026.
- **[trust-aware-agent](https://github.com/vabhishekprakash/trust-aware-agent)**: a retrieval QA agent on a 3B local model that estimates the probability its own answer is right, and asks, abstains or escalates when that probability is low. The analysis was preregistered and the held-out split read once. The result is negative and published as such: confidence did not transfer to the test split, and the cheap signals read from the agent's trace matched the expensive ones.
- **[rag-eval-system](https://github.com/vabhishekprakash/rag-eval-system)**: a fully local RAG pipeline (FAISS, Mistral 7B via Ollama) with a RAGAs harness that compares chunking strategies.

### Currently working on

- **[Bail_Reckoner](https://github.com/vabhishekprakash/Bail_Reckoner)**: computes an undertrial prisoner's statutory entitlement to release under Section 479 of the BNSS, 2023. It walks six statutory gates in order and cites the provision behind each step, and its offence data is going through human review before any result is treated as verified.
- Reading about training models with AI feedback: so far [Constitutional AI](https://arxiv.org/abs/2212.08073) (Anthropic, 2022) and [RLAIF](https://arxiv.org/abs/2309.00267) (Lee et al., 2023).

**Tools I use in these projects:** Python, FastAPI, scikit-learn, pandas, FAISS, LangChain, SQL, Docker


[LinkedIn](https://www.linkedin.com/in/vallamalla-abhishek-prakash) · vabhishekprakash@gmail.com
