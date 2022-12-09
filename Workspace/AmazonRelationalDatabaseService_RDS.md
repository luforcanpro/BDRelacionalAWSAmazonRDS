# Amazon Relational Database Service (RDS)

### Configure, opere e escale um banco de dados relacional na nuvem com apenas alguns cliques.

[Comece a usar o Amazon RDS](https://console.aws.amazon.com/rds/home)

O Amazon Relational Database Service (Amazon RDS) facilita a configuração, a operação e a escalabilidade de bancos de dados relacionais na nuvem. O serviço oferece capacidade econômica e redimensionável e automatiza tarefas demoradas de administração, como provisionamento de hardware, configuração de bancos de dados, aplicação de patches e backups. Dessa forma, você pode se concentrar na performance rápida, alta disponibilidade, segurança e conformidade que os aplicativos precisam.

O Amazon RDS está disponível em vários [tipos de instância de banco de dados](https://aws.amazon.com/pt/rds/instance-types/) – com otimização para memória, performance ou E/S – e oferece seis mecanismos de bancos de dados comuns, incluindo [Amazon Aurora](https://aws.amazon.com/pt/rds/aurora/), [PostgreSQL](https://aws.amazon.com/pt/rds/postgresql/), [MySQL](https://aws.amazon.com/pt/rds/mysql/), [MariaDB](https://aws.amazon.com/pt/rds/mariadb/), [Oracle Database](https://aws.amazon.com/pt/rds/oracle/) e [SQL Server](https://aws.amazon.com/pt/rds/sqlserver/). Você pode usar o [AWS Database Migration Service](https://aws.amazon.com/pt/dms/) para migrar ou replicar facilmente bancos de dados existentes para o Amazon RDS.

Understanding Amazon Relational Database Service (1:53)

# Mecanismos de banco de dados do Amazon RDS

[![Aurora](https://d1.awsstatic.com/Products/product-name/product-icons/Aurora.a4e3560533c66b28b2ffdc350ccd9aaca2bf65c5.png)](https://aws.amazon.com/pt/rds/aurora/)

[![200x100_PostgreSQL_Logo_v2](https://d1.awsstatic.com/logos/rds/200x100_PostgreSQL_Logo_v2.a18ae5300a6efebee36ecfcc1ab7e56d8b00bc07.png)](https://aws.amazon.com/pt/rds/postgresql/)

[![200x100_MySQL_Logo_v2](https://d1.awsstatic.com/logos/rds/200x100_MySQL_Logo_v2.51446b577f0938c90ce5f19fc8fca00e7b44ec3e.png)](https://aws.amazon.com/pt/rds/mysql/)

[![200x100_MariaDB_Logo_v2](https://d1.awsstatic.com/logos/rds/200x100_MariaDB_Logo_v2.f4a0fd7c0db2466f521b58f778fbfe05fe7a8da8.png)](https://aws.amazon.com/pt/rds/mariadb/)

[![200x100_Oracle_Logo_v2](https://d1.awsstatic.com/logos/rds/200x100_Oracle_Logo_v2.7d04f429e97ea6a194501e606c49842294f64e4e.png)](https://aws.amazon.com/pt/rds/oracle/)

[![200x100_Microsoft-SQL-Server_Logo_v2](https://d1.awsstatic.com/logos/rds/200x100_Microsoft-SQL-Server_Logo_v2.80f16c4207b8b79c1b13c8435868213a8b7131cc.png)](https://aws.amazon.com/pt/rds/sqlserver/)

# Benefícios

### Fácil de administrar

O Amazon RDS facilita passar da concepção do projeto para a implantação. Use o [Console de Gerenciamento do Amazon RDS](https://console.aws.amazon.com/rds), a [interface de linha de comando do AWS RDS](https://docs.aws.amazon.com/cli/latest/reference/rds/index.html) ou [chamadas de API](https://docs.aws.amazon.com/AmazonRDS/latest/APIReference/Welcome.html) simples para, em alguns minutos, acessar os recursos de um banco de dados relacional pronto para produção. Sem necessidade de provisionamento de infraestrutura e de instalação e manutenção de software de banco de dados.

[Saiba mais »](https://aws.amazon.com/pt/rds/details/#administration)

### Altamente escalável

Você pode [alterar a escala dos recursos de computação e de armazenamento do banco de dados](https://aws.amazon.com/pt/rds/details/#DB_Instance_Classes) com apenas alguns cliques do mouse ou com uma chamada de API e, muitas vezes, sem necessidade de tempo de inatividade. Vários tipos de mecanismo do Amazon RDS permitem executar uma ou mais [réplicas de leitura](https://aws.amazon.com/pt/rds/features/#Scalability) para redirecionar o tráfego de leitura da instância de banco de dados primária.

[Saiba mais »](https://aws.amazon.com/pt/rds/details/#scalability)

### Disponível e resiliente

O Amazon RDS é executado na mesma infraestrutura altamente confiável usada por outros serviços da Amazon Web Services. Quando você provisiona uma instância de banco de dados [Multi-AZ](https://aws.amazon.com/pt/rds/details/multi-az/), o Amazon RDS replica os dados de forma síncrona para uma instância em espera em uma zona de disponibilidade (AZ) diferente. O Amazon RDS tem diversos outros recursos que aprimoram a confiabilidade de bancos de dados de produção críticos, incluindo backups automatizados, snapshots de banco de dados e substituição automática de hosts.

[Saiba mais »](https://aws.amazon.com/pt/rds/details/#ha)

### Rápido

O Amazon RDS oferece suporte aos aplicativos mais exigentes de banco de dados. Você pode escolher entre duas opções de armazenamento baseado em SSD: uma otimizada para aplicativos OLTP de alta performance e a outra para uso econômico de propósito geral. Além disso, o [Amazon Aurora](https://aws.amazon.com/pt/rds/aurora/) disponibiliza uma performance equivalente à oferecida por bancos de dados comerciais a um décimo do custo.

[Saiba mais »](https://aws.amazon.com/pt/rds/details/#performance)

### Seguro

O Amazon RDS facilita o controle do acesso ao banco de dados pela rede. Além disso, o Amazon RDS permite executar instâncias de banco de dados na [Amazon Virtual Private Cloud](https://aws.amazon.com/pt/vpc/) (Amazon VPC), o que possibilita isolar instâncias de banco de dados e conectá-las à infraestrutura de TI atual por meio de uma VPN IPsec criptografada padrão do mercado. Vários tipos de mecanismo do Amazon RDS oferecem criptografia para dados ociosos e em trânsito.

[Saiba mais »](https://aws.amazon.com/pt/rds/details/#security)

### Baixo custo

Você paga taxas muito baixas e apenas para os recursos que você realmente utilizar. Além disso, você se beneficia da opção de [definição de preço sob demanda](https://aws.amazon.com/pt/rds/pricing/) sem compromissos antecipados ou em longo prazo, ou mesmo de taxas horárias reduzidas por meio da [definição de preço de instância reservada](https://aws.amazon.com/pt/rds/reserved-instances/).

[Saiba mais »](https://aws.amazon.com/pt/rds/details/#cost-effectiveness)

## Clientes do RDS em destaque

[![BuildOn-Logos_600x400_unilever](https://d1.awsstatic.com/BuildOnAssets/BuildOn-CustomerLogos/BuildOn-Logos_600x400_unilever.7ea5ea87b32fb513668913d999b640a837a62929.png)](https://aws.amazon.com/pt/rds/sqlserver/customers/)

[![600x400_Expedia_logo](https://d1.awsstatic.com/logos/600x400_logos/600x400_Expedia_logo.e3439eae7aebb3238178808a483933616102cb62.png)](https://aws.amazon.com/pt/solutions/case-studies/expedia/)

[![600x400_Netflix_Logo](https://d1.awsstatic.com/Industries/Telecom/600x400_Netflix_Logo.1d04083b4bc98a0d8863798681f04c7a0782809c.png)](https://aws.amazon.com/pt/solutions/case-studies/netflix/)

[![600x400_GE_Logo](https://d1.awsstatic.com/logos/600x400_logos/600x400_GE_Logo.e6f67e4439b4e9242e9c925e320846ce867c220a.png)](https://aws.amazon.com/pt/solutions/case-studies/ge-digital-transformation/)

[![Blackboard](https://d1.awsstatic.com/WWPS/images/Blackboard.3e7a9a49774d8a871ff19573a0ff6cbd65415947.png)](https://aws.amazon.com/pt/solutions/case-studies/blackboard/)

[![600x400_Intuit_Logo](https://d1.awsstatic.com/product-marketing/AI/customers/Approved_Logos_600x4001/600x400_Intuit_Logo.e5a700df6f634301f42ec9c8cdd222e6d9bb56fb.png)](https://aws.amazon.com/blogs/database/intuit-story-automate-migration-from-on-premises-mysql-to-amazon-aurora/)

[![VA Seal](https://d1.awsstatic.com/WWPS/images/folder/VA%20Seal.43f1e200ac0e297dec37bbe05d943397996ae087.png)](https://aws.amazon.com/pt/rds/oracle/customers/)

[![recochoku_logo](https://d1.awsstatic.com/logos/customers/jp/recochoku_logo.5a49bf1ac4dc382ae18e2035baa3e50c3acad6f8.png)](https://aws.amazon.com/pt/solutions/case-studies/recochoku-aurora/)

**[Veja todos os estudos de caso do Amazon RDS >>](https://aws.amazon.com/pt/rds/customers/)**

## Parceiros do RDS em destaque

[![app associates](https://d1.awsstatic.com/partner-network/Apps-Associates-Logo_200x100.1d88a3d9e745650cc4ee718acc4a2a8dbdefaee1.png)](https://pages.awscloud.com/GLOBAL-acq-IPC-pcc-migration-appsassociates-july-2019-learn.html)

A Apps Associates, parceira da AWS especializada em Oracle, pode migrar workloads empresariais para a nuvem, liberando os clientes para manter o foco em iniciativas de maior valor. Assista ao nosso webinar para saber como a Apps Associates ajuda os clientes a mudar para o Amazon Aurora.

[Saiba mais »](https://pages.awscloud.com/GLOBAL-acq-IPC-pcc-migration-appsassociates-july-2019-learn.html)

[![rackspace](https://d1.awsstatic.com/partner-network/partner_marketing_web_team/rackspace_200x100-2.433dcb55637c3833ce7040fdf7130d03e84d1f7f.png)](https://pages.awscloud.com/NAMER-adoptf90d-LN-Aurora-Resonate-2019-learn-Rackspace_01-Download-Page.html)

A Rackpace é uma parceira da AWS que pode ajudar você a implementar as práticas recomendadas de desenvolvimento de aplicações modernas com o Amazon Aurora para que você possa acompanhar os requisitos dos clientes e dos negócios. Leia o e-book para saber como a Rackspace ajudou a TotalTrax a automatizar processos e atender à crescente demanda.

[Saiba mais »](https://pages.awscloud.com/NAMER-adoptf90d-LN-Aurora-Resonate-2019-learn-Rackspace_01-Download-Page.html)

## Casos de uso

### Aplicativos web e móveis

Aplicativos web e móveis criados para operar em escalas muito grandes precisam de um banco de dados com alto throughput, escalabilidade de armazenamento massiva e alta disponibilidade. O Amazon RDS atende às necessidades desses aplicativos altamente exigentes com espaço para crescimento futuro. Como o Amazon RDS não tem nenhuma restrição de licenciamento, ele é ideal para o padrão de uso variável desses aplicativos.

[![AirBnB logo pretzel-204x64](https://d1.awsstatic.com/china/hp/change_size/AirBnB%20logo%20pretzel-204x64.1d56c32711170e167b2ae294f927bf83dd6c81f0.png)](https://aws.amazon.com/pt/solutions/case-studies/airbnb/)

> O Airbnb escolheu o Amazon RDS porque ele simplifica a maior parte das tarefas administrativas demoradas geralmente associadas aos bancos de dados. O Airbnb usa a implantação Multi-Availability Zone (Multi-AZ) para automatizar ainda mais a sua replicação de banco de dados e aumentar a resiliência dos dados. O Airbnb conseguiu completar a migração inteira do seu banco de dados para o Amazon RDS com um tempo de inatividade de apenas 15 minutos.

### Aplicativos de comércio eletrônico

O Amazon RDS oferece a empresas de comércio eletrônico de pequeno e grande porte uma solução de banco de dados flexível, segura, altamente escalável e de baixo custo para vendas e varejo online. O Amazon RDS disponibiliza um produto de banco de dados gerenciado que ajuda as empresas de comércio eletrônico a cumprir os requisitos de conformidade da PCI e priorizar a criação de experiências do cliente, sem preocupar-se com o gerenciamento do banco de dados subjacente.

[![Instacart](https://d1.awsstatic.com/product-marketing/AI/customers/Instacart.86952951559a736ac3e819e6a9616d69c1e7a0b7.png)](https://aws.amazon.com/pt/solutions/case-studies/instacart/)

> Para evitar as complexidades de criar um novo banco de dados de produção do zero, a Instacart optou pelo Amazon RDS para seu novo serviço de entrega de compras de supermercado no mesmo dia. Agora, a empresa pode adicionar milhões de itens ao seu banco de dados todo mês. Além disso, sua equipe de engenharia pode focar-se no desenvolvimento de novos recursos e na melhoria da experiência do cliente em geral.

### Jogos móveis e online

Jogos móveis e online precisam de uma plataforma de banco de dados com alto throughput e disponibilidade elevada. O Amazon RDS gerencia a infraestrutura de banco de dados para que desenvolvedores de jogos não precisem se preocupar com provisionar, escalar e o monitorar servidores de banco de dados. O Amazon RDS disponibiliza mecanismos de banco de dados conhecidos no mercado que podem aumentar rapidamente a capacidade para atender às demandas do usuário.

[![bandai](https://d1.awsstatic.com/security-center/bandai.114b4caa516d1edbcc14f23a6e7fd75c067f7ec4.png)](https://aws.amazon.com/pt/solutions/case-studies/bandai-namco-studios/)

> A Bandai Namco Studios usa o Amazon RDS para disponibilizar melhor performance, custos mais baixos, melhor segurança e maior disponibilidade para seus jogos de fliperama, de rede social e móveis. A Bandai Namco viu os benefícios quanto a reduções na sobrecarga, especialmente com relação à inclusão, modificação e remoção de recursos de servidor.

![Standard Product Icons (Features) Squid Ink](https://d1.awsstatic.com/webteam/product-pages/Product-Page_Standard-Icons_01_Product-Features_SqInk.a8d5666758afc5121b4eb818ae18126031c4b61e.png)

Confira os recursos do produto

Explore os principais recursos do Amazon RDS 

[Saiba mais ](https://aws.amazon.com/pt/rds/features/)

![Sign up for a free account](https://d1.awsstatic.com/webteam/product-pages/Product-Page_Standard-Icons_02_Sign-Up_SqInk.f43d5ddc9c43883eec6187f34c68155402b13312.png)

Cadastrar-se para ter uma conta gratuita

Obtenha acesso instantâneo ao nível gratuito da AWS. 

[Cadastre-se ](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html)

![Standard Product Icons (Start Building) Squid Ink](https://d1.awsstatic.com/webteam/product-pages/Product-Page_Standard-Icons_03_Start-Building_SqInk.6a1ef4429a6604cda9b0857084aa13e2ee4eebca.png)

Comece a criar no console

Comece a usar o console de gerenciamento do Amazon RDS.

[Faça login ](https://console.aws.amazon.com/rds)