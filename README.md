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

## Gestão de Serviços - pgAdmin (PostgreSQL)

```bash
# URL: http://localhost:5050/
# user: hello@example.com
# pass: password
```

## GERANDO BASELINE DO LARASTAN/PHPSTAN

Caso necessário (e isso não é uma boa prática), podemos gerar um arquivo do phpstan/larastan para ignorar os warnings e
erros encontrados com o seguinte comando:

```bash
./vendor/bin/sail bin phpstan --generate-baseline
```

## **Atenção:** Após verificar os warnings e erros, pague o débito técnico para evitar bugs futuramente.

## CRIANDO TESTES DE INTEGRAÇÃO COM PEST

Nesse projeto já estamos utilizando as últimas atualizações do Laravel (11) e do Pest (3).
Para criar testes de frontend, basta digitar o seguite comando:

```bash
sail art pest:test Frontend/NomeXptoTest
```

Esse comando vai criar o seu arquivo em `/tests/Feature/Frontend/NomeXptoTest`

**Atenção:** O arquivo PRECISA ter o `sufixo` como `Test`.

---

## CRIANDO TESTES E2E (FRONTEND) COM DUSK

Para criar um novo arquivo de testes E2E com Laravel Dusk, basta executar o seguinte comando:

```bash
sail art dusk:make Frontend/HomeTest

# ou

sail art dusk:make Backend/CompaniesTest
```

## EXECUTANDO TESTES E2E (FRONTEND) COM DUSK (E SAIL)

Para executar sua bateria de testes de frontend, você pode utilizar os seguintes comandos:

```bash
sail dusk

# Ou separado por grupos
sail dusk --group=validation
```

---

## REFERÊNCIAS

gitflow:
[https://danielkummer.github.io/git-flow-cheatsheet/](https://danielkummer.github.io/git-flow-cheatsheet/)

docker: [https://docs.docker.com/desktop/install/ubuntu/](https://docs.docker.com/desktop/install/ubuntu/)

Make: [https://www.gnu.org/software/make/manual/make.html](https://www.gnu.org/software/make/manual/make.html)

cURL: [https://curl.se/docs/](https://curl.se/docs/)
