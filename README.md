# Relatório de Segurança em Aplicações AWS

Este repositório contém uma atividade prática desenvolvida durante a formação **AWS Cloud Practitioner Certification**.

O objetivo do projeto é apresentar **três medidas fundamentais de segurança em aplicações hospedadas na AWS**, demonstrando como serviços da plataforma podem ser utilizados para proteger infraestrutura, aplicações e dados.

---

## Objetivo

Demonstrar, de forma conceitual e aplicada, como utilizar serviços da AWS para aumentar a segurança de aplicações em nuvem.

O relatório aborda três pilares importantes de segurança:

* Controle de acesso
* Proteção contra ataques em aplicações web
* Proteção contra ataques de negação de serviço (DDoS)

---

## Serviços AWS Abordados

### AWS IAM (Identity and Access Management)

Responsável pelo **controle de acesso** aos recursos da AWS.

Permite:

* Criar usuários e grupos
* Definir políticas de permissão
* Aplicar o princípio do **menor privilégio**
* Utilizar **roles** para serviços acessarem recursos de forma segura

---

### AWS WAF (Web Application Firewall)

Ferramenta de proteção para **aplicações web** contra ataques comuns da internet.

Protege contra:

* SQL Injection
* Cross-Site Scripting (XSS)
* Bots maliciosos
* Tráfego suspeito

Pode ser integrado com:

* CloudFront
* Application Load Balancer
* API Gateway

---

### AWS Shield

Serviço de proteção contra **ataques DDoS (Distributed Denial of Service)**.

Principais características:

* Mitigação automática de ataques
* Proteção para serviços expostos à internet
* Integração com CloudFront, Route 53 e Elastic Load Balancing

---

## Estrutura do Projeto

```
/relatorio
 ├── relatorio.md
 ├── anexos
 │   ├── boas-praticas-aws.pdf
 │   ├── arquitetura-segura.pdf
 │   └── politicas-iam.pdf
```

---

## Anexos

O projeto inclui documentos complementares:

1. **Guia de Boas Práticas de Segurança na AWS**
2. **Arquitetura Segura de Aplicação**
3. **Documentação de Políticas de Acesso (IAM)**

---

## Autor

**Almir de Lima Felix dos Santos**

Desenvolvedor e participante da formação **AWS Cloud Practitioner Certification**.

---

## Licença

Este projeto foi desenvolvido apenas para **fins educacionais** como parte da formação AWS.
