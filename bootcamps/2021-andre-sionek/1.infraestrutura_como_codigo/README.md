# 📝 Aula 01 — Infraestrutura como Código
- Conceitos de AWS e Cloudformation
- Criando buckets no S3
- Criando um banco de dados Redshift
- IAM / User / Roles / POlicies
- Criando um data stream usando Kinesis
- Integração Contínua
- Exercício: Deploy do Redash na AWS com IaC

## 👩🏻‍💻 Tópicos
### 📌 Criando Buckets no S3

1. **Criar o template** 
    - Código no GitHub
    - Navegando na documento do CloudFormation

        [What is AWS CloudFormation?](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html)

2. **Deploy usando o console**

    Abrir a AWS → Procurar por CLoudFormation → Ir em Stacks → Create stack

    Em Create Stack, colocar:

    - Template is ready
    - Upload a template file

        Baixar o arquivo YML criado anteriormente (template)

3. **Atualizar a stack usando o console**

    Atualizando a stack ao colocar opção de criptografia

4. **Excluir a stack usando o console** 

---

### 📌 Criando um cluster RedShift no S3

1. **Criar o template YML**

    Código no GitHub

2. **Deploy usando o console**

    Abrir a AWS → Procurar por CLoudFormation → Ir em Stacks → Create stack

    Em Create Stack, colocar:

    - Template is ready
    - Upload a template file

        Baixar o arquivo YML criado anteriormente (template)

3. **Testar o acesso**
4. **Modificar para permitir somente acesso a partir de endereços de IP específicos**

### 📌 Criando permissões para engenheiro de dados

1. **Criar o template**
    - Criar grupo
    - Criar role
    - Criar policy
2. **Deploy usando o console**
3. **Assumindo a função**
4. **Testando as permissões**

### 📌 Criando um data stream usando Kinesis

1. **Criar o template**
    - Criar Kinesis Data Stream
    - Criar KInesis Firehose para S3

        No arquivo Python voce precisa instalar antes o fake-web-events 

    - Criar chave de criptografia
2. **Testando em tempo real**

### 📌 Deploy Automático de Bucket S3

- Criar o template para GitHUb Actions
- Criar branch
- Commitar atualização e fazer push para o branch
