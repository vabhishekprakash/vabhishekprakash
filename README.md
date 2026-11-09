## Hi, I'm Abhishek

Final-year CSE (AI & ML) student. 

Since July 2026 I've been part of the Handshake AI Fellowship, working to a US-based program's standards and review cycle. I was a reviewer there and was recently promoted to Specialist. My work covers several evaluation projects for frontier AI models:

- Writing multi-hop search questions built so a model can't reach the answer in a single search or recall it from memory. I check every fact against primary records such as court opinions and government registers, then test each draft against fresh sessions from two model families to find shortcuts and close them.
- Building Terminal-Bench 2 tasks that test whether AI coding agents can handle real engineering work in systems infrastructure, ML pipelines, data processing and databases. Each task ships with a Dockerised environment, a hidden test-based verifier and a working reference solution, goes in as a pull request, and has to clear two-stage human review and automated quality gates.
- Comparing two candidate responses in conversations that often include screenshots, charts or photos, picking the better one or marking both good or both weak, and stating the deciding difference.
- Creating realistic tasks and scoring rubrics for comparing model outputs.
- Writing prompts in which people ask an AI assistant for help with everyday activities.

I also completed an internship at AMIK Technologies, where I worked on a RAG-based support assistant and diagnosed charger faults from OCPP telemetry.

### Projects

- **[trust-aware-agent](https://github.com/vabhishekprakash/trust-aware-agent)**: a retrieval QA agent on a 3B local model that estimates the probability its own answer is right, then answers, asks, abstains or escalates based on that number. I preregistered the analysis and read the 100-item held-out split once. The result is negative and published as such: AUROC fell from 0.70 on development to 0.66 on test, and the tuned policy raised the error rate among the answers it showed. Signals read for free from the agent's trace did as well as the full feature set.
- **[amazon-ml-2026](https://github.com/vabhishekprakash/amazon-ml-2026)**: business entity resolution for the Amazon ML Challenge 2026. It links business listings from two sources to the entity each one describes, across the US, India and France. Candidates come from blocking on name, address and number keys, and a learned pre-ranker, five bagged LightGBM models and a fine-tuned multilingual cross-encoder score them. The final submission scored 0.979 macro F0.5 on the public leaderboard and 0.985 out of fold on the labelled US and India entities. We were a team of two: I designed and built the pipeline, and my teammate ran training jobs on his GPU and MacBook.
- **[surya-lekka](https://github.com/vabhishekprakash/surya-lekka)**: checks a household's rooftop solar quote before they sign. Amazon Textract reads the quote, the household confirms each number, and tested Python code checks the sums and the central subsidy rule. It runs on AWS Lambda, S3 and DynamoDB, and the [site is live](https://main.d2sqhcgne0nq26.amplifyapp.com/). On 9 held-out quotes, read once, the reader got 27 of 92 printed values right, which is why no finding appears until the household confirms its numbers. I built it with one teammate: I collected and labelled the quotes, ran the evaluation, made the product decisions and deployed it on AWS.
- **[Bail_Reckoner](https://github.com/vabhishekprakash/Bail_Reckoner)**: computes an undertrial prisoner's statutory entitlement to release under Section 479 of the BNSS, 2023. It walks six statutory gates in order, cites the provision behind each step, and abstains on offences it has not verified against the printed bare act (5 of 86 are signed so far). In its statute search, a cross-encoder reranker cut Recall@10 on natural-language queries from 0.921 to 0.684, so the shipped search leaves it out.
- **[ev-apm-agent](https://github.com/vabhishekprakash/ev-apm-agent)**: fault detection over OCPP telemetry from a 655-charger production fleet, validated on 39 of its stations. Rule-based detectors cover 6 fault categories, and a per-connector Isolation Forest flags drift with a 3.62% false-positive rate on a chronological holdout. Its own lead-time study found that the drift model gives no early warning before a fault. Built for the ET AI Hackathon 2026 in a team of three; I wrote the code.
- **[rag-eval-system](https://github.com/vabhishekprakash/rag-eval-system)**: a fully local RAG pipeline (FAISS, Mistral 7B via Ollama) benchmarked against a 28-question set I wrote over the OCPP specification. Both RAGAs metrics ranked a no-retrieval baseline above every retrieval configuration, while grading against the reference answers found that baseline correct on 0 of 23 answerable questions.
- **[AegisMesh](https://github.com/cyber-del/AegisMesh)**: a two-person hackathon project where an LLM reads correlated traces, logs and token metrics over MCP and patches live service config through a guardrail engine. I built the three instrumented FastAPI services, the OpenTelemetry setup and the self-hosted SigNoz deployment.

### Currently working on

- Reading about training models with AI feedback: so far [Constitutional AI](https://arxiv.org/abs/2212.08073) (Anthropic, 2022) and [RLAIF](https://arxiv.org/abs/2309.00267) (Lee et al., 2023).

**Tools I use in these projects:** Python, PyTorch, Hugging Face Transformers, LightGBM, scikit-learn, pandas, FAISS, LangChain, FastAPI, SQL, Docker, AWS (Lambda, S3, DynamoDB, Textract), OpenTelemetry, Unity, C#

[LinkedIn](https://www.linkedin.com/in/vallamalla-abhishek-prakash) · vabhishekprakash@gmail.com
