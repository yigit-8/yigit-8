# yigit-8

**AI Master's Student @ FAU · IT Specialist @ TUM**

Learning MLOps by building end to end: model training, experiment tracking, deployment, and monitoring.

[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-Live%20Demo-FFD21E?logo=huggingface&logoColor=black)](https://yliman-churn-prediction.hf.space/docs)

---

## Tech

**ML:** XGBoost · PyTorch · scikit-learn · MLflow · Evidently
**Serving:** FastAPI · Docker · Docker Compose
**Orchestration:** Apache Airflow · Kubernetes
**Monitoring:** Prometheus · Grafana
**LLM / RAG:** LangChain · ChromaDB · Anthropic Claude
**CI/CD:** GitHub Actions · GHCR

---

## Projects

| Project | What it does | Stack |
|---|---|---|
| [**churn-prediction**](https://github.com/yigit-8/churn-prediction) · [live demo](https://yliman-churn-prediction.hf.space/docs) | Churn API with model registry, drift + Prometheus monitoring, and Kubernetes manifests | XGBoost, MLflow, Evidently, Prometheus, Docker, K8s |
| [**price-prediction**](https://github.com/yigit-8/price-prediction) | California house-price regression API | XGBoost, MLflow, Evidently, FastAPI, Docker |
| [**anomaly-detection**](https://github.com/yigit-8/anomaly-detection) | Unsupervised sensor anomaly detection | IsolationForest, MLflow, Evidently, FastAPI, Docker |
| [**airflow-ml-pipeline**](https://github.com/yigit-8/airflow-ml-pipeline) | Scheduled training pipeline with drift-triggered retraining | Airflow, MLflow, Docker Compose |
| [**image-classifier**](https://github.com/yigit-8/image-classifier) | CIFAR-10 CNN served over an API | PyTorch, MLflow, FastAPI, Docker |
| [**document-qa**](https://github.com/yigit-8/document-qa) | RAG document Q&A with source citations and retrieval evaluation | LangChain, ChromaDB, Claude, FastAPI, Docker |

Every project ships with tests, a Dockerfile, and a GitHub Actions pipeline.
