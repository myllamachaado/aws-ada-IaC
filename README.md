# Ada + Nuclea | Projeto final do modulo IaC 


### Projeto proposto

## **Implantação de WordPress com Amazon ECS usando AWS CloudFormation**

Criar uma pilha do AWS CloudFormation para implantar um ambiente do WordPress usando o Amazon ECS (Elastic Container Service). O ambiente incluirá um cluster ECS, uma definição de tarefa, um serviço, um balanceador de carga, dimensionamento automático e um sistema de arquivos EFS para armazenar dados persistentes do WordPress.

**Descreva a Infraestrutura: No template do CloudFormation, defina os seguintes recursos:**

- Um cluster ECS para hospedar os containers do WordPress.
- Uma definição de tarefa que especifica como os containers do WordPress serão configurados.
- Um serviço ECS para garantir que a tarefa do WordPress seja sempre executada.
- Um balanceador de carga para distribuir o tráfego entre os containers.
- Configurações de dimensionamento automático para ajustar automaticamente o número de containers com base na carga.
- Um sistema de arquivos EFS para armazenar dados persistentes do WordPress.

**Use Parâmetros:**

- No template, utilize parâmetros para permitir a personalização durante a criação da pilha, como nome do cluster, tamanho da instância, etc.

- Implante a pilha através do CLI ou do Management Console, a escolha é livre.


### Arquitetura Proposta

<figure>
<p align="center">
  <img src="https://github.com/myllamachaado/aws-ada-IaC/blob/master/diagrama.png"/><br>
</p>
</figure>



### Pré Requisitos:
Para que esse projeto seja executado da forma correta é preciso que você tenha uma VPC com duas subnets e um security group já configurados na conta em questão. Os itens serão usados como entrada na tela do CloudFormation.


### Executando o projeto:

1) Faça o clone do repositório 
2) Insira o arquivo `ecs-wordpress-stack.yml` no CloudFormation.
3) Insira os parâmetros necessários para a execução do scrips (VPC, Subnet1 e Subnet2 e Security Groups, etc).


