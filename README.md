# Yigit Liman

**AI Master's Student @ FAU · IT Specialist @ TUM**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-yigitliman-0A66C2?logo=linkedin&logoColor=white)](https://linkedin.com/in/yigitliman)
[![Location](https://img.shields.io/badge/Munich-Germany-informational)](https://github.com/yigit-8)
[![Open to work](https://img.shields.io/badge/Open%20to-opportunities-success)](https://linkedin.com/in/yigitliman)

Learning MLOps by building end to end: model training, experiment tracking, deployment, and monitoring.

---

## Tech

**ML:** XGBoost · PyTorch · scikit-learn · MLflow · Evidently
**Serving:** FastAPI · Docker · Docker Compose
**Orchestration:** Apache Airflow · Kubernetes · Terraform
**Monitoring:** Prometheus · Grafana
**LLM / RAG:** LangChain · ChromaDB · Anthropic Claude
**CI/CD:** GitHub Actions · GHCR

---

## Projects

### MLOps

| Project | What it does | Stack |
|---|---|---|
| [**churn-prediction**](https://github.com/yigit-8/churn-prediction) | Churn API with model registry, drift + Prometheus monitoring, and Kubernetes manifests | XGBoost, MLflow, Evidently, Prometheus, Docker, K8s |
| [**price-prediction**](https://github.com/yigit-8/price-prediction) | California house-price regression API | XGBoost, MLflow, Evidently, FastAPI, Docker |
| [**anomaly-detection**](https://github.com/yigit-8/anomaly-detection) | Unsupervised sensor anomaly detection | IsolationForest, MLflow, Evidently, FastAPI, Docker |
| [**airflow-ml-pipeline**](https://github.com/yigit-8/airflow-ml-pipeline) | Scheduled training pipeline with drift-triggered retraining | Airflow, MLflow, Docker Compose |
| [**image-classifier**](https://github.com/yigit-8/image-classifier) | CIFAR-10 CNN served over an API | PyTorch, MLflow, FastAPI, Docker |
| [**document-qa**](https://github.com/yigit-8/document-qa) | RAG document Q&A with source citations and retrieval evaluation | LangChain, ChromaDB, Claude, FastAPI, Docker |
| [**mlops-sentiment-pipeline**](https://github.com/yigit-8/mlops-sentiment-pipeline) | Sentiment pipeline with experiment tracking, drift detection and a two-service Compose stack | DistilBERT, MLflow, Evidently, FastAPI, Docker Compose |

### Infrastructure

| Project | What it does | Stack |
|---|---|---|
| [**gpu-scheduler**](https://github.com/yigit-8/gpu-scheduler) | Fair-share GPU cluster scheduler with EASY backfill and starvation-free job aging | Python, FastAPI, Prometheus, Grafana, Docker |
| [**llm-inference-server**](https://github.com/yigit-8/llm-inference-server) | Continuous-batching inference server with iteration-level scheduling and TTFT/throughput metrics | PyTorch, Transformers, FastAPI, Prometheus, Docker |
| [**ai-platform-lab**](https://github.com/yigit-8/ai-platform-lab) | Terraform + Kubernetes + monitoring learning lab, with remote state, a CI/CD pipeline and a Docker demo | Terraform, Kubernetes, GitHub Actions, Docker |

### Robotics

| Project | What it does | Stack |
|---|---|---|
| [**pepper-games**](https://github.com/yigit-8/pepper-games) | Voice games, tablet kiosk and web admin panel for a SoftBank Pepper robot, answered by a self-hosted LLM | Python, naoqi SDK, Whisper, gpt-oss-120b |

Every MLOps and Infrastructure project ships with tests, a Dockerfile, and a GitHub Actions pipeline.

---

<p align="left">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=yigit-8&show_icons=true&hide_title=true&hide_border=true&count_private=true&theme=default" alt="Yigit's GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=yigit-8&layout=compact&hide_border=true&theme=default" alt="Top languages" />
</p>
