# 🚀 Desafio DIO: CloudFormation 2 — Infraestrutura Automatizada na AWS

Este repositório documenta minha participação no segundo desafio de CloudFormation da DIO, onde implementei uma infraestrutura simples e funcional na AWS utilizando um template YAML. O objetivo foi aplicar os conceitos de infraestrutura como código (IaC), testar recursos reais e registrar todo o processo técnico.

---

## 🎯 Objetivo do Desafio

- Criar uma stack automatizada com AWS CloudFormation
- Provisionar recursos reais na nuvem
- Testar a execução de uma função Lambda
- Documentar o processo técnico de forma clara e organizada

---

## 🛠️ Recursos Criados

A stack foi criada com sucesso e contém os seguintes recursos:

### 🔹 Bucket S3

- Nome: `meu-bucket-dio-simples`
- Finalidade: armazenamento de arquivos e dados estáticos

### 🔹 Função Lambda

- Nome: `minha-funcao-simples`
- Runtime: Python 3.9
- Código inline que retorna uma mensagem e imprime no log
- Testada com sucesso via console da AWS

### 🔹 Role IAM

- Nome: `minha-role-lambda-simples`
- Permissões: política gerenciada `AWSLambdaBasicExecutionRole`
- Finalidade: permitir que a função Lambda seja executada com segurança

---

## 📄 Template YAML

O arquivo `template.yaml` define toda a infraestrutura da stack. Ele está localizado na raiz do repositório e pode ser reutilizado para futuras implementações.

---

## 🧪 Teste da Função Lambda

Após a criação da stack, a função Lambda foi testada diretamente no console da AWS:

- Um evento de teste foi criado com conteúdo simples
- A função retornou o seguinte resultado:

```json
{
  "statusCode": 200,
  "body": "Olá da Lambda!"
}

