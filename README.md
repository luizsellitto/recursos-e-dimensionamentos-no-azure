# ☁️ Computação e Rede no Azure

## 💻 Serviços de Computação

Azure oferece recursos sob demanda para computação, incluindo processadores, memória, armazenamento, rede e sistemas operacionais, tudo flexível e escalável para suas necessidades.

---

## 🖥️ Máquinas Virtuais (VMs) do Azure

- VMs simulam computadores físicos completos, com processador, memória, armazenamento e rede virtual.
- Modelo **IaaS (Infraestrutura como Serviço)** com total liberdade para escolher sistemas operacionais e configurações.
- Aplica o modelo de **responsabilidade compartilhada**.
- **Conjuntos de dimensionamento de VMs:**
  - Automatizam o balanceamento de carga e escalabilidade.
  - Não funcionam exatamente como um load balancer tradicional.

---

## ⚙️ Conjuntos de Disponibilidade para VMs

- VMs são distribuídas em diferentes **domínios de falha** (racks físicos) para evitar falhas simultâneas.
- Ideal separar VMs em pelo menos **3 domínios de falha** para maior resiliência.
- **Domínios de atualização** indicam a sequência para aplicar atualizações nas VMs.
- Pode aumentar o custo devido à replicação em múltiplos domínios.

---

## 🖥️ Azure Virtual Desktop (Área de Trabalho Virtual)

- Virtualização completa de desktops e aplicativos, hospedada na nuvem.
- Dispensa servidores adicionais de gateway, com implantação multiusuário.
- Permite ambientes customizados e com **alto nível de segurança**.
- Minimiza riscos de ambientes desatualizados e facilita o acesso remoto.

---

## 🐳 Contêineres no Azure

- Ambientes virtuais leves e portáteis, sem necessidade de gerenciar sistemas operacionais.
- Baseados em Docker, que é amplamente suportado no Azure.
- **Azure Container Instances (ACI):**
  - Serviço PaaS que elimina a necessidade de VMs.
  - Suporta balanceamento de carga e escalabilidade automática.
- **Azure Kubernetes Service (AKS):**
  - Orquestração robusta para gestão de múltiplos contêineres.
  - Ideal para arquiteturas distribuídas e microsserviços.

---

## ⚡ Azure Functions

- Computação **serverless** baseada em eventos, oferecida como PaaS.
- Executa código sob demanda, sem infraestrutura ativa em períodos ociosos.
- Personalizável por timers, mensagens e eventos.
- Perfeita para automações e funções acionadas por eventos.

---

## 🔍 Comparativo das Opções de Computação no Azure

| Serviço                | Características                                                                 | Casos de Uso                               |
|------------------------|--------------------------------------------------------------------------------|--------------------------------------------|
| **Máquinas Virtuais**   | Servidores completos na nuvem, com sistema operacional e controle total.       | Migrações lift-and-shift, workloads tradicionais. |
| **Área de Trabalho Virtual** | Desktop Windows acessível via navegador, com múltiplos usuários simultâneos. | Ambientes corporativos para trabalho remoto. |
| **Contêineres**        | Ambiente leve, gerenciado via AKS, ideal para microsserviços e escalabilidade.  | Aplicações distribuídas e altamente escaláveis. |

---

## 🌐 Serviços de Aplicativos no Azure

- Plataforma gerenciada para criação, implantação e escalonamento de apps web e APIs.
- Suporte para integração e implantação contínua.
- Compatível com sistemas Windows e Linux.
- Serviço no modelo PaaS, facilitando o desenvolvimento.

---

## 🌍 Serviços de Rede no Azure

- **Rede Virtual (VNet):** conecta recursos Azure entre si, à internet e redes locais.
- Pontos de extremidade públicos e privados para controle de acesso.
- Comunicação entre VNets exige emparelhamento para garantir isolamento e segurança.
- IPs duplicados em redes conectadas podem causar conflitos.
- **Gateway VPN:** tráfego criptografado entre Azure e redes externas.
- **ExpressRoute:** conexão privada e dedicada entre redes locais e Azure via provedores especializados.

---

## 🛡️ DNS do Azure

- Rede global de servidores DNS com tecnologia **Anycast** para alta performance e confiabilidade.
- Segurança reforçada com controle de acesso baseado em funções (RBAC) e monitoramento contínuo.
- Suporta domínios privados e personalizados em redes virtuais para maior controle interno.

---

✨ *Este resumo foi preparado para facilitar o entendimento e aplicação dos principais componentes de arquitetura da nuvem Azure, consolidando os conceitos fundamentais e boas práticas.*
