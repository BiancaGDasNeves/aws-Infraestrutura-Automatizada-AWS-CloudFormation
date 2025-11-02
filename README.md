🚀 Desafio DIO: Automatizando Infraestrutura com AWS CloudFormation
📘 Descrição do Projeto

Este repositório foi criado como parte do desafio da Digital Innovation One (DIO), com o objetivo de aplicar os conceitos de Infraestrutura como Código (IaC) utilizando o AWS CloudFormation.

A proposta é construir e documentar uma infraestrutura automatizada na AWS, explorando boas práticas de versionamento e documentação técnica com o GitHub.

🧩 Objetivos de Aprendizagem

Ao finalizar este desafio, fui capaz de:

Aplicar na prática os conceitos de IaC;

Utilizar o AWS CloudFormation para provisionar recursos automaticamente;

Documentar processos técnicos de forma clara e organizada;

Utilizar o GitHub como ferramenta de versionamento e compartilhamento técnico.

🏗️ Estrutura da Infraestrutura Criada

O template CloudFormation (template.yml) provisiona os seguintes recursos:

✅ VPC configurada com sub-rede pública

✅ Security Group com regras específicas de acesso

✅ Instância EC2 com Amazon Linux 2

✅ (Opcional) Bucket S3 para armazenamento

✅ (Opcional) Outputs informando o IP público da instância ou URLs geradas

💡 Ajuste esta lista conforme o que você implementou no seu template.

⚙️ Tecnologias Utilizadas

AWS CloudFormation

AWS CLI

YAML

Git e GitHub

Markdown (para documentação)

🪜 Passo a Passo da Implementação

1. Criação do Template

Desenvolvi o arquivo template.yml contendo toda a definição da infraestrutura.

Exemplo de comando para validar o template:

aws cloudformation validate-template --template-body file://template.yml


Deploy da Stack

Após validação, realizei o deploy:

aws cloudformation deploy \
    --template-file template.yml \
    --stack-name dio-cloudformation-lab \
    --capabilities CAPABILITY_IAM


Verificação

Acessei o AWS Management Console para confirmar a criação da stack e dos recursos.

Testes

Conectei-me à instância EC2 (caso criada) via SSH para validar o funcionamento:

ssh -i "minha-chave.pem" ec2-user@<IP-PUBLICO>


Documentação

Capturei prints e salvei na pasta /images.


🧠 Insights e Aprendizados

Durante o desenvolvimento deste desafio, aprendi:

A importância do CloudFormation para padronizar e automatizar a criação de recursos em nuvem;

Como validar e implantar templates de forma segura com o AWS CLI;

O valor de documentar todo o processo técnico para aprendizado e portfólio;

Boas práticas de uso do GitHub para versionar e compartilhar conhecimento.

📚 Referências

Documentação Oficial AWS CloudFormation

Guia Markdown no GitHub

Formação GitHub Certification - GitBook

Repositório DIO no GitHub

💼 Autor

Bianca Gonçalves das Neves
📧 [biancagneves@gmail.com]
