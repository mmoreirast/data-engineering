# 📝 Aula 03 — Apache Airflow + Spark
- Conceitos de Airflow
- Deploy de Airflow com ECS Fargate (IaC)
- Extraindo dados de uma API para o Data Lake com Docker OPerator
- Transformação com Spark Streaming em AWS EMR
- Criando DAG para executar queries SQL
- **Exercício:** Ingerir dados de uma API pública, processar e disponibilizar

## 👩🏻‍💻 Tópicos
### 📌 Airflow Local com Docker

1. **Repositório puckel/docker-airflow**
2. **Verificar DockFile**
3. **Deploy local**
    - docker pull puckel/docker-airflow
    - docker run -d -p 8080:8080 -e LOAD_EX=y puckel/docker-airflow webserver
4. **Navegar na UI**
    - localhost:8080

---

### 📌 Deploy de Airflow com ECS Fargate (IaC)

1. **Estudar o template CloudFormation airflow-autoscaling-ecs**
    - ECS Fargate + ECR
    - Autoscaling
    - Banco de metadados
2. **Criar Dockerfile**
3. **Testar UI**
    - localhost:8080

---

### 📌 Extraindo Dados de uma API com Airflow + Docker

1. **Criar script Pyhton para realizar extração e ingestão para o data lake**
2. **Criar imagem**
    - Subir para ECR
3. **Criar DAG para executar container**

---

### 📌 Transformação com Spark Streaming em AWS EMR

1. **Criar job PySpark para transformar de raw para processed**
2. **Criar template**
    - EMR
3. **Iniciar cluster**
4. **Verificar se dados foram processados com Athena**

---

### 📌 Criando DAGs para executar queries SQL

1. **Criar DAG para executar queries no Athena**
    - Criar tabela de sessões
    - Criar tabela de métricas a partir das sessões
