# Yigit Liman

**AI Platform & Infrastructure Engineer** · IT Specialist @ TUM · M.Sc. Artificial Intelligence @ FAU

[Website](https://yigitliman.github.io) ·
[LinkedIn](https://linkedin.com/in/yigitliman) ·
Munich, Germany

M.Sc. thesis at NHR@FAU on eBPF-based NFS rate limiting for HPC clusters.

---

## Infrastructure

**[gpu-scheduler](https://github.com/yigitliman/gpu-scheduler)** ·
`Python` `FastAPI` `Prometheus` `Grafana` `Docker`

Fair-share scheduler for a shared GPU cluster: Slurm-style usage decay, job aging so
nothing starves, and EASY backfill. This is the formal version of the job queueing and
fair-use allocation I built for the cluster at TUM. On a seeded 400-job simulation over
8 GPUs, backfill takes utilisation from 89.5% to 99.5% and cuts mean queue wait by 20%.

**[llm-inference-server](https://github.com/yigitliman/llm-inference-server)** ·
`PyTorch` `Transformers` `FastAPI` `Prometheus` `Docker`

Continuous-batching inference server with iteration-level scheduling and KV-cache
bookkeeping, written against Hugging Face transformers rather than delegating to vLLM.
4.16x throughput at batch 16 versus sequential decoding, with inter-token latency going
from 19ms to 68ms. Batched output is byte-identical to a sequential baseline.

**[ai-platform-lab](https://github.com/yigitliman/ai-platform-lab)** ·
`Terraform` `Kubernetes` `LiteLLM` `Prometheus` `Grafana`

A LiteLLM gateway with master-key auth and rate limits in front of a local model,
Terraform for the AWS side with remote state and locking, a non-root service on
Kubernetes with probes, and Prometheus scraping both.

---

## MLOps

| Project | What it does | Stack |
|---|---|---|
| [**churn-prediction**](https://github.com/yigitliman/churn-prediction) | MLflow registry with alias promotion, Evidently drift checks, Prometheus metrics, K8s manifests with probes and an HPA | XGBoost, MLflow, Evidently, K8s |
| [**airflow-ml-pipeline**](https://github.com/yigitliman/airflow-ml-pipeline) | Scheduled retraining DAG with per-run artifact isolation and a ROC-AUC gate that fails the run instead of shipping a worse model | Airflow, MLflow, Docker Compose |
| [**document-qa**](https://github.com/yigitliman/document-qa) | RAG where retrieval itself is evaluated against a golden set, enforced in CI | LangChain, ChromaDB, Claude, FastAPI |

Same stack, different targets:
[price-prediction](https://github.com/yigitliman/price-prediction) (regression) ·
[anomaly-detection](https://github.com/yigitliman/anomaly-detection) (unsupervised) ·
[image-classifier](https://github.com/yigitliman/image-classifier) (PyTorch CNN) ·
[mlops-sentiment-pipeline](https://github.com/yigitliman/mlops-sentiment-pipeline) (multi-service Compose) ·
[ai-sentiment-api](https://github.com/yigitliman/ai-sentiment-api)
([live](https://yliman-ai-sentiment-api.hf.space))

---

## Robotics

**[pepper-games](https://github.com/yigitliman/pepper-games)** · `Python` `naoqi SDK` `Whisper`

Voice games, a tablet kiosk and a web admin panel for a SoftBank Pepper robot, with
answers from a self-hosted gpt-oss-120b. Built for teaching use at the chair.

---

## Tech

**Core:** Python · Linux · eBPF
**Platform:** Kubernetes · Terraform · Docker · GHCR
**Serving:** FastAPI · LiteLLM
**Monitoring:** Prometheus · Grafana
**Pipelines:** Apache Airflow · GitHub Actions · MLflow · Evidently
**ML / LLM:** PyTorch · XGBoost · scikit-learn · LangChain · ChromaDB · Anthropic Claude

Everything under Infrastructure and MLOps ships with tests, a GitHub Actions pipeline and
a container it runs in.
