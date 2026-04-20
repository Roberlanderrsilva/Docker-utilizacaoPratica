<p align="right">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker Badge">
  <img src="https://img.shields.io/badge/Security-Compliance-green?style=for-the-badge" alt="Security Badge">
</p>

# 🐳 Docker: Infraestrutura Segura e Microsserviços

> **Repositório de Governança de TI:** Este projeto demonstra o provisionamento de um ambiente **LEMP Stack** (Linux, Nginx, MySQL, PHP) utilizando containers, com foco na padronização e segurança de ambientes de microsserviços.

---

## 🎯 Visão Estratégica (GRC)
Em um cenário de **Compliance e Auditoria**, a containerização não é apenas sobre rodar o código, mas sobre garantir a **rastreabilidade** e a **segurança** da infraestrutura. Este projeto foca em:
1. **Imutabilidade:** Garantir que o ambiente de desenvolvimento seja idêntico ao de produção.
2. **Hardening:** Configuração de serviços (Nginx e PHP) com exposição controlada.
3. **Isolamento:** Segregação entre a camada de dados (MySQL) e a camada web.

---

## 📂 Arquitetura e Estrutura de Arquivos

O projeto está organizado para facilitar a manutenção e a conformidade técnica:

```text
/Docker-utilizacaoPratica
├── dockerfile          # Definição da imagem base (Segurança de Camadas)
├── nginx.conf          # Hardening do servidor Web e Proxy Reverso
├── banco.sql           # Provisionamento de Banco de Dados (Schema)
├── index.php           # Aplicação Backend (Ponto de entrada)
├── README.md           # Documentação de Governança
└── assets/             # Evidências de implementação e testes
