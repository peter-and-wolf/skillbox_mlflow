# Воспроизводимость в ML для Skillbox PRO

## Запуск MLflow-сервера

Следуйте инструкциям из [mlflow/README.md](mlflow/README.md).

## Конфигурация клиента MLFlow

Создайте (в той же директории, гда находится файл [main.ipynb](main.ipynb)) файл .env с таким содержанием: 

```bash
MLFLOW_S3_ENDPOINT_URL=http://localhost:9001
MLFLOW_TRACKING_URI=http://localhost:5050
AWS_ACCESS_KEY_ID=pmwGHCLBuSTM5eHzyWmB
AWS_SECRET_ACCESS_KEY=26GOdhDyvBP78wEPuh4nP76KPUbeSNjZKWXGINtq
```

> Обратите внимание, что значения переменных `AWS_ACCESS_KEY_ID` и `AWS_SECRET_ACCESS_KEY` должны совпадать с теми, которые вы установили при запуске [mlflow/docker-compose.yaml](mlflow/docker-compose.yaml) (см. [mlflow/README.md](mlflow/README.md)).

## Эксперименты

Запустите Jupyter-notebook и выполните [main.ipynb](main.ipynb).