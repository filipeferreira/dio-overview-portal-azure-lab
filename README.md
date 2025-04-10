# Lab DIO Bootcamp Bradesco Java Cloud Native  

## Lab Visão geral do portal de serviços da Azure

Este repositório é uma entrega para o Bootcamp Bradesco Java Cloud Native e contém um resumo sobre a visão geral sobre a apresentação do portal de serviços da Azure na prática de laboratório do conteúdo.

Neste laboratório, utilizamos uma conta trial. Seu painel é visualmente idêntico ao das contas ativas, porém alguns recursos podem estar indisponíveis devido a custos elevados ou restrições de região.

O portal permite personalizações de idioma, aparência e outras configurações.

Há uma ampla variedade de serviços disponíveis, organizados em categorias como computação, contêineres, banco de dados, DevOps, machine learning, armazenamento, rede, entre outros.

Em redes, destacou-se o Bastion, que fornece acesso seguro às máquinas atuando como um jump server. Outro ponto relevante foi a criação de firewall na nuvem, já que estar no ambiente cloud não garante segurança automática.

No armazenamento, o principal destaque foi a migração de dados. O portal da Azure oferece serviços especializados para transferir grandes volumes de dados para a cloud.

Além disso, o portal disponibiliza serviços em versão prévia, que não possuem SLA (acordos de nível de serviço) e podem ser descontinuados pela Microsoft, exigindo cautela ao serem utilizados.

A computação em nuvem é uma realidade, e desenvolvedores que desejam atender às demandas do mercado devem se aprofundar no tema.

## Lab Benefícios da Nuvem

O primeiro tópico abordado foi relacionado as SLAs com uma demonstração dos tempos de inatividade permitido para as porcentagens de SLA acima de 99%.

Uma arquitetura de cloud deve levar em consideração a SLA desejada. Quanto maior a SLA, maior o custo do gerenciamento.

Caso o SLA não seja atingido, o cliente receberá créditos para utilização no portal Azure. O dinheiro não é devolvido de outra forma.

Durante a criação de uma máquina virtual, pode-se selecionar uma das opções de disponibilidade. Cada opção de disponibilidade possui um SLA específico. Dentre as opções de disponibilidade, temos a Zona de disponibilidade, Conjuntos de Escala de Máquinas Virtuais e Conjuntos de disponibilidade com SLAs partindo de 99.9%.

Outro ponto referente a replicação estão nas contas de armazenamento. Temos opções de redundância entre datacenters ou entre regiões que também influenciarão o SLA.

## Lab Tipos de Serviços de Nuvem

Tipos de serviço de nuvem

IaaS - Infraestrutura como Serviço

Recursos e serviços que exigem mais intervenção humana e temos mais acesso no contexto de personalização dos recursos e serviços, como por exemplo: configurações, monitoramento, backup, atualizações

PaaS - Plataforma como Serviço

Neste modelo é fornecido um ambiente para criação, teste e implantação de softwares sem se preocupar com a criação e manutenção da infraestrutura

SaaS - Software como Serviço

Aplicativos e apps hospedados disponibilizados para uso na plataforma de nuvem de acordo com a licença contratada que definirá o que os usuários estão visualizando no software.

## Componentes de arquitetura da Azure

### Regiões 
Os custos dos recursos e serviços variam conforme a região e os valores de cada região são diferentes e nem todos os recursos estão disponíveis em todas as regiões.

As regiões são compostas de um ou mais datacenters muito próximos (zonas de disponibilidade), que se comunicam com baixa latência e alta performance.

As regiões preservam a residência dos dados conforme as leis de proteção de dados de cada país.

Existe um tipo de região especial que não está disponível para seleção no portal azure quando for criar seus recursos que são as Regiões Soberanas. Estas são regiões são exclusivas e voltadas para as necessidades de segurança e conformidades das agências federais

### Zonas de disponibilidade
São os datacenters que se comunicam entre si dentro de uma região.

### Pares de regiões 
Cada região possui uma região par que vai atuar como uma zona secundária quando tivermos um problema de indisponibilidade na região. O par de região faz parte do plano de disaster recovery e faz a replicação automática para alguns serviços.

### Recursos
São componentes disponíveis para criação como máquinas virtuais, contas de armazenamento, redes virtuais, bancos de dados, etc.

### Grupos de recursos: 
Os recursos são armazenados em grupos de recursos. São utilizados para organização dos recursos em uma única unidade, como se fosse uma caixa. Os recursos podem existir em apenas um grupo de recursos e os recursos podem existir em diferentes regiões. Os recursos podem ser movidos para diferentes grupos de recursos.

### Assinaturas
Uma boa forma de organização dos centros de custos são via grupos de assinaturas. As assinaturas possuem controle de acesso de autenticação e autorização. Podemos limitar um limite para cobranças e controle de acesso.

### Grupos de gerenciamento
Também relacionado a organização. Agrupa as assinaturas de uma conta.

## Lab Computação e Rede

### Serviços de computação da Azure

Computação é um serviço sob demanda que fornece recursos de computação como discos, processadores, memória, rede e sistemas operacionais.

### Máquinas virtuais do Azure

São emulações de software de computadores físicos e inclui processaror virtual, memória, armazenamento e rede. É um serviço de IaaS que oferece personalização e controle total.

### Conjuntos de dimensionamento de VMs

Balanceamento de carga. Aumente ou diminua o número de VMs automaticamente de acordo com a demanda ou agenda definida fornecendo maior disponibilidade para as aplicações.

### Conjuntos de disponibilidade de VMs

São agrupamentos lógicos de VMs que reduzem as chances de falhas correlacionadas derrubarem as VMs ao mesmo tempo. Os conjuntos de disponibilidade agrupam as VMs em diferentes domínios de falha (racks diferentes).

Os domínios de falha compartilham a mesma fonte de energia e mesma rede, portanto utilizar domínios de falha diminui as chances de falha por hardware físico, interrupções de rede ou energia.

Os conjuntos de disponibilidade aumentam a disponibilidade e resiliência das aplicações

###  Área de trabalho Virtual do Azure

Virtualização de área de trabalho na nuvem, eliminando a necessidade de envio de máquinas físicas para os colaboradores trabalharem.

### Serviços de contêiners

Ambiente virtualizado que não exige o gerenciamento do sistema operacional. Pode ser iniciado e destruído rapidamente. É um serviço PaaS. Exemplo: docker, kubernetes.

### Azure functions

Um serviço PaaS baseado em eventos executado quando chamado, sem exigir uma infraestrutura de servidor durante períodos inativos

### Serviços de Aplicativos

Plataforma pra criação de aplicativos web e APIs. Suporte para linguagens .NET, Node.js, Java, Python e PHP.

### Serviços de rede

Permite que os recursos do Azure se comuniquem entre si, entre diferentes redes virtuais e com a internet.
São isoladas por padrão.

Também é fornecido Gateways de VPN para comunicação entre redes Azure e redes locais da organização

Há uma opção chamada de ExpressRoute que se trata se um cabeamento físico entre as redes Azure e da organização.

Outro serviço é de DNS que dão suporte a um conjunto de alias, facilitando o gerenciamento de nomes.







