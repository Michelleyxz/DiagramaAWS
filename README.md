# DiagramaAWS
Projeto prático do curso AWS da DIO com integração entre EC2, Lambda, S3 e RDS, conforme o diagrama arquitetural.

Serviços Utilizados

Amazon EC2 → Instância para executar scripts e acionar a Lambda

AWS Lambda → Função serverless processando dados enviados pelo EC2

Amazon S3 → Bucket para armazenamento de arquivos

Amazon RDS → Banco de dados relacional para persistência das informações

Fluxo da Arquitetura

O usuário faz upload de um arquivo no EC2.

O EC2 aciona a função Lambda.

A Lambda processa os dados e armazena o resultado no S3.

Informações processadas são gravadas no RDS.

Logs podem ser acompanhados no CloudWatch.

▶ Como Executar

Criar bucket no S3.

Criar função Lambda com permissão para gravar no S3 e no RDS.

Subir script no EC2 para invocar a Lambda.

Criar instância RDS configurada para receber os dados.

Testar o fluxo enviando um arquivo via EC2.

