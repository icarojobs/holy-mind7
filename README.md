# HOLY MIND7

Caso dê erro ao subir os containers, remover postgresql local.

## Gestão de Serviço - PostgreSQL

```bash
sudo systemctl status postgresql
sudo systemctl restart postgresql
sudo systemctl stop postgresql
sudo systemctl start postgresql
```

## Gestão de Serviço - Minio/S3:

```bash
# URL Dashboard (localhost): http://localhost:8900
# user: sail (localhost)
# pass: sail (localhost)
# Criar bucket com nome 'holy-mind7'  (sem as aspas simples)
```

## Gestão de Serviços - mailpit

```bash
# URL: http://localhost:8025
```

## Gestão de Serviços - rabbitmq

```bash
# URL: http://localhost:15672
# user: guest
# pass: guest
# criar a queue chamada 'default'
```

## Gestão de Serviços - meilisearch

```bash
# URL: http://localhost:7700
```
