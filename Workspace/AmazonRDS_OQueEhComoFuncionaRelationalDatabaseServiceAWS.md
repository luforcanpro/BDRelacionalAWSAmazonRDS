# Amazon RDS: o que é e como funciona o Relational Database Service da AWS

POSTED ON [25 DE MAIO DE 2020](https://flexa.cloud/amazon-rds-o-que-e-e-como-funciona-o-relational-database-service-da-aws/) BY [FERNANDA TESSAROLE](https://flexa.cloud/author/fernanda-tessaroleflexa-cloud/)

[![Amazon RDS: o que é e como funciona o Relational Database Service da AWS](https://flexa.cloud/wp-content/uploads/2020/05/amazon.RDS_.como_.funciona-800x800.png)](https://flexa.cloud/amazon-rds-o-que-e-e-como-funciona-o-relational-database-service-da-aws/)

25
Maio

Amazon Relational Database Service (Amazon RDS) é um serviço de banco de dados SQL gerenciado fornecido pelo Amazon Web Services ( AWS ). O Amazon RDS suporta uma variedade de mecanismos de banco de dados para armazenar e organizar dados e ajuda nas tarefas de gerenciamento de banco de dados, como migração, backup, recuperação e aplicação de patches. 

Neste artigo, além de entender o conceito de RElational Database Service, você vai ver como funciona o Amazon RDS, líder neste mercado.
Confira!

## Para que serve o Amazon RDS

Um administrador de nuvem usa o Amazon RDS para configurar, gerenciar e dimensionar uma instância de banco de dados relacional na nuvem. 

O serviço também faz backup automaticamente das instâncias do banco de dados RDS, captura uma captura instantânea diária de dados e retém os logs de transações para permitir a recuperação point-in-time. Esse recurso permite gerar uma cópia do banco, no estado que ele estava, um segundo antes de uma determinada falha, facilitando de maneira, quase que imediata, a solução do problema..

O RDS também corrige automaticamente o software do mecanismo de banco de dados.

Para aprimorar a disponibilidade e a confiabilidade das cargas de trabalho de produção, o Amazon RDS permite a replicação. 

O administrador também pode ativar o failover automático em várias zonas de disponibilidade com replicação de dados síncrona.

E, normalmente, os usuários da AWS controlam o Amazon RDS por meio do AWS Management Console, APIs do Amazon RDS ou da AWS Command Line Interface.

## Instâncias do banco de dados Amazon RDS

Normalmente, o administrador de banco de dados pode criar, configurar, gerenciar e excluir uma instância do Amazon RDS, que é um ambiente de banco de dados em nuvem, juntamente com os recursos de computação e armazenamento que usa. Dependendo do mecanismo de banco de dados escolhido pelo administrador, ele ou ela pode ativar vários bancos de dados ou esquemas .

O Amazon RDS limita cada cliente a um total de 40 instâncias de banco de dados por conta. A AWS impõe limitações adicionais para instâncias do Oracle e SQL Server — um usuário pode ter apenas até 10 de cada.

## Mecanismos de banco de dados Amazon RDS

Um usuário da AWS pode ativar seis tipos de mecanismos de banco de dados no Amazon RDS:

- RDS para MySQL — compatível com o sistema de gerenciamento de banco de dados relacional de código aberto do MySQL ;
- RDS para PostgreSQL —- compatível com o sistema de gerenciamento de banco de dados objeto-relacional de código aberto do PostgreSQL ;
- RDS para MariaDB — compatível com MariaDB , uma ramificação do MySQL desenvolvida pela comunidade;
- RDS para SQL Server — compatível com o Microsoft SQL Server , um sistema de gerenciamento de banco de dados relacional;
- RDS para Oracle Database — compatível com várias edições do Oracle Database , incluindo várias versões traga sua própria licença e versões incluídas na licença; e
- Amazon Aurora — compatível com MySQL e PostgreSQL, um mecanismo de banco de dados relacional proprietário da AWS.

O Amazon RDS adiciona suporte para versões principais e secundárias dos mecanismos de banco de dados ao longo do tempo, e um administrador pode especificar uma versão do mecanismo quando ele cria uma instância de banco de dados. 

Na maioria dos casos, o Amazon RDS pode oferecer suporte a códigos, aplicativos e ferramentas de desenvolvedor que já estão em uso com bancos de dados existentes.

A AWS fornece outros serviços de banco de dados, como os bancos de dados DynamoDB for NoSQL, Amazon Neptune for graph e o AWS Database Migration Service para facilitar as transferências e transformações do banco de dados.

## Resumo dos recursos e benefícios do Amazon RDS

O RDS foi projetado para reduzir custos operacionais e superar alguns desafios comuns que as empresas enfrentam ao executar bancos de dados por meio de ferramentas como MySQL. Seus principais benefícios incluem:

- **Escalonamento preciso e independente:** uma solução baseada em hardware pode causar ineficiências no gerenciamento do banco de dados, porque os recursos (CPU, memória, armazenamento etc.) são agrupados. O RDS permite que os desenvolvedores alterem facilmente esses fatores independentemente, para que possam ajustá-los às necessidades de seus bancos de dados.
- **Facilidade de implementação:** como o RDS se integra a aplicativos de banco de dados comuns, os desenvolvedores podem continuar trabalhando nos programas com os quais eles já estão familiarizados.
- **Automação de processos:** backups de bancos de dados, aplicação de patches de software, detecção de falhas e recuperação fazem parte do gerenciamento contínuo do banco de dados que pode levar a custos significativos. O Amazon RDS os automatiza para reduzir os encargos administrativos.
- **Segurança:** O Amazon RDS restringe o acesso às instâncias do banco de dados, onde são necessários privilégios avançados, e evita o acesso ao shell. Sua integração com a AWS torna possível gerenciar bancos de dados na Virtual Private Cloud (VPC) e expandir os recursos de segurança com o AWS Identity and Access Management (IAM).
- **Confiabilidade e disponibilidade:** o Amazon RDS inclui replicação que permite alta disponibilidade em bancos de dados de alta prioridade e failover automático se um banco de dados primário ficar indisponível.
- **Custo:** as opções de preço da Amazon para o RDS incluem taxas por demanda e por hora, adaptadas às demandas reais de recursos dos aplicativos de banco de dados
- **Implementação mais rápida:** o RDS supera a necessidade de provisionamento e investimento em recursos de hardware, acelerando o tempo desde a concepção até a implantação.

Que tal, nós conseguimos lhe apresentar o Amazon RDS? [Faça contato conosco](https://flexa.cloud/contact/) para ter uma explicação detalhada de um de nossos especialistas!

### *Relacionado*

[![O que é Amazon Aurora?](https://i1.wp.com/flexa.cloud/wp-content/uploads/2021/02/Amazon_Aurora_Flexa_Cloud.png?resize=350%2C200&ssl=1)](https://flexa.cloud/o-que-e-amazon-aurora/)

#### [O que é Amazon Aurora?](https://flexa.cloud/o-que-e-amazon-aurora/)

18 de janeiro de 2021

Em "AWS"

[![Amazon Aurora: o que é e que benefícios oferece esse mecanismo](https://i1.wp.com/flexa.cloud/wp-content/uploads/2020/05/Amazon.aurora.oq_.e.beneficios.ofere_..png?resize=350%2C200&ssl=1)](https://flexa.cloud/amazon-aurora-o-que-e-e-que-beneficios-oferece-esse-mecanismo/)

#### [Amazon Aurora: o que é e que benefícios oferece esse mecanismo](https://flexa.cloud/amazon-aurora-o-que-e-e-que-beneficios-oferece-esse-mecanismo/)

1 de junho de 2020

Em "AWS"

[![Os serviços de armazenamento da AWS e seus benefícios](https://i1.wp.com/flexa.cloud/wp-content/uploads/2020/04/os.servicos.armazenamento.da_.aws_.e.seus_.beneficios.png?resize=350%2C200&ssl=1)](https://flexa.cloud/os-servicos-de-armazenamento-da-aws-e-seus-beneficios/)

#### [Os serviços de armazenamento da AWS e seus benefícios](https://flexa.cloud/os-servicos-de-armazenamento-da-aws-e-seus-beneficios/)

4 de maio de 2020

Em "AWS"