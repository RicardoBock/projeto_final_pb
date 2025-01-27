# PROJETO FINAL 
## Projeto final do programa de Bolsas Compass UOL/Out-2024

## Objetivos
Realizar uma modernização de um sistema de servidores locais para o ambiente AWS, no qual esta melhoria será realizada em duas etapas, etapa 1 constituí realizar a migração dos servidores locais para o ambiente AWS e a etapa 2 constitui em modernizar o sistema de servidores utilizando kubernets e outras tecnologias

## Tecnologias utilizadas
Diversas ferramentas que a AWS disponibiliza foram utilizadas nesta atividade, aqui estão elas listadas:

* AWS MGN - O MGN (Application Migration Service) é um serviço altamente automatizado de lift-and-shift (as-is), no qual permite a migração de servidores físicos, virtuais ou em nuvem, sem problemas de compatibilidade. - Documentação: https://docs.aws.amazon.com/pt_br/mgn/latest/ug/what-is-application-migration-service.html
* AWS DMS - O DMS (Database Migration Service) é um serviço que auxilia na mobilidade de banco de dados para a nuvem AWS. - Documentação: https://docs.aws.amazon.com/pt_br/prescriptive-guidance/latest/migration-databases-postgresql-ec2/aws-database-migration-service.html
* AWS S3 - O Amazon S3 (Simple Storage Service) é um serviço de armazenamento de objetos que oferece escalabilidade, utilizado neste caso para backup dos sistemas. - Documentação: https://docs.aws.amazon.com/pt_br/AmazonS3/latest/userguide/Welcome.html
* AWS EC2 - O Amazon EC2 (Elastic Compute Cloud) disponibiliza capacidade computacional segura e redimensionável, utilizado neste projeto para alocar o funcionamento dos servidores back-end e front-end. - Documentação: https://docs.aws.amazon.com/pt_br/AWSEC2/latest/UserGuide/concepts.html
* AWS RDS - O Amazon RDS (Relational Database Service) é um serviço de banco de dados relacional de fácil gerenciamento e otimizado para o custo total da propriedade, utilizado neste caso para armazenar o servidor dedicado ao MySQL. - Documentação: https://docs.aws.amazon.com/pt_br/rds/?nc2=h_ql_doc_rds
* AWS IAM - O Amazon IAM (Identity and Access Management) é um serviço de gerenciamento de acessos da força de trabalho, sendo possível definir barreiras e permissões de diferentes colaboradores do projeto. - Documentação: 
