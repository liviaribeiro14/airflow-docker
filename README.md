# Airflow via container

Vídeo base: https://www.youtube.com/watch?v=aTaytcxy2Ck

yaml do compose: https://airflow.apache.org/docs/apache-airflow/stable/docker-compose.yaml

## Baixar as imagens
Na pasta raiz do projeto, criar o `.env`:
```bash
echo -e "AIRFLOW_UID=$(id -u)\nAIRFLOW_GID=0" > .env
```

Criar as pastas na raiz do projeto
```bash
mkdir ./dags ./plugins ./logs
```

Baixar as imagens do airflow.
```bash
docker-compose up airflow-init
```

## Subir ambiente
Na pasta raiz do projeto: 
```bash
docker-compose up
```

## Airflow no ar
URL: http://localhost:8080/

*user:* airflow

*password:* airflow