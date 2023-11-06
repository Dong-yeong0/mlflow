# Setup MLflow + Minio(s3)

## Set environment variables for MLflow, Minio, postgreSQL

`docker/mlflow-minio-postgre/.env_template`에 각각 원하는 환경변수를 설정합니다.  
(**미기입 시 docker-compose up 때 오류가 발생합니다.**)

```json
MLFLOW_POSTGRES_USER=
MLFLOW_POSTGRES_PASSWORD=
MLFLOW_POSTGRES_DB=
MLFLOW_POSTGRES_PORT=

MLFLOW_MINIO_APP_PORT=
MLFLOW_MINIO_WEB_PORT=
MLFLOW_MINIO_ROOT_USER=
MLFLOW_MINIO_ROOT_PASSWORD=

MLFLOW_SERVER_PORT=
```

## Run MLflow + Minio

아래 커멘드로 MLflow + Minio를 실행합니다.

```shell
cd .\docker\mlflow-minio-postgre\
docker-compose up -d
```
