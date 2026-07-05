# ☁️ Nebula Cloud Dynamics (NCD) - ServiceNow ITSM Architecture
> **ServiceNow Living Laboratory & CSA Governance Case Study**

![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-success)
![Platform](https://img.shields.io/badge/Platform-ServiceNow%20(Next%20Experience)-blue)
![Role](https://img.shields.io/badge/Role-System%20Administrator%20%7C%20Developer-darkgreen)

<div align="center">
  <img src="https://github.com/leonardorafaelprojects/nebula-cloud-dynamics/blob/main/Logo%20Nebula.png?raw=true" alt="Nebula Cloud Dynamics Logo" width="300"/>
</div>

## 🌐 Sobre o Projeto
A **Nebula Cloud Dynamics (NCD)** é uma empresa provedora de serviços em nuvem (Cenário Fictício/Sandbox). Este repositório documenta a implementação de ponta a ponta do ambiente **ServiceNow (ITSM)** da companhia, desenhado para suportar operações de alta escalabilidade. 

Este projeto atua como um laboratório vivo para a certificação **Certified System Administrator (CSA)**, focando em melhores práticas de arquitetura, segurança de dados (ACLs), automação de processos (Flow Designer/Business Rules) e governança de instâncias (Scoped Apps & Update Sets).

---

## 🏗️ Escopo de Implementação (Arquitetura)

### 1. Gestão de Identidade e Acesso (User/Group Management)
* **Estrutura NCD:** Criação de departamentos isolados (NCD_Cloud_Support, NCD_SecOps, NCD_L1_HelpDesk).
* **Segurança:** Implementação de Roles customizadas e Access Control Lists (ACLs) para garantir o princípio de menor privilégio.

### 2. Gestão de Configuração (CMDB & Tabelas)
* **Arquitetura de Dados:** Extensão de Base Tables (como `task` e `cmdb_ci`) para acomodar servidores virtuais e infraestrutura de nuvem específica da NCD.
* **Governança:** Customização de Form Layouts, List Views e Dictionary Overrides.

### 3. Service Catalog & Portal do Usuário
* Criação de **Catalog Items** e **Record Producers** para requisições comuns da NCD (ex: "Provisionamento de Nova VM" ou "Acesso a Banco de Dados").
* Uso de Variáveis Globais, UI Policies e Client Scripts para dinamizar os formulários.

### 4. Automação e Inteligência de Processos
* **Flow Designer:** Fluxos de aprovação automatizados para requisições de alto custo ou impacto.
* **Server-Side Scripting:** Business Rules operando no backend para validação de dados críticos.

---

## 📦 Log de Implementação (Update Sets)

*Este log reflete as entregas técnicas empacotadas via Update Sets na instância de desenvolvimento (PDI).*

- [x] `NCD_Foundation_v1`: Configuração inicial da instância, branding (cores e logo da NCD) e User/Group management. *(04/07/2026)*
- [ ] `NCD_CMDB_Tables_v1`: Estruturação das tabelas base e relacionamentos.
- [ ] `NCD_Catalog_Flows_v1`: Catálogo de serviços e automações do Flow Designer.
- [ ] `NCD_Security_ACLs_v1`: Endurecimento de segurança e regras de acesso.

---

## 👨‍💻 Autor

**Leonardo Rafael Lima de Oliveira**
*Developer ServiceNow Jr | System Administrator | AI-Augmented Developer*

* [LinkedIn](https://www.linkedin.com/in/leonardorafaelx/)
* [Portfólio & Contato](mailto:leonardorafaeltech@gmail.com)

> *Projeto desenvolvido integrando ferramentas de AI-Augmented Development (LLMs) para mapeamento de requisitos, arquitetura de código e documentação técnica.*
