# resumo-lab-dio
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO

Configurações do portal:
    - Alterar o idioma
    - Alterar a aparência e o menu de inicialização

Demonstração dos serviços por Categoria
- Computação:
  - Área de trabalho do Azure
  - Chave SSH
  - Conta de laboratório e vários outros.

- Rede
    - Bastions
    - Endereço IP
    - Gateways
    - Links
    - Firewall
    - Peering, etc
- Armazenamento
  - Servidores
  - Discos
  - Migração, etc

- **Versão Prévia**: O provider não garante que o recurso continuará.


# RESUMO PARA CRIAR UMA MÁQUINA VIRTUAL
1. **Acesse o Portal do Azure**: Fazer login na Portal do Azure com sua conta.

2. **Navegue até "Máquinas Virtuais"**: Localize e clique em "Máquinas Virtuais" e depois em "Adicionar" ou "Criar".
   - Definir a subscrição e o Grupo.
   - Definir detalhes como nome da máquina, região e opções de Zona.
   - **Selecione uma Imagem**: Escolha o sistema operacional que você deseja usar (por exemplo, Windows, Ubuntu ou outro).

3. **Defina o Tipo de Máquina**: Escolha o tamanho e as especificações da máquina virtual (como quantidade de CPU, RAM, arquitetura, etc.).
    - Crie um nome de usuário.
    - Escolha o método de autenticação (senha ou chave SSH).
    - Configure a rede virtual, sub-rede e regras de segurança (como portas específicas, por exemplo, RDP ou SSH). 
    - Escolha o tipo de disco (SSD ou HDD) e a capacidade de armazenamento.

4. **Revise e Crie**: Revise todas as configurações. Se tudo estiver correto, clique em "Criar".

5. **Acompanhe a Implantação**: Aguarde a conclusão da implantação no painel de notificações do Azure.
   - Após a criação, localize sua máquina virtual no painel e faça a conexão. 

# CRIAÇÃO DE INSTÂNCIA DE BANCO DE DADOS NO AZURE

1. **Criando uma Instância Gerenciada do Azure SQL**
   - Acesse o Portal do Azure e vá até Azure SQL. 
   - Escolha Instância Gerenciada e clique em Criar.
   - Defina as configurações básicas, como assinatura, grupo de recursos, nome da instância e região.
   - Escolha o tamanho da instância, considerando vCore e armazenamento necessário.
   - Configure a rede virtual para garantir conectividade segura.

2. **Configuração de Segurança e Acesso**
   - Habilite autenticação do Azure AD para maior segurança.
   - Defina regras de firewall para permitir conexões seguras.
   - Configure grupos de segurança de rede para restringir acessos indesejados.

3. **Gerenciamento e Monitoramento**
   - Utilize Azure Monitor para acompanhar o desempenho da instância.
   - Configure alertas para monitorar métricas críticas.
   - Use Azure Automation para tarefas de manutenção automatizadas.

4. **Backup e Recuperação**
   - Configure backup automático para garantir a recuperação de dados.

# CONSTRUINDO ARQUITETURA NO AZURE
1.  **Criando um Grupo de Recursos**
    - Acesse o Portal do Azure e localize Grupo de Recursos
    - Escolha a assinatura
    - Defina um nome para o Grupo de Recursos
    - Escolha a região
    - Inclua marcações (opcional)
    - Revise e Crie e finalize clicando em Criar.
2. **Criando Vnet**
  - Acesse o Portal do Azure e localize Grupo de Recursos
  - Escolha a assinatura e o Grupo de Recursos
  - Defina um nome para a Vnet 
  - Defina a região
  - Clique em Analisar e Criar e depois Criar

# CONHECENDO O ESTÚDIO DE FALA
- Acesse o site https://speech.microsoft.com/portal
  - Caso não tenha recurso criado, será necessário criar:
    - Clicar em Configurações (Engrenagem) -> Criar Novo Recurso
      - Definir o nome, selecionar a assinatura, região, tipo de preço e o Grupo de Recursos
  - Selecionar o recurso e clicar em Usar o Recurso -> Clicar no "X" para fechar
  - Clicar em Conversão de fala em Texto em Tempo Real
  - Selecionar o Idioma do texto e localizar o arquivo de áudio



# CONHECENDO O LANGUAGE STUDIO
1. **Criando um recurso de idioma**
    - Acesse o Portal do Azure, clique em Create a Resource
      - Selecione AI + Machine Learning
        - Language Service -> Create
        - Selecionar o Grupo de Recursos, região, definir um nome e Pricing Tier
        - Clicar em Review + Crete -> Create
2. **Acessar o Language Cognitive do Azure**
   - Site: https://language.cognitive.azure.com/
   - Selecionar a subscrição, tipo de resource (Language) e o nome -> Done
   - **Analisando sentimentos**
     - Selecionar Classify text -> Analyze sentiment and mine opinions
     - Selecionar o linguagem do texto e o nome do Recurso
     - Digitar ou colar o texto a ser analisado
     - Marcar o checkbox e executar (RUN)

# CONHECENDO O AI SEARCH
1. **Criando o Azure AI Search**
    - Acesse o Portal do Azure, em Azure Services, clique em AI Search -> Create
      - Selecionar o Grupo de Recursos, região, definir um nome e Pricing Tier
      - Clicar em Review + Create -> Create
2. **Criando um recurso de IA**
    - Clicar em Create a Resource
      - Selecione AI + Machine Learning
      - Azure AI Services -> Create
      - Selecionar o Grupo de Recursos, região, definir um nome e Pricing Tier
      - Clicar em Review + Create -> Create
3. **Criando a conta de Armazenamento**
    - Clicar em Storage accounts -> Create
      - Selecionar o Resource group, definir um nome, definir a região, performance e redundância
      - Review + Create -> Create
      - Será necessário permitir o acesso de Blob anonymous
        - Em configuration -> Marcar Enable Allow Blob anonymous access -> Save
      - Em Data Storage -> Containers -> + Container
        - Definir o Nome do container e marcar a opção Container (anonymous read access...) -> Create
        - Após criar o Storage account, acessar o container e fazer o upload dos arquivos (*.docx)
4. **Testando a busca**
    - Ir no mecanismos de busca AI Search, clicar no que foi criado
      - Import data - Selecionar onde dados congnitivos estão armazenados
    - Clicar em Search explorer - > e fazer a devida pesquisa. Exs: search=*&$count=true ou search=locations:'Chicago'


--------------------------------------------------------------------------
--------------------------------------------------------------------------
# - MÓDULO 1 - 
# COMPUTAÇÃO EM NUVEM

## Domínio de Objetivo
- **O que é computação em nuvem?**
  - É o fornecimento de serviços de computação pela internet, habilitando inovações mais rápidas, recursos flexíveis e economias de escala e pagando apenas pelo que é usado.

- **Nuvem Privada:**
    - Infraestrutura dedicada exclusivamente a uma única organização, podendo ser hospedada localmente ou em um datacenter de terceiros.
    - As organizações são responsáveis por operar os serviços que fornecem.
    - Não fornece acesso aos usuários fora da organização.
- **Nuvem Pública:**
    - Infraestrutura de computação fornecida por terceiros (como AWS, Azure, Google Cloud), acessível pela internet.
    - Fornece recursos e serviços a várias organizações e usuários.
    - Acessada via conexão de rede segura.

- **Nuvem Híbrida:**
  - Combinação de nuvem pública e privada, permitindo que dados e aplicações sejam compartilhados entre elas.

## Comparação de modelos de nuvem
- **Nuvem Privada:**
    - As organizações têm controle total sobre os recursos e a segurança.
    - As organizções são responsáveis pela manutenção e pelas atualizações de hardware e software.
- **Nuvem Pública:**
    - Nenhuma despesa de capital para escalar verticalmente.
    - Os aplicativos podem ser provisionados e desprovisionados rapidamente.
    - As organizações pagam apenas pelo que utilizam.

- **Nuvem Híbrida:**
    - As organizações determinam onde executar seus aplicativos.
    - As organizações controlam a segurança, a conformidade e os requisitos legais.
    - Fornece a maior flexibilidade.


## Comparação entre Capex e Opex
- **CAPEX:**
    - **O que é**: Investimento inicial em bens físicos e infraestrutura.
    - **Na prática**: Comprar servidores, licenças de software, datacenter próprio.
    - **Características**:
        - Alto custo inicial.
        - Depreciação ao longo do tempo.
        - Exemplo: Montar um datacenter próprio para rodar seus sistemas.
- **OPE**X:
  - **O que é**: Custos contínuos para operar e manter os serviços.
  - **Na prática**: Pagar mensalmente pelos serviços de nuvem (ex: AWS, Azure).
  - **Características**:
    - Pagamento conforme o uso ("pay-as-you-go").
    - Flexível e escalável.
    - Reduz gastos com manutenção de hardware.
    - Exemplo: Usar máquinas virtuais na AWS e pagar apenas pelo tempo utilizado.

## Benefícios da Nuvem
  - **Alta Disponibilidade**: Recursos disponível sempre que necessário. Associado ao SLA.
    - Se concentra em garantir a disponibilidade máxima, independente de interrupções ou eventos que possam ocorrer.
  - **Escalabilidade**: É a capacidade de ajustar recursos para atender à demanda.
    - É possível adicionar mais recursos para lidar melhor com o aumento da demanda.
  - **Elasticidade**: É a possibilidade de aumentar (automaticamente ou manualmente) os recursos, conforme a necessidade.
    - Ex: É possível adicionar máquinas virtuais eou contêineres por meio da expansão.
  - **Confiabilidade**: Devido ao design descentralizado, a nuvem naturalmente dá suporte a uma infraestrutura confiável e resiliente.
    - Dessa forma é possível ter recursos implantados em várias regiões do mundo.
  - **Previsibilidade**: Com a cloud, permite que se avance com confiança, seja no desempenho ou no custo.
  - **Segurança**: Há várias ferramentas que atendem às necessidades dos clientes, importante lembrar que a implementação de muitas delas devem ser realizadas pelo cliente.
  - **Governança**: Ao estabelecer uma presença de governança o mais cedo possível, você poderá manter sua presença de nuvem atualizada, protegida e bem gerenciada
    - A auditoria baseada em nuvem ajuda a sinalizar qualquer recurso que esteja fora de conformidade com seus padrões corporativos e fornece estratégias de mitigação.
  - **Gerenciabilidade**: São as opções de capacidade de gerenciamento. Há dois tipos que trazem excelentes benefícios.
    - O gerenciamento na nuvem diz respeito à maneira de gerenciar o ambiente: Por meio do Portal Web, linha de comando, usando APIs, usando PowerShell.

## Tipos de Serviços de Nuvem na Azure
- **IaaS**: Infraestrutura como Serviço - Ambiente para gerenciamento da infraestrutura sujacente.
  - Servidores, Firewalls/Segurança de rede e Planta física/Edifício do datacenter.
- **Paas**: Plataforma como Serviço - fornece um ambiente para criação, o teste e a implantação de aplicativos de softwares, sem focar no gerenciamento da infraestrutura subjacente.
  - Envolve a Iaas e Sistemas Operacionais e Ferramentas para desenvolvedores, análise de negócios de gerenciamento de database.
  - 
- **Saas**: Software como serviço - Os usuários se conectam e sam aplicativos com base em nuvem pela Interneto. Exemplos: Microsoft Office 365, email e calendários.
  - Envolve a Iaas e Paas e aplicativo/apps hospedados.
  - Modelo de preço de pagamento conforme o uso.
  - Os usuários pagam pelo software que utilizam em um modelo de assinatura.

# - MÓDULO 2 - 
# COMPONENTES DE ARQUITETURA DO AZURE
- ## Regiões: 
  - São compostas de um ou mais datacenters muito próximos
  - Fornecem flexibilidade e escala para reduzir a latência do cliente
  - Preservam a residência dos dados com uma oferta de abrangente de conformidade
- ## Zona de disponibilidade:
  - Fornece proteção contra tempo de inatividade devido a falha do datacenter
  - Separa fisicamente os datacenters dentro da mesma região
  - Cada datacenter é equipado com alimentação, resfriamento e rede independentes
  - Conectadas por meio de redes privadas de fibra ótica
- ## Pares de região
  - No mínimo 300 milhas de separação entre pares de região
  - Replicação automática para alguns serviços
  - Recuperação de região priorizada em caso de interrupção
- ## Regiões soberanas do Azure
  - Serviços Governamentais dos EUA:
    - Atende às necessidades de segurança e conformidade das agência federais, governos e locais dos EUA e seus provedores de soluções
  - Azure Governamental:
    - Fisicamente separada do Azure
    - Fisicamente isolada de implantações que não sejam governos dos EUA
    - Acessível somente a pessoal verificado e autorizado
  - Azure China
    - A Microsoft é o primeiro provedor estrangeiro de serviços de nuvem pública da China, em conformidade com as regulamentações governamentais
    - Instância separada fisicamente dos serviços de nuvem do Azure e operados pela 21Vianet
    - Todos os dados permanecem dentro da China para garantir a conformidade
- ## Recursos do Azure
  - São componentes como armazenamento, máquinas virtuais e redes que estão disponíveis para criar soluções de nuvem
- ## Grupo de Recursos
  - É um contêiner para gerenciar e agregar recursos em uma única unidade.
  - Os recursos podem existem em apenas um grupo de recursos
  - Os recursos podem existir em diferente regiões
  - Podem ser movidos para outros grupos de recursos
  - Os aplicativos podem utilizar vários grupos de recursos
- ## Assinaturas do Azure
  - Fornece a você acesso autenticado e autorizado às contas do Azure
  - Gerar relatórios de cobrança e faturas separados para cada assinatura
  - Gerenciar e controlar o acesso aos recursos que os usuários podem provisionar com assinatura específicas
- ## Grupos de Gerenciamento
  - Podem incluir várias assinaturas
  - As assinaturas herdam as condições aplicadas ao grupo de gerenciamento
- ## Serviços de computação do Azure
  - A computação do Azure é um serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.
    - **Máquinas Virtuais do Azure**: São emulações de computadores físicos, inclui processador, memória, armazenamento e rede
    - **Conjunto de dimensionamento de VMs**: Oferecem uma oportunidade de balanceamento de carga dimensionar os recursos automaticamente.
    - **Conjunto de disponibilidade de VM**: 
    - **Área de trabalho do Azure**: Criação de um ambiente completo de virtualização da área de trabalho sem precisar executar outros servidores de gateway.
    - **Serviços de contêineres do Azure**: Fornecem um ambiente leve e virtualizado que não exige o gerenciamento do sistema operacional e pode responder a alterações sob demanda.
    - **Aplicativos de contêiner do Azure**: uma oferta de PaaS, como instancia de contêineres, que pode balancear a carga e escala.
    - **Serviço de Kubernetes do Azure**: serviço de orquestração para contêineres com arquiteturas distribuidas e grandes volumes de contêineres.
    - **Azure Functions**: Oferta de PaaS que dá suporte a operações de computação sem servidor - O código baseado em eventos é executado quando chamado.
    - **Serviços de Aplicativos do Azure**: Consistem em uma plataforma (PaaS) totalmente gerenciada para criar, implantar e dimensionar aplicativos Web e APIs rapidamente.
    - **Serviços de rede do Azure**: permite que os recursos do Azure se comuniquem uns com os outros, com a Internet e com as redes locais.
- ## IDENTIDADE, ACESSO E SEGURANÇA
  - **Microsoft Entra ID**: serviço de gerenciamento de identidades e acesso baseado em nuvem do Microsfoft Azure.
    - Garante a Autenticação
    - Logon único (SSO)
    - Gerenciamento de aplicativos
    - Negócios para Negócios (B2B)
    - Gerenciamento de dispositivos
  - **Autenticação**:
    - Identifica a pessoa ou serviço buscando acesso a um recurso
    - Solicita credenciais de acesso legítimo
    - Base para criar princípios de identidade e controle de acesso seguros
  - **Autorização**: 
    - Determina o nível de acesso de uma pessoa ou serviço autenticado
    - Define quais dados eles podem acessar e o que podem fazer com eles
  - **Acesso Condicional**: Ferramenta usada para permitir/negar o acesso a recursos baseados em sinais e de identidade
    - Associação de usuário ou grupo
    - Local do IP
    - Dispositivo
    - Aplicativo
    - Detecção de risco
  - **Controle de acesso baseado em função**:
    - Gerenciamento de acesso de granularidade fina
    - Divida as tarefas dentro da equipe e conceda somente a quantidade de acesso de que os usuários precisam para trabalhar
    - Habilite o acesso ao portal do Azure e o controle de acesso ao recursos
  - **Microsoft Defender para Nuvem**: serviço de monitoramento que fornece proteção contra ameaças nos datacenters do Azure e locais
  - 