
# 🚀 Projeto AWS DIO – EC2, Lambda, S3 e RDS  

## 📌 Descrição  
Projeto prático do curso AWS da DIO com integração entre **EC2, Lambda, S3 e RDS**, conforme o diagrama arquitetural.  

## 🛠️ Serviços Utilizados  
- **Amazon EC2** → Instância para executar scripts e acionar a Lambda  
- **AWS Lambda** → Função serverless processando dados enviados pelo EC2  
- **Amazon S3** → Bucket para armazenamento de arquivos  
- **Amazon RDS** → Banco de dados relacional para persistência das informações  

## 📂 Fluxo da Arquitetura  
1. O usuário faz upload de um arquivo no **EC2**.  
2. O **EC2** aciona a **função Lambda**.  
3. A **Lambda** processa os dados e armazena o resultado no **S3**.  
4. Informações processadas são gravadas no **RDS**.  
5. Logs podem ser acompanhados no **CloudWatch**.  

## ▶️ Como Executar  
1. Criar bucket no **S3**.  
2. Criar função **Lambda** com permissão para gravar no **S3** e no **RDS**.  
3. Subir script no **EC2** para invocar a Lambda.  
4. Criar instância **RDS** configurada para receber os dados.  
5. Testar o fluxo enviando um arquivo via EC2.  

## 📊 Diagrama da Arquitetura  
![Diagrama AWS](docs/diagrama.png) 


Testar o fluxo enviando um arquivo via EC2.

