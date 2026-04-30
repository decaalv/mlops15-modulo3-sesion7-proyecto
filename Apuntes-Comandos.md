## Paso 0: Vinculación
gcloud init

## Paso 1: Creación del repositorio en Artifact Registry (GCP)
gcloud artifacts repositories create repositorio-mlops15-sesion7-proyecto-ml --repository-format docker --project modulo3-sesion7-proyecto
 --location us-central1

## Paso 2: Crear el repo de github

## Paso 3: Crear la Key de la Cuenta de Servicio

## Paso 4: Colocar el Service Account Key en GitHub Settings
- Debes ir a Secrets and variables
- Luego a Actions
- Clic en New repository secret
- El nombre del Secreto es "GCP_SERVICE_ACCOUNT_KEY"

## Paso Automatizacion:
- git init
- git add .
- git commit -m "Proyecto de automatización de despliegue en GCR"
- git branch -M main
- git remote set-url origin https://github.com/KevinInoCol/MLOps-Deploy-GCP-Actions.git
- git remote add origin https://github.com/KevinInoCol/mlops-14-ml-regression-casas-streamlit.git
- git push -u origin main



## Cuando deseas volver a subir por algun error corres lo siguiente:
- git status
- git add .
- git commit -m "Ajustes en workflow de CI/CD"
- git push

