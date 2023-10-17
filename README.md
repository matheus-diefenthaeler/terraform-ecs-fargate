# Terraform AWS ECS Fargate Configuration

## Overview

Este conjunto de arquivos Terraform `main.tf` tem como objetivo facilitar a implantação de uma aplicação utilizando o AWS Elastic Container Service (ECS) com a opção Fargate. O processo inclui a criação de um repositório no Elastic Container Registry (ECR), configuração de uma Virtual Private Cloud (VPC), provisionamento de um Application Load Balancer (ALB) e definição de tarefas para o ECS.

## Recursos Criados

- **Elastic Container Registry (ECR):** Um repositório para armazenar imagens Docker.

- **Virtual Private Cloud (VPC):** Rede isolada para hospedar a aplicação com sub-redes públicas e privadas.

- **Application Load Balancer (ALB):** Gerencia o tráfego da aplicação entre as instâncias Fargate.

- **ECS Cluster:** Ambiente para executar as tarefas Fargate.

## Requisitos

Antes de executar este script, certifique-se de ter os seguintes pré-requisitos:

- **Credenciais AWS:** Configure as credenciais da AWS com as permissões necessárias. Isso pode ser feito definindo variáveis de ambiente ou usando perfis AWS CLI.

- **Terraform Instalado:** Instale o Terraform em sua máquina. Você pode baixá-lo em [terraform.io](https://www.terraform.io/downloads.html).

## Execução

Siga estas etapas para implantar a instância RDS usando o Terraform:

1. **Inicializar o Terraform:**
    ```bash
    terraform init
    ```

2. **Revisar o Plano:**
    ```bash
    terraform plan
    ```

3. **Aplicar Alterações:**
    ```bash
    terraform apply
    ```

4. **Destruir Recursos (Opcional):**
    ```bash
    terraform destroy
    ```