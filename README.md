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

##
