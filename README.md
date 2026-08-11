# Yigit Liman

**AI Master's Student @ FAU · IT Specialist @ TUM**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-yigitliman-0A66C2?logo=linkedin&logoColor=white)](https://linkedin.com/in/yigitliman)
[![Location](https://img.shields.io/badge/Munich-Germany-informational)](https://github.com/yigitliman)
[![Open to work](https://img.shields.io/badge/Open%20to-opportunities-success)](https://linkedin.com/in/yigitliman)

GPU scheduling, inference serving and ML platform infrastructure.
M.Sc. thesis at NHR@FAU on eBPF-based NFS I/O rate limiting for HPC clusters.

---

## Tech

**Core:** Python · Linux · eBPF
**ML:** PyTorch · XGBoost · scikit-learn · MLflow · Evidently
**Serving:** FastAPI · Docker · Docker Compose
**Orchestration:** Apache Airflow
**Monitoring:** Prometheus · Grafana
**LLM / RAG:** LangChain · ChromaDB · Anthropic Claude
**CI/CD:** GitHub Actions · GHCR

**Currently learning:** Kubernetes · Terraform

---

## Projects

### Infrastructure

| Project | What it does | Stack |
|---|---|---|
| [**gpu-scheduler**](https://github.com/yigitliman/gpu-scheduler) | Fair-share GPU cluster scheduler with EASY backfill and starvation-free job aging | Python, FastAPI, Prometheus, Grafana, Docker |
| [**llm-inference-server**](https://github.com/yigitliman/llm-inference-server) | Continuous-batching inference server with iteration-level scheduling and TTFT/throughput metrics | PyTorch, Transformers, FastAPI, Prometheus, Docker |
| [**ai-platform-lab**](https://github.com/yigitliman/ai-platform-lab) | Terraform + Kubernetes + monitoring learning lab, with remote state, a CI/CD pipeline and a Docker demo | Terraform, Kubernetes, GitHub Actions, Docker |

### Robotics

| Project | What it does | Stack |
|---|---|---|
| [**pepper-games**](https://github.com/yigitliman/pepper-games) | Voice games, tablet kiosk and web admin panel for a SoftBank Pepper robot, answered by a self-hosted LLM | Python, naoqi SDK, Whisper, gpt-oss-120b |

### MLOps

A learning series on one shared stack, where each project adds a piece the previous one did not have.

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
