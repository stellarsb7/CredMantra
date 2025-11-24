# CredMantra: A Production-Ready MLOps Pipeline for Credit Risk Assessment

## Project Overview

**CredMantra** is an end-to-end Machine Learning Operations (MLOps) project designed to **predict credit risk**, specifically focusing on loan default probability.

This repository provides a comprehensive and reproducible architecture for building, deploying, and monitoring a credit risk model. By implementing a robust MLOps pipeline, we ensure that the model is consistently trained, seamlessly deployed into a production environment using containers, and actively monitored for performance, data, and concept drift. This foundation is critical for reliable and automated financial decision-making.

---

## Tech Stack & Core Technologies

The project is built around modern MLOps principles, utilizing the following technologies:

| Category | Component/Technology | Role in Project |
| :--- | :--- | :--- |
| **Data & ML Development** | **Python**, **Jupyter Notebook** (28.9%) | Used for data exploration, cleaning, Feature Engineering, and Model Training/Development (e.g., Scikit-learn, Pandas). |
| **Containerization** | **Docker** (`Dockerfile`, `docker-compose.yml`) | Used to package the model, its dependencies, and the serving logic into lightweight, deployable containers. |
| **Deployment** | **Web Application/API** (`HTML` - 70.3%) | Provides a simple web interface for interaction and the core API for serving predictions. |
| **MLOps & Automation** | **Orchestration/Tracking Tools** (Implied) | The pipeline structure supports tools like **MLflow** for tracking experiments and **CI/CD** for automated build and release. |
| **Production Monitoring** | **Monitoring Tools** (Implied) | The system is structured to allow integration with tools like **Prometheus** and **Grafana** for observing model health and drift. |



---

## Repository Structure

The project follows a standard MLOps structure to separate development, deployment, and operational concerns:

| Folder | Description |
| :--- | :--- |
| `datasets` | Stores raw or processed data necessary for model training and testing. |
| `model_development` | Contains the training scripts and notebooks for model selection, training, and artifact serialization (saving the trained model). |
| `model_deployment` | Holds the code for the prediction API (e.g., Flask/FastAPI) and necessary configurations to serve the model. |
| `model_orchestration_and_tracking` | Setup files for defining the automated ML workflow and tracking model versions/experiments. |
| `monitoring` | Configuration files and scripts for setting up monitoring dashboards and alerts for the production model. |
| `images` | Contains visual assets, such as architecture diagrams or result visualizations, used in documentation. |
| `Dockerfile` & `docker-compose.yml` | Used to define the runtime environment and quickly deploy the entire application locally. |
