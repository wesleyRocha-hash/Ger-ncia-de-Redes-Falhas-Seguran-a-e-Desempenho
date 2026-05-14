# 🌐 Gerência de Redes: Falhas, Segurança e Desempenho

Este repositório contém anotações, resumos e exercícios focados nos fundamentos de Gerenciamento de Redes de Computadores. O conteúdo explora os padrões de gerência, métricas de hardware, mecanismos de segurança cibernética e indicadores de Qualidade de Serviço (QoS).

## 📚 Tópicos Abordados

O conteúdo está dividido nas principais áreas do modelo de gerenciamento proposto pela ISO (Desempenho, Falhas, Configuração, Contabilização e Segurança - *FCAPS*).

### 🛠️ 1. Gerência de Falhas e Segurança
Foco em como lidar com problemas de comunicação, prever quebras de hardware e proteger a infraestrutura contra intrusões.

*   **Erros de Transmissão:**
    *   Causados por interferência, distorção ou atenuação física.
    *   Podem ser de *único bit* (degradação rápida) ou em *rajada* (múltiplos bits, degradação prolongada).
    *   *Correção:* FEC (uso de bits redundantes) ou retransmissão de pacotes.
*   **Métricas de Hardware:**
    *   **MTBF (Tempo Médio Entre Falhas):** Previsão estatística do tempo de operação contínua antes de uma nova quebra.
    *   **MTTR (Tempo Médio para Reparos):** Tempo médio necessário para restaurar a operação após uma falha.
*   **Mecanismos de Segurança:**
    *   **Criptografia:** Ocultação de dados utilizando chaves de 64, 128 ou 256 bits (chaves maiores são recomendadas para ambientes governamentais ou críticos).
    *   **Logs e NTP:** Registros de atividades da rede. Dependem estritamente do protocolo NTP para sincronização global de relógios, garantindo auditorias confiáveis.
    *   **NAC (Controle de Acesso):** Barreira contra dispositivos não autorizados, vulneráveis ou infectados.

### 🚥 2. Gerência de Desempenho e Configuração
Aborda os parâmetros para garantir a entrega de dados e o isolamento lógico das sub-redes.

*   **Indicadores de Qualidade e Desempenho (QoS):**
    *   **Vazão (Throughput):** Quantidade efetiva de dados processados em bps.
    *   **Latência (Atraso):** Tempo total entre o envio do pacote e a confirmação de recebimento.
    *   **Jitter:** Variação irregular no tempo e na ordem de entrega dos pacotes.
    *   **Perda de Pacotes:** Descarte de dados quando os *buffers* dos roteadores atingem o limite de armazenamento.
*   **Isolamento Lógico (VLANs e VTP):**
    *   Uso de VLANs para dividir e isolar redes físicas em várias sub-redes virtuais por segurança e organização.
    *   Uso do protocolo **VTP** (VLAN Trunk Protocol) para automatizar e propagar configurações de um switch servidor para os clientes.

### 🔌 3. Modelos e Protocolos de Gerenciamento
*   **SNMP:** Protocolo popular e simples, operando com gerentes, agentes e MIBs.
*   **CMIP:** Baseado no modelo OSI, consome mais recursos do sistema, mas possui alta segurança.
*   **TMN:** Modelo estruturado focado em redes de telecomunicações.
*   **Sniffing:** Ferramenta/técnica para interceptar pacotes e validar parâmetros de rede.

---

## 📝 Lista de Exercícios de Fixação

O repositório também inclui uma lista de exercícios de múltipla escolha e questões discursivas para validar os conhecimentos sobre o modelo OSI, FCAPS, métricas (MTTR/MTBF), ferramentas de QoS e criptografia. *(Consulte os arquivos do repositório para ver os exercícios completos e o gabarito).*

---

**Autor:** Wesley Fernandes
*Desenvolvido durante os estudos de Análise e Desenvolvimento de Sistemas (ADS).*
