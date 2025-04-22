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

4. **Defina o Tipo de Máquina**: Escolha o tamanho e as especificações da máquina virtual (como quantidade de CPU, RAM, arquitetura, etc.).
    - Crie um nome de usuário.
    - Escolha o método de autenticação (senha ou chave SSH).
    - Configure a rede virtual, sub-rede e regras de segurança (como portas específicas, por exemplo, RDP ou SSH). 
    - Escolha o tipo de disco (SSD ou HDD) e a capacidade de armazenamento.

5. **Revise e Crie**: Revise todas as configurações. Se tudo estiver correto, clique em "Criar".

6. **Acompanhe a Implantação**: Aguarde a conclusão da implantação no painel de notificações do Azure.
   - Após a criação, localize sua máquina virtual no painel e faça a conexão. 

--------------------------------------------------------------------------
--------------------------------------------------------------------------

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
  - **Escalabilidade**: É a capacidade de ajustar rcursos apra atender à demanda.
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