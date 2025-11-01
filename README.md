# AWS-DIO-DESAFIO-05
## tarefas automatizadas lambda e S3

- Lambda é um serviço de computação serverless (sem servidor) que permite executar código sem precisar provisionar ou gerenciar servidores.

- 🏗️ Componentes principais
Componente	Descrição

Função Lambda	O código que você escreve (o “cérebro” da execução)

Trigger/Event Source	Origem do evento que dispara a execução (S3, API Gateway, DynamoDB, etc.)

Execution Role (IAM Role)	Permissões que a função precisa (ex: acessar S3, logs, etc.)

Handler	Ponto de entrada do código (função que o Lambda chama)

Runtime	Linguagem e ambiente de execução (Node.js, Python, Java, etc.)

Environment Variables	Configurações dinâmicas passadas à função

Layers	Pacotes externos (bibliotecas reutilizáveis)

Concurrency	Número de execuções simultâneas da função

- Amazon S3 (Simple Storage Service) é um serviço de armazenamento de objetos oferecido pela AWS, projetado para armazenar e recuperar qualquer quantidade de dados a partir de qualquer lugar na web, de forma segura, durável e escalável.

- ⚙️ Como funciona

Os dados são armazenados em “Buckets”, que funcionam como pastas ou contêineres principais.

Dentro de cada bucket, você armazena “Objetos”, que são os arquivos propriamente ditos (cada objeto tem um nome, dados e metadados).

O S3 é infinitamente escalável — você não precisa se preocupar com capacidade ou manutenção de servidores.


- 💡 Principais características
Recurso	Descrição

Armazenamento de objetos	Armazena dados como arquivos binários (não como blocos ou sistemas de arquivos).

Alta durabilidade	99.999999999% (11 noves) de durabilidade — os dados são replicados automaticamente entre zonas de disponibilidade.

Escalabilidade automática	Nenhuma necessidade de gerenciar espaço de disco ou servidores.

Segurança	Controle de acesso via IAM, ACLs, Policies e Bucket Policies.

Controle de versões	O S3 pode manter várias versões de um mesmo objeto (Versioning).

Criptografia	Criptografia em repouso (SSE-S3, SSE-KMS) e em trânsito (HTTPS).

Classes de armazenamento	Permite escolher o custo e performance conforme o uso (Standard, Infrequent Access, Glacier etc.).

🔐 Segurança e controle de acesso

O acesso ao S3 é controlado de várias formas:

IAM Policies → Controlam quem (usuário/serviço) pode acessar o S3 e o que pode fazer.

Bucket Policies → Regras no nível do bucket.

ACLs (Access Control Lists) → Controle de acesso granular a objetos individuais.

Criptografia (SSE) → Garante proteção dos dados armazenados.

🌍 Integrações comuns

O S3 é amplamente integrado a outros serviços AWS, como:

CloudFront → distribuição de conteúdo global (CDN);

Lambda → processamento de eventos (ex: redimensionar imagens ao fazer upload);

Athena → consultas SQL diretamente sobre dados armazenados no S3;

### Esse projeto mostrou o fluxo dos sistemas integrados para funcionamento de um software, a relação do usuário e suas solicitações e o fornecimento de informações armazenadas no Banco de Dados. 

![image](https://github.com/DrieleMoreira/AWS-DIO-DESAFIO-05/blob/main/Lambda%20e%20S3.drawio)



