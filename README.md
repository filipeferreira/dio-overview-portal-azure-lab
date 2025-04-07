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
