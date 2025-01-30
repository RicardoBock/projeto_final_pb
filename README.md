# PROJETO FINAL 

## Projeto final do programa de Bolsas Compass UOL/Out-2024
Projeto para realizar a arquitetura de uma migração de servidores locais de uma empresa para os sistemas e serviços AWS, utilizando dos conhecimentos obtidos durante a trilha do projeto de bolsas DEVSECOPS da empresa Compass UOL.


## Objetivos Principais
Realizar o projeto de modernização de um sistema de servidores locais para o ambiente AWS, no qual esta melhoria será realizada em duas etapas:
* Etapa 1 - Realizar a migração dos servidores locais por meio de ferramentas lift-and-shift/as-is para o ambiente AWS;
* Etapa 2 - Modernizar o sistema de servidores utilizando kubernetes e outras tecnologias para o aumento da segurança do sistema.

## Tecnologias utilizadas
Diversas ferramentas que a AWS disponibiliza foram utilizadas nesta atividade, aqui estão elas listadas:

* __TERRAFORM__ - O Terraform é uma ferramenta de infraestrutura como código (IaC) que permite gerenciar e provisionar infraestrutura de software. Ele é usado para gerenciar nuvens públicas e privadas, serviços SaaS, instâncias, storage, redes, DNS e bancos de dados. - Documentação: https://www.ibm.com/br-pt/topics/terraform
* __AWS MGN__ - O MGN (Application Migration Service) é um serviço altamente automatizado de lift-and-shift (as-is), no qual permite a migração de servidores físicos, virtuais ou em nuvem, sem problemas de compatibilidade. - Documentação: https://docs.aws.amazon.com/pt_br/mgn/latest/ug/what-is-application-migration-service.html
* __AWS DMS__ - O DMS (Database Migration Service) é um serviço que auxilia na mobilidade de banco de dados para a nuvem AWS. - Documentação: https://docs.aws.amazon.com/pt_br/prescriptive-guidance/latest/migration-databases-postgresql-ec2/aws-database-migration-service.html
* __AWS S3__ - O Amazon S3 (Simple Storage Service) é um serviço de armazenamento de objetos que oferece escalabilidade, utilizado neste caso para backup dos sistemas. - Documentação: https://docs.aws.amazon.com/pt_br/AmazonS3/latest/userguide/Welcome.html
* __AWS EC2__ - O Amazon EC2 (Elastic Compute Cloud) disponibiliza capacidade computacional segura e redimensionável, utilizado neste projeto para alocar o funcionamento dos servidores back-end e front-end. - Documentação: https://docs.aws.amazon.com/pt_br/AWSEC2/latest/UserGuide/concepts.html
* __AWS RDS__ - O Amazon RDS (Relational Database Service) é um serviço de banco de dados relacional de fácil gerenciamento e otimizado para o custo total da propriedade, utilizado neste caso para armazenar o servidor dedicado ao MySQL. - Documentação: https://docs.aws.amazon.com/pt_br/rds/?nc2=h_ql_doc_rds
* __AWS IAM__ - O Amazon IAM (Identity and Access Management) é um serviço de gerenciamento de acessos da força de trabalho, sendo possível definir barreiras e permissões de diferentes colaboradores do projeto, utilizado como uma das medidas protetivas do projeto - Documentação: https://docs.aws.amazon.com/pt_br/IAM/latest/UserGuide/introduction.html
* __AWS EBS__ - O Amazon EBS (Elastic Block Store) é um serviço que oferece recursos de armazenamento em blocos escaláveis, utilizado para armazenar os documentos e configurações do EC2. - Documentação: https://docs.aws.amazon.com/pt_br/ebs/latest/userguide/what-is-ebs.html
* __AWS EKS__ - O Amazon Elastic Kubernetes Service (Amazon EKS) é um serviço gerenciado do Kubernetes que elimina a necessidade de operar e manter a disponibilidade e a escalabilidade de clusters do Kubernetes na Amazon Web Services (AWS) e em data centers próprios. - Documentação: https://docs.aws.amazon.com/pt_br/eks/latest/userguide/what-is-eks.html
* __AWS Route 53__ - O Amazon Route 53 é um serviço web de Sistema de Nomes de Domínio (DNS) altamente disponível e escalável. - Documentação: https://docs.aws.amazon.com/pt_br/Route53/latest/DeveloperGuide/Welcome.html
* __AWS WAF__ - O Amazon WAF é um firewall de aplicativo web que permite monitorar os pedidos HTTP e HTTPS que são encaminhados para os recursos protegidos do aplicativo web. - Documentação: https://docs.aws.amazon.com/pt_br/waf/latest/developerguide/waf-chapter.html
* __AWS CLOUDFRONT__ - O Amazon CloudFront é um serviço da web que acelera a distribuição do conteúdo estático e dinâmico da web, como arquivos .html, .css, .js e arquivos de imagem, para os usuários. - Documentação: https://docs.aws.amazon.com/pt_br/AmazonCloudFront/latest/DeveloperGuide/Introduction.html
* __APPLICATION LOAD BALANCER__ - O Elastic Load Balancing (ELB) distribui automaticamente o tráfego de aplicações de entrada entre vários destinos e dispositivos virtuais em uma ou mais zonas de disponibilidade (AZs). - Documentação: https://docs.aws.amazon.com/pt_br/elasticloadbalancing/latest/application/application-load-balancer-getting-started.html
* __AWS AUTO SCALING__ - O Amazon EC2 Auto Scaling ajuda você a garantir que você tenha o número correto de EC2 instâncias da Amazon disponíveis para lidar com a carga do seu aplicativo. - Documentação: http://docs.aws.amazon.com/pt_br/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html
* __AWS CloudWatch__ - O AWS CloudWatch monitora os recursos da Amazon Web Services (AWS) e as aplicações executadas na AWS em tempo real. - Documentação: https://docs.aws.amazon.com/pt_br/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html
* __AWS ECR__ - O Amazon Elastic Container Registry é um serviço de registro de imagem de contêiner, seguro, escalável e confiável, gerenciado pela AWS. - Documentação: https://docs.aws.amazon.com/pt_br/AmazonECR/latest/userguide/what-is-ecr.html
* __AWS GuardDuty__ - O GuardDuty Amazon é um serviço de detecção de ameaças que monitora, analisa e processa continuamente fontes de dados AWS e registros em seu ambiente AWS. - Documentação: https://docs.aws.amazon.com/pt_br/guardduty/latest/ug/what-is-guardduty.html
* __AWS SECRETS MANAGER__ -  AWS Secrets Manager ajuda você a criptografar, armazenar e recuperar credenciais com segurança para bancos de dados e outros serviços. - Documentação: https://docs.aws.amazon.com/pt_br/secretsmanager/latest/userguide/intro.html
* __AWS Cost and Usage Reposrt__ - O AWS Cost and Usage Report é utilizada para realizar relatórios de custos. - Documentação: https://docs.aws.amazon.com/pt_br/cur/latest/userguide/what-is-cur.html 
* __AWS Simple Email Service__ - O AWS SES é uma plataforma de e-mail que fornece uma maneira fácil e econômica de enviar e receber e-mails usando seus próprios endereços de e-mail e domínios. - Documentação: https://docs.aws.amazon.com/pt_br/ses/latest/dg/Welcome.html

## ETAPA 1

### Diagrama da infraestrutura e cálculo do custo:
A primeira etapa do projeto consiste em realizar uma migração de 3 servidores locais de uma empresa, utilizando do Application Migration Service (AWS MGN) para os responsáveis pelo Back-end e Front-End é possível realizar a migração destes servidores e por meio do DataBase Migration Service é possível realizar a migração do banco de dados MySQL, o backup dos dados e arquivos é realizado pelo AWS S3

A Arquitetura para a migração destes servidores locais é feita da seguinte forma:
<src img="./imgs/arquitetura_migracao.jpg">

__ÁREA DE PREPARAÇÃO__ 
A área de preparação do AWS Application Migration Service (MGN) é onde o agente de replicação da AWS é instalado nos servidores de origem. Durante a instalação, é possível definir parâmetros de replicação e configurações para gerenciar a preparação da área. 

__ÁREA DE TESTES/TRANSIÇÃO__
A Área de teste e preparação são necessárias para alterar ou reparar erros observados pelo sistema e preparar o sistema para uso.


## ETAPA 2 

A segunda etapa do projeto é realizado a modernização do sistema e a utilização de kubernetes para gerenciamento de containers, no qual os elementos de __Front end__ e __Back end__ vão estar configurados. A utilização do _Kubernetes_ ou K8s possui diversos benefícios como uma maior orquestração dos conteiners, caso necessário alguma modificação, otimização dos recursos, autocorreção, automatização e a segurança da informação. Por meio do _Terraform_ é possível gerenciar infraestruturas e criar algo próximo do diagrama criado:

<src img="./imgs/arquitetura_k8s.jpg">



