# RELATORIO DE MEDIDAS DE SEGURANÇA

**Data:** 10 de março de 2026

**Empresa:** Abstergo Industries

**Responsável:** Almir de Lima Felix dos Santos

---

## Introdução

Este relatório apresenta três medidas de segurança que podem ser implementadas utilizando serviços da **AWS (Amazon Web Services)** para aumentar a proteção de aplicações em nuvem. O estudo foi realizado por **Almir de Lima Felix dos Santos** na empresa **Abstergo Industries**.

O objetivo deste relatório é demonstrar como a utilização de serviços de segurança da AWS pode contribuir para a **proteção de dados sensíveis, prevenção de ataques e controle de acesso**, garantindo maior confiabilidade e integridade para aplicações hospedadas na nuvem.

---

## Descrição das Medidas de Segurança

A implementação das medidas de segurança foi dividida em três etapas, cada uma utilizando um serviço específico da AWS para fortalecer diferentes camadas da infraestrutura da aplicação.

### Etapa 1

- **Nome da ferramenta:** AWS Identity and Access Management (IAM)
- **Foco da ferramenta:** Controle de Acesso e Gerenciamento de Permissões.
- **Descrição de caso de uso:**

A utilização do **IAM** permite controlar quais usuários ou serviços podem acessar recursos da infraestrutura AWS.

Por meio da criação de **roles, políticas e permissões específicas**, é possível garantir que cada usuário tenha acesso apenas aos recursos necessários para executar suas funções, seguindo o princípio do **menor privilégio**.

Exemplo de aplicação prática:

- Desenvolvedores possuem acesso apenas ao ambiente de desenvolvimento.
- Administradores possuem permissões mais amplas para manutenção da infraestrutura.
- Serviços automatizados utilizam **IAM Roles** para acessar bancos de dados ou armazenamento sem necessidade de credenciais expostas no código.

Essa abordagem reduz significativamente riscos de **acesso indevido e vazamento de credenciais**.

---

### Etapa 2

- **Nome da ferramenta:** AWS Web Application Firewall (WAF)
- **Foco da ferramenta:** Proteção contra ataques a aplicações web.
- **Descrição de caso de uso:**

O **AWS WAF** é utilizado para proteger aplicações web contra ataques comuns da internet, como:

- **SQL Injection**
- **Cross-Site Scripting (XSS)**
- Ataques de **bots maliciosos**
- Tentativas de exploração automatizadas

O WAF pode ser integrado a serviços como **Application Load Balancer**, **Amazon CloudFront** e **API Gateway**, permitindo a criação de **regras personalizadas** que bloqueiam tráfego suspeito antes que ele alcance a aplicação.

Com essa camada de proteção, a aplicação passa a ter um **filtro de segurança na borda da rede**, reduzindo riscos de exploração de vulnerabilidades.

---

### Etapa 3

- **Nome da ferramenta:** AWS Shield
- **Foco da ferramenta:** Proteção contra ataques DDoS.
- **Descrição de caso de uso:**

O **AWS Shield** fornece proteção contra ataques de **Distributed Denial of Service (DDoS)**, que têm como objetivo sobrecarregar servidores e tornar aplicações indisponíveis.

O serviço funciona automaticamente para detectar e mitigar ataques que tentem:

- Saturar a rede da aplicação
- Consumir recursos computacionais
- Derrubar serviços expostos à internet

O **AWS Shield Standard**, disponível sem custo adicional para serviços AWS, protege recursos como:

- **Amazon CloudFront**
- **Elastic Load Balancing**
- **Amazon Route 53**

Essa proteção garante maior **disponibilidade da aplicação**, mesmo durante tentativas de ataques massivos.

---

## Conclusão

A implementação de medidas de segurança utilizando serviços da AWS permite fortalecer significativamente a proteção de aplicações em nuvem.

Neste relatório foram apresentados três mecanismos importantes:

- **Controle de acesso com IAM**
- **Proteção contra ataques web com AWS WAF**
- **Mitigação de ataques DDoS com AWS Shield**

A adoção dessas soluções contribui para garantir **confidencialidade, integridade e disponibilidade dos sistemas**, além de reduzir riscos de ataques e acessos não autorizados.

Recomenda-se que a empresa **Abstergo Industries** continue investindo em práticas de segurança em nuvem e considere a adoção de outras ferramentas complementares, como **AWS GuardDuty**, **AWS Security Hub** e **AWS CloudTrail**, para ampliar o monitoramento e auditoria da infraestrutura.

---

## Anexos

1. Guia de Boas Práticas de Segurança na AWS.
2. Diagrama de Arquitetura Segura da Aplicação.
3. Documentação de Políticas de Acesso (IAM).

---

**Assinatura do Responsável pelo Projeto:**

---

Almir de Lima Felix dos Santos