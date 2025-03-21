# AIkube  




## Design Doc

### Problem Definition  

- Generalized AI/ML Systems orchestration with Kubernetes as the control plane  

### Data Science  

- Data Collection & Preprocessing  

```
BigQuery → Serverless data warehouse for large-scale analytics.
Cloud Storage → Object storage for raw datasets, model artifacts, etc.
Cloud SQL / Spanner / Firestore → Managed relational and NoSQL databases.
Pub/Sub → Real-time data ingestion and streaming.
Dataflow (Apache Beam) → Managed stream and batch data processing.
Dataplex → Data governance and management.

```


### Data Eng  

- Data Processing & Feature Engineering  


```
Dataproc (Apache Spark, Hadoop) → Managed big data processing.
Dataflow → ETL (Extract, Transform, Load) for real-time and batch pipelines.
BigQuery ML (BQML) → Run ML models directly on BigQuery.
Vertex AI Feature Store → Centralized feature management and reuse.


```




### ML Eng  

- Model Selection Development & Training  

```
Vertex AI Workbench → Jupyter-based notebooks for ML development.
AI Platform Training (Vertex AI Custom Training) → Train models at scale with GPUs/TPUs.
Deep Learning VM (DLVM) → Pre-configured VMs with TensorFlow, PyTorch, JAX, etc.
TPU (Tensor Processing Units) → Specialized hardware for deep learning.
Kubeflow on GKE → ML pipelines and orchestration on Kubernetes.
AutoML (Vertex AI AutoML) → Train ML models with minimal expertise.


```

- Model Evaluation & Explainability  


```
Vertex AI Experiments → Track ML model training experiments.
Vertex AI Explainability → Interpretability of AI models using SHAP, LIME.
TensorBoard on Vertex AI → Visualize training metrics, loss curves.
```

### ML Ops  

- Model Deployment  

```
Vertex AI Prediction → Managed service for serving ML models.
AI Platform Prediction (Legacy) → Model hosting service.
Cloud Run → Serverless containerized model deployment.
GKE (Google Kubernetes Engine) → Scalable containerized deployment.
Cloud Functions → Lightweight serverless inference.

```

- Monitoring & Maintenance  

```
Vertex AI Pipelines → Managed ML pipeline orchestration (like Kubeflow).
Vertex AI Model Monitoring → Detect model drift, bias, and performance degradation.
Cloud Logging & Monitoring → Track logs and metrics for ML workflows.
Cloud Composer (Apache Airflow) → Workflow automation for ML pipelines.

```


- Automated Retraining, Continuous Improvement & Retraining  

```
Cloud Composer (Airflow) + Vertex AI Pipelines → Automate retraining when data drift is detected.
Cloud Functions + Cloud Scheduler → Schedule model retraining at fixed intervals.
BigQuery ML + AutoML Retraining → Auto-retrain models directly from BigQuery.

```


- Model Explainability Security & Compliance  

```
IAM (Identity & Access Management) → Secure access to ML resources.
VPC Service Controls → Restrict access to ML services.
DLP API (Data Loss Prevention) → Mask sensitive data in ML workflows.

```








