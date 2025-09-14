# 🏎️ F1 Race Podium Predictor

Predict podium probabilities for Formula 1 races using historical data, ML pipelines, and a cloud-native deployment.

## 🚀 Features
- End-to-end ML pipeline (ETL → feature engineering → training → deployment).
- Nightly retraining with GitHub Actions.
- REST API (Azure Functions) for predictions.
- Cosmos DB (serverless, free tier) for metadata & logs.
- Authentication with Microsoft Entra External ID.
- Simple dashboard frontend (Next.js/Vite).
- Free-tier friendly: runs mostly at $0.

## 📂 Repo Structure
- `api/` — Azure Functions for serving predictions.
- `training/` — Feature engineering + model training pipeline.
- `infra/` — IaC for Azure setup (Bicep/Terraform).
- `frontend/` — Dashboard to visualize predictions.
- `.github/workflows/` — CI/CD workflows.
- `data/` — F1DB snapshot for local dev.
