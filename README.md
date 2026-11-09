## Hi, I'm Abhishek

Final-year CSE (AI & ML) student. I build ML and LLM systems, test them on held-out data, and publish the results even when they're negative.

I'm a Specialist in the Handshake AI Fellowship, promoted from reviewer, and have worked there since July 2026. I build evaluation tasks for frontier AI models: multi-hop search questions checked against primary records, Terminal-Bench 2 tasks with Docker environments and hidden test verifiers, and rubric-based comparisons of model outputs, including conversations with images. I also completed an internship at AMIK Technologies, working on a RAG-based support assistant and on charger-fault diagnosis from OCPP telemetry.

### Projects

- **[trust-aware-agent](https://github.com/vabhishekprakash/trust-aware-agent)**: a retrieval QA agent on a local 3B model that estimates how likely its own answer is to be right, then answers, asks, abstains or escalates. I preregistered the evaluation and read the held-out split once. The result was negative (AUROC 0.70 on development, 0.66 on test), and the repo reports it that way.
- **[amazon-ml-2026](https://github.com/vabhishekprakash/amazon-ml-2026)**: entity resolution for the Amazon ML Challenge 2026, using blocking, LightGBM and a fine-tuned multilingual cross-encoder. It scored 0.979 macro F0.5 on the public leaderboard. I designed and built the pipeline; my teammate ran training jobs on his machines.
- **[surya-lekka](https://github.com/vabhishekprakash/surya-lekka)**: checks a household's rooftop solar quote before they sign. Amazon Textract reads it, the household confirms the numbers, and tested Python code checks the sums and the subsidy rule. Serverless on AWS, with a [live site](https://main.d2sqhcgne0nq26.amplifyapp.com/). Team of two; I did the data, evaluation, product decisions and AWS deployment.
- **[Bail_Reckoner](https://github.com/vabhishekprakash/Bail_Reckoner)**: computes an undertrial prisoner's statutory entitlement to release under Section 479 BNSS, 2023, cites the provision behind each step, and abstains on any offence nobody has verified against the printed act. Its retrieval study found that a cross-encoder reranker cut Recall@10 from 0.921 to 0.684.
- **[ev-apm-agent](https://github.com/vabhishekprakash/ev-apm-agent)**: fault and drift detection over OCPP telemetry from a 655-charger production fleet, with rule-based detectors for 6 fault categories and per-connector Isolation Forests. Hackathon team of three; I wrote the code.
- **[rag-eval-system](https://github.com/vabhishekprakash/rag-eval-system)**: a local RAG pipeline and a 28-question OCPP benchmark. RAGAs ranked a no-retrieval baseline above every retrieval setup, though that baseline was correct on 0 of 23 answerable questions.
- **[AegisMesh](https://github.com/cyber-del/AegisMesh)**: a two-person hackathon project where an LLM controller patches live service config through a guardrail engine. I built the OpenTelemetry-instrumented FastAPI services and the self-hosted SigNoz deployment.

### Currently working on

- Reading about training models with AI feedback: so far [Constitutional AI](https://arxiv.org/abs/2212.08073) (Anthropic, 2022) and [RLAIF](https://arxiv.org/abs/2309.00267) (Lee et al., 2023).

**Tools I use in these projects:** Python, PyTorch, Hugging Face Transformers, LightGBM, scikit-learn, pandas, FAISS, LangChain, FastAPI, SQL, Docker, AWS (Lambda, S3, DynamoDB, Textract), OpenTelemetry, Unity, C#

[LinkedIn](https://www.linkedin.com/in/vallamalla-abhishek-prakash) · vabhishekprakash@gmail.com
