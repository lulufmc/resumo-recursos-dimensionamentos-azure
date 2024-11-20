# resumo-recursos-dimensionamentos-azure
Resumo sobre o módulo de " Configurando Recursos e Dimensionamentos em Máquinas Virtuais na Azure"

# Serviços de computação e Máquinas Virtuais

A computação do Azure é um serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.

- Máquinas Virtuais

  As Máquinas Virtuais(VMs) são emulações de software de computadores físicos. Inclui processador virtual, memória, armazenamento e rede. Oferta de Infraestrutura como Serviço(IaaS) que oferece personalização e controle total.

- Conjuntos de dimensionamento de VMs

  Os conjuntos de dimensionamento oferecem uma oportunidade de balanceamento de carga para dimensionar os recursos automaticamente. Um conjunto de dimensionamento de VMs é como contratar "funcionários temporários" para um restaurante em horários de pico. Ele ajusta automaticamente o número de máquinas virtuais com base na necessidade, garantindo que seu sistema funcione bem, economizando dinheiro e mantendo seus clientes satisfeitos.

- Conjunto de disponibilidade de VMs

  Um conjunto de disponibilidade funciona como um plano B dentro do data center. Ele garante que, mesmo em caso de falhas ou atualizações, suas VMs permaneçam operacionais, protegendo a continuidade do seu serviço. É ideal para quem precisa de confiabilidade máxima no ambiente de nuvem. Os conjuntos de disponibilidade dividem suas VMs em dois grupos importantes: Domínios de Falha (Fault Domains), As VMs são distribuídas em racks diferentes dentro do data center, e cada rack tem seu próprio sistema de energia e rede. Domínios de Atualização (Update Domains): As VMs são organizadas de forma que atualizações no sistema (como patches de segurança) sejam feitas em grupos diferentes, sem atualizar todas ao mesmo tempo.

- Área de Trabakho virtual do Azure

  É uma virtualização da área de trabalho e aplicativo executada na nuvem. Crie um ambiente completo de virtualização da área de trabalho, sem precisar executar outros servidores de gateway. Reduza o risco de que o recurso seja deixado para trás. Implantações reais de várias sessões.

- Serviços de contêineres do Azure

  Os serviços de contêineres do Azure oferecem um ambiente poderoso e flexível para desenvolver, testar e implantar aplicativos modernos, e que não exige o gerenciamento do sistema operacional. Eles ajudam a economizar recursos, aumentar a eficiência, e garantir que suas aplicações sejam resilientes e escaláveis, podendo responder a alterações sob demanda.
  Instâncias de contêineres do Azure: uma oferta de PaaS, que executa um contêiner ou pod de contêineres no Azure.
  Aplicativos de contêineres do Azure: uma oferta de PaaS, como instâncias de contêineres, que pode balancear a carga e escalar.
  Azure Kubernetes Service (AKS):Serviço gerenciado para orquestrar contêineres usando Kubernetes. Permite gerenciar milhares de contêineres, cuidar da escalabilidade e garantir alta disponibilidade. Exemplo real: Um e-commerce que precisa escalar automaticamente durante a Black Friday.

- Azure Functions

  Uma oferta de PaaS que dá suporte a operações de computação sem servidor. O código baseado em eventos é executado quando chamado, sem exigir uma infraestrutura de servidor durante períodos inativos.

- Serviços de Aplicativo do Azure

  Consistem em uma plataforma totalmente gerenciada para criar, implantar e dimensionar aplicativos Web e API's rapidamente. Oferta de PaaS com requisitos de nível corporativo de desempenho, segurança e conformidade.

- Serviços de rede do Azure

  A Rede Virtual do Azure(VNet) permite que os recursos Azure se comuniquem uns com os outros, com a Internet e com as redes locais. Uma curiosidade, duas redes virtuais não se comunicam por padrão, elas necessitam de um emparelhamento.
  Gateway de VPN: é usado para enviar tráfego criptografado entre uma rede virtual do Azure e uma no local pela internet pública.
  ExpressRoute: estende as redes locais para o Azure por meio de uma conexão privada facilitada por um provedor de conectividade. É como ter um cabo de fibra ótica conectado do datacenter da Microsoft até sua empresa, porém é viável apenas para empresas que estão mais próximas geograficamente da zona de disponibilidade.
  DNS do Azure: O DNS do Azure é um serviço que permite hospedar seus domínios DNS diretamente na plataforma Azure, gerenciando o tráfego e os nomes de domínio para seus aplicativos e serviços na nuvem. funciona como uma agenda telefônica da internet: ele traduz nomes de domínio legíveis (como meusite.com) em endereços IP, que são os identificadores usados pelos computadores para se comunicarem. Vantagens do DNS do Azure: Gerenciamento Centralizado, Alta Disponibilidade, Baixa Latência, Integração com Serviços do Azure e Escalabilidade Global.
  
