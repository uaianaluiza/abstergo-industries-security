# abstergo-industries-security

**Desafio:** Elaborar um relatório para o gerente de TI destacando medidas de segurança integradas a serviços AWS, com o objetivo de aumentar a proteção dos dados e sistemas da empresa.

## Relatório de Implementação de Medidas de Segurança AWS

**Data:** 18/06/2025  
**Empresa:** Abstergo Industries  
**Responsável:** Ana Luiza Santos

---

### Introdução

Este relatório apresenta as principais medidas de segurança implementadas na infraestrutura AWS da Abstergo Industries. O objetivo é fortalecer a proteção dos dados, garantir a conformidade e mitigar riscos de ameaças cibernéticas, utilizando serviços nativos da AWS.

---

### Medidas de Segurança Implementadas

#### 1. Gerenciamento de Identidade e Acesso (IAM) com Princípio do Menor Privilégio

- **Descrição:** O AWS Identity and Access Management (IAM) permite criar e gerenciar usuários, grupos e permissões de acesso aos recursos AWS. A política do menor privilégio garante que cada usuário ou serviço tenha apenas as permissões estritamente necessárias para executar suas funções.
- **Ação Implementada:**
  - Criação de políticas customizadas para cada função.
  - Ativação de autenticação multifator (MFA) para todos os usuários.
  - Revisão periódica de permissões e remoção de acessos desnecessários.
- **Benefício:** Reduz o risco de acessos não autorizados e limita o impacto de credenciais comprometidas.

#### 2. Criptografia de Dados com AWS Key Management Service (KMS) e S3 Encryption

- **Descrição:** O AWS KMS gerencia chaves de criptografia para proteger dados em repouso e em trânsito. O Amazon S3 permite habilitar criptografia automática para todos os objetos armazenados.
- **Ação Implementada:**
  - Ativação da criptografia automática em buckets S3 usando chaves gerenciadas pelo KMS.
  - Utilização de KMS para criptografar volumes EBS e bancos de dados RDS.
  - Rotação periódica das chaves de criptografia.
- **Benefício:** Garante a confidencialidade dos dados, mesmo em caso de acesso físico ou lógico não autorizado.

#### 3. Monitoramento e Detecção de Ameaças com AWS GuardDuty e CloudTrail

- **Descrição:** O AWS GuardDuty é um serviço de detecção de ameaças que monitora continuamente atividades maliciosas e comportamentos anômalos. O AWS CloudTrail registra todas as ações realizadas na conta AWS para auditoria e resposta a incidentes.
- **Ação Implementada:**
  - Ativação do GuardDuty para análise de logs de VPC, CloudTrail e DNS.
  - Configuração de alertas automáticos para eventos suspeitos.
  - Integração do CloudTrail com o Amazon S3 para retenção segura dos logs.
- **Benefício:** Permite resposta rápida a incidentes, auditoria detalhada e identificação proativa de ameaças.

---

### Recomendações Adicionais

- Treinamento contínuo da equipe em práticas de segurança AWS.
- Revisão periódica das políticas de segurança e conformidade.
- Utilização do AWS Well-Architected Framework (pilar de segurança) para avaliação contínua da arquitetura.

---

### Conclusão

A adoção dessas medidas de segurança, integradas aos serviços AWS, fortalece a proteção dos dados e sistemas da Abstergo Industries, reduzindo riscos e garantindo conformidade com as melhores práticas do mercado. Recomenda-se a evolução contínua das políticas de segurança e o acompanhamento das novidades da AWS para manter a empresa sempre protegida.

---

**Ana Luiza Santos**  
Responsável pelo Projeto de Segurança Cloud  
Abstergo Industries
