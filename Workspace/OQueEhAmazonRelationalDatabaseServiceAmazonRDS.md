# O que é o Amazon Relational Database Service (Amazon RDS)?

[PDF - ](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/rds-ug.pdf#Welcome) -[RSS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/rdsupdates.rss)



O Amazon Relational Database Service (Amazon RDS) é um serviço Web que facilita a configuração, operação e dimensionamento de um banco de dados relacional na Nuvem AWS. Ele fornece capacidade econômica e redimensionável para um banco de dados relacional padrão do setor e gerencia tarefas comuns de administração de banco de dados.

**nota**

Este guia abrange mecanismos de banco de dados do Amazon RDS diferentes do Amazon Aurora. Para obter informações sobre o Amazon Aurora, consulte o [*Guia do usuário do Amazon Aurora*](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html).

Este guia aborda o uso do Amazon RDS na Nuvem AWS. Para obter informações sobre o uso do Amazon RDS em ambientes do VMware on-premises, consulte o [*Guia do usuário do Amazon RDS on VMware*](https://docs.aws.amazon.com/AmazonRDS/latest/RDSonVMwareUserGuide/rds-on-vmware.html).

## Visão geral do Amazon RDS

Por que usar um serviço de banco de dados relacional gerenciado? Porque o Amazon RDS assume muitas das tarefas de gerenciamento difíceis ou entediantes de um banco de dados relacional:

- Quando você comprar um servidor, recebe CPU, memória, armazenamento e IOPS, todos no mesmo pacote. Com o Amazon RDS, estes elementos se separaram, para que você possa escalá-los independentemente. Se você precisar de mais CPU, menos IOPS ou mais capacidade de armazenamento, poderá alocá-los facilmente.
- O Amazon RDS gerencia backups, patches de software, detecção automática de falhas e recuperação.
- Para oferecer uma experiência de serviço gerenciada, o Amazon RDS não fornece acesso ao shell para as instâncias de banco de dados. Ele também restringe o acesso a determinados procedimentos e tabelas do sistema que exigem privilégios avançados.
- Você pode ter backups automatizados realizados conforme necessário ou pode criar manualmente seu próprio snapshot de backup. Você pode usar esses backups para restaurar um banco de dados. O processo de restauração do Amazon RDS funciona de maneira confiável e eficiente.
- Você pode usar os produtos de banco de dados já conhecidos com: MySQL, MariaDB, PostgreSQL, Oracle, Microsoft SQL Server.
- Você pode obter alta disponibilidade com uma instância primária e uma instância secundária síncrona que pode ser usada para failover em caso de problemas. Também é possível usar réplicas de leitura MariaDB, Microsoft SQL Server, MySQL, Oracle, e PostgreSQL para aumentar a escalabilidade de leitura.
- Além da segurança no seu pacote de banco de dados, você pode ajudar a controlar quem pode acessar seus bancos de dados do RDS usando o AWS Identity and Access Management (IAM) para definir usuários e permissões. Você também pode ajudar a proteger seus bancos de dados colocando-os em uma nuvem privada virtual (VPC).

Caso esteja começando a usar os produtos e serviços AWS, passe a saber mais com os seguintes recursos:

- Para obter uma visão geral de todos os produtos AWS, consulte [O que é computação em nuvem?](http://aws.amazon.com/what-is-aws/)
- A Amazon Web Services fornece vários serviços de banco de dados. Para obter orientação sobre qual é o melhor serviço para o seu ambiente, consulte [Executar bancos de dados no AWS](http://aws.amazon.com/running_databases/).

## Instâncias de banco de dados

O bloco de construção básico do Amazon RDS é a instância do banco de dados. Uma *instância de banco de dados* é um ambiente isolado de banco de dados na Nuvem AWS. A instância de banco de dados pode conter vários bancos de dados criados pelo usuário. É possível acessar a instância de banco de dados usando as mesmas ferramentas e os mesmos aplicativos usados com uma instância de banco de dados independente. Crie e modifique uma instância de banco de dados usando a AWS Command Line Interface, a API do Amazon RDS ou o AWS Management Console.

Cada instância de banco de dados executa um *mecanismo de banco de dados*. Atualmente, o Amazon RDS oferece suporte aos mecanismos de banco de dados MySQL, MariaDB, PostgreSQL, Oracle e Microsoft SQL Server. Cada mecanismo de banco de dados tem seus próprios recursos com suporte, e cada versão de um mecanismo de banco de dados pode incluir recursos específicos. Além disso, cada mecanismo de banco de dados tem um conjunto de parâmetros em um parameter group de banco de dados que controlam o comportamento dos bancos de dados que ele gerencia.

A capacidade de computação e memória de uma instância de banco de dados é determinada de acordo com sua *classe de instância de banco de dados*. Você pode selecionar a instância de banco de dados que melhor atende às suas necessidades. Se as suas necessidades mudarem com o passar do tempo, você poderá alterar as instâncias de bancos de dados. Para obter mais informações, consulte [Classes de instância de banco de dados ](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/Concepts.DBInstanceClass.html).

**nota**

Para obter informações sobre a definição de preço de classes de instâncias de banco de dados, consulte a seção Definição de preço da página de produto do [Amazon RDS](http://aws.amazon.com/rds/).

Existem três tipos de armazenamento de instâncias de bancos de dados: Magnético, Uso geral (SSD) e IOPS provisionadas (PIOPS). Eles diferem em características de desempenho e preço, permitindo que você adapte o custo e o desempenho de armazenamento às necessidades do seu banco de dados. Cada instância de banco de dados tem requisitos mínimos e máximos de armazenamento, de acordo com o tipo de armazenamento e o mecanismo de banco de dados compatíveis. É importante ter armazenamento suficiente para que os bancos de dados tenham espaço para se expandir. Além disso, armazenamento suficiente garante que os recursos do mecanismo de banco de dados tenha espaço para escrever conteúdo ou entradas de log. Para obter mais informações, consulte [Armazenamento de instâncias de banco de dados do Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/CHAP_Storage.html).

É possível executar uma instância de banco de dados em uma nuvem privada virtual (VPC) usando o serviço Amazon Virtual Private Cloud (Amazon VPC). Ao usar uma VPC, você tem controle sobre o ambiente de rede virtual. É possível escolher seu próprio intervalo de endereços IP, criar sub-redes e configurar o roteamento e listas de controle de acesso. A funcionalidade básica do Amazon RDS é a mesma, não importa se ela está sendo executada ou não em uma VPC. O Amazon RDS gerencia backups, patches de software, detecção automática de falhas e recuperação. Não há custos adicionais para executar a instância de banco de dados em uma VPC. Para obter mais informações sobre como usar a Amazon VPC com o RDS, consulte [VPCs da Amazon Virtual Private Cloud e do Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/USER_VPC.html).

O Amazon RDS usa o Network Time Protocol (NTP) para sincronizar o tempo em instâncias de banco de dados.

## AWSRegiões e zonas de disponibilidade da

Os recursos de computação em nuvem da Amazon estão alojados em instalações de datacenter altamente disponíveis em diferentes áreas do mundo (por exemplo, América do Norte, Europa ou Ásia). Cada localização de datacenter é chamada de uma região da AWS.

Cada região da AWS contém vários locais distintos, chamados de zonas de disponibilidade, ou AZs. Cada zona de disponibilidade é projetada para ser isolada de falhas em outras zonas de disponibilidade. Cada uma é projetada para fornecer conectividade de rede de baixa latência e custo reduzido para outras zonas de disponibilidade na mesma região da AWS. Ao iniciar as instâncias em Zonas de disponibilidade separadas, você pode proteger seus aplicativos de falha de um único local. Para obter mais informações, consulte [Regiões, zonas de disponibilidade e Local Zones ](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html).

Você pode executar sua instância de banco de dados em várias zonas de disponibilidade, uma opção chamada de implantação Multi-AZ. Quando você escolhe essa opção, a Amazon automaticamente provisiona e mantém uma instância de banco de dados secundária em espera em uma zona de disponibilidade diferente. A instância de banco de dados primária é sincronicamente replicada ao longo das zonas de disponibilidade para a instância secundária. Essa abordagem ajuda a fornecer redundância de dados e suporte a failover, eliminar congelamentos de E/S e minimizar picos de latência durante backups do sistema. Para obter mais informações, consulte [Alta disponibilidade (Multi-AZ) para Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/Concepts.MultiAZ.html).

## Security

Um *grupo de segurança* controla o acesso a uma instância de banco de dados. Ele faz isso permitindo acesso aos intervalos de endereços IP ou instâncias do Amazon EC2 que você especificar.

Para obter mais informações sobre security groups, consulte [Segurança em Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/UsingWithRDS.html).

## Monitorar uma instância de banco de dados do Amazon RDS

Existem várias maneiras de controlar o desempenho e a integridade de uma instância de banco de dados. Você pode usar o serviço gratuito do Amazon CloudWatch para monitorar a performance e a integridade de uma instância. Os gráficos de performance do CloudWatch são exibidos no console do Amazon RDS. Também é possível assinar eventos do Amazon RDS para receber notificações sobre alterações em uma instância de banco de dados, em um snapshot de banco de dados, em um grupo de parâmetros de banco de dados ou em um grupo de segurança de banco de dados. Para obter mais informações, consulte [Monitorar uma instância de banco de dados do Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/CHAP_Monitoring.html).

## Como trabalhar com o Amazon RDS

Existem várias maneiras de interagir com o Amazon RDS.

### AWS Management Console

O AWS Management Console é uma interface de usuário simples e baseada na Web. Você pode gerenciar suas instâncias de banco de dados a partir do console sem necessidade de programação. Para acessar o console do Amazon RDS, faça login no AWS Management Console e abra o console do Amazon RDS em https://console.aws.amazon.com/rds/.

### Interface da linha de comando

Você pode usar a AWS Command Line Interface (AWS CLI) para acessar interativamente a API do Amazon RDS. Para instalar a AWS CLI, consulte [Instalação da AWSinterface da linha de comando](https://docs.aws.amazon.com/cli/latest/userguide/installing.html). Para começar a usar a AWS CLI para o RDS, consulte [a referência da AWS Command Line Interface para o Amazon RDS](https://docs.aws.amazon.com/cli/latest/reference/rds/index.html).

### Como p rogramar com o Amazon RDS

Se você for desenvolvedor, poderá acessar o Amazon RDS de forma programática. Para obter mais informações, consulte [Referência da interface de programação de aplicações (API) do Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/ProgrammingGuide.html).

Para desenvolvimento de aplicativos, recomendamos usar um dos Kits de desenvolvimento de software (SDKs) da AWS. Os SDKs AWS contêm detalhes de nível baixo, como autenticação, lógica de nova tentativa e gerenciamento de erros, para que você possa se concentrar na lógica da aplicação. AWS Os SDKs estão disponíveis para uma ampla variedade de linguagens. Para obter mais informações, consulte [Ferramentas para a Amazon Web Services ](http://aws.amazon.com/tools/).

AWSA também fornece bibliotecas, código de exemplo, tutoriais e outros recursos para ajudar você a começar de maneira mais fácil. Para obter mais informações, consulte [Código de exemplo e bibliotecas](http://aws.amazon.com/code).

## Como você é cobrado pelo Amazon RDS

Quando você usa o Amazon RDS, você pode optar por usar instâncias de banco de dados sob demanda ou instâncias de banco de dados reservadas. Para obter mais informações, consulte [Faturamento da instância de banco de dados para Amazon RDS ](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/User_DBInstanceBilling.html).

Para obter informações sobre a definição de preço do Amazon RDS, consulte a [página de produto do Amazon RDS](http://aws.amazon.com/rds/pricing).

## Próximas etapas

Na seção anterior, você conheceu os componentes de infraestrutura básicos que o RDS oferece. O que você deve fazer em seguida?

### Conceitos básicos

Criar uma instância de banco de dados usando as instruções em [Conceitos básicos do Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/CHAP_GettingStarted.html).

### Tópicos específicos do mecanismo de banco de dados

Você pode rever informações específicas para um determinado mecanismo de banco de dados nas seções a seguir:

- [MariaDB no Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/CHAP_MariaDB.html)
- [Microsoft SQL Server no Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/CHAP_SQLServer.html)
- [MySQL no Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/CHAP_MySQL.html)
- [Oracle no Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/CHAP_Oracle.html)
- [PostgreSQL no Amazon RDS](https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/UserGuide/CHAP_PostgreSQL.html)