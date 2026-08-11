# Yigit Liman

**AI Master's Student @ FAU · IT Specialist @ TUM**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-yigitliman-0A66C2?logo=linkedin&logoColor=white)](https://linkedin.com/in/yigitliman)
[![Location](https://img.shields.io/badge/Munich-Germany-informational)](https://github.com/yigitliman)
[![Open to work](https://img.shields.io/badge/Open%20to-opportunities-success)](https://linkedin.com/in/yigitliman)

**AI Platform & HPC Infrastructure Engineer**

M.Sc. thesis at NHR@FAU on eBPF-based NFS rate limiting for HPC clusters

---

## Tech

**Core:** Python · Linux · eBPF
**Platform:** Kubernetes · Terraform
**Serving:** FastAPI · Docker · Docker Compose
**Orchestration:** Apache Airflow
**CI/CD:** GitHub Actions · GHCR
**Monitoring:** Prometheus · Grafana
**ML:** PyTorch · XGBoost · scikit-learn · MLflow · Evidently
**LLM / RAG:** LangChain · ChromaDB · Anthropic Claude

---

## Projects

### Infrastructure

| Project | What it does | Stack |
|---|---|---|
| [**ai-platform-lab**](https://github.com/yigitliman/ai-platform-lab) | End-to-end AI platform: Terraform-provisioned Kubernetes with remote state, monitoring and a CI/CD pipeline shipping containers to the cluster | Terraform, Kubernetes, GitHub Actions, Docker |
| [**gpu-scheduler**](https://github.com/yigitliman/gpu-scheduler) | Fair-share GPU cluster scheduler with EASY backfill and starvation-free job aging | Python, FastAPI, Prometheus, Grafana, Docker |
| [**llm-inference-server**](https://github.com/yigitliman/llm-inference-server) | Continuous-batching inference server with iteration-level scheduling and TTFT/throughput metrics | PyTorch, Transformers, FastAPI, Prometheus, Docker |

### Robotics

| Project | What it does | Stack |
|---|---|---|
| [**pepper-games**](https://github.com/yigitliman/pepper-games) | Voice games, tablet kiosk and web admin panel for a SoftBank Pepper robot, answered by a self-hosted LLM | Python, naoqi SDK, Whisper, gpt-oss-120b |

### MLOps

One shared stack across the series, where each project adds a piece the previous one did not have.

| Project | What it does | Stack |
|---|---|---|
| [**churn-prediction**](https://github.com/yigitliman/churn-prediction) | The baseline of the series: a model registry and drift detection wired into a serving API | XGBoost, MLflow, Evidently, Prometheus, Docker, K8s |
| [**price-prediction**](https://github.com/yigitliman/price-prediction) | Same pipeline pointed at a regression target, so the metrics are errors rather than class scores | XGBoost, MLflow, Evidently, FastAPI, Docker |
| [**anomaly-detection**](https://github.com/yigitliman/anomaly-detection) | Drops the labels entirely and scores sensor readings with an unsupervised model | IsolationForest, MLflow, Evidently, FastAPI, Docker |
| [**airflow-ml-pipeline**](https://github.com/yigitliman/airflow-ml-pipeline) | Takes training off my machine into a scheduled DAG that retrains when drift crosses a threshold | Airflow, MLflow, Docker Compose |
| [**image-classifier**](https://github.com/yigitliman/image-classifier) | First GPU-trained deep learning model here, a CIFAR-10 CNN behind the same API shape | PyTorch, MLflow, FastAPI, Docker |
| [**document-qa**](https://github.com/yigitliman/document-qa) | Answers from retrieved documents instead of a trained model, and evaluates the retrieval itself | LangChain, ChromaDB, Claude, FastAPI, Docker |
| [**mlops-sentiment-pipeline**](https://github.com/yigitliman/mlops-sentiment-pipeline) | Splits the single container into a multi-service Compose stack with a transformer doing inference | DistilBERT, MLflow, Evidently, FastAPI, Docker Compose |

Every MLOps and Infrastructure project ships with tests, a Dockerfile, and a GitHub Actions pipeline.
