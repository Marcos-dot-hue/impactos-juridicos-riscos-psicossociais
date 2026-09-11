# Projeto Integrado: Automação n8n (WF5) & Nexus Legal (Riscos Psicossociais)

Repositório oficial unificado contendo o desenvolvimento do projeto prático de automação de infraestrutura no **Bootcamp DIO** e a documentação de pesquisa do projeto acadêmico-jurídico **Nexus Legal**.

---

## 🎯 **Links de Acesso e Submissão**
* **Repositório GitHub:** [Cole aqui o link do seu repositório público]
* **Plataforma DIO:** Link de entrega do Desafio Criativo de Automações com n8n.

---

## 🚀 Parte 1: Automação, Monitoramento de Erros e Gestão de Credenciais (Bootcamp DIO)

Desenvolvido com a plataforma **n8n** para automação de processos de engenharia de confiabilidade, tratamento avançado de exceções e governança de credenciais.

### **Visão Geral e Objetivos do WF5**
O projeto foi estruturado para garantir alta disponibilidade e monitoramento proativo, dividido em dois fluxos principais:
1. **Fluxo Superior (Tratamento de Erros e Alertas):** Captura falhas em tempo de execução, registra logs estruturados em planilhas, envia notificações via Slack e gerencia escalações críticas de dados sensíveis via Gmail.
2. **Fluxo Inferior (Gestão Periódica de Credenciais):** Automação baseada em cronograma (`Schedule Trigger`) para auditoria e rotatividade mensal de tokens e chaves OAuth corporativas.

### 🧩 **Prompt Criativo Utilizado (Desafio DIO)**
```text
Atue como um especialista em N8N.
Crie uma automação para monitoramento de erros de execução e gestão proativa de credenciais de sistemas (WF5).

Público:
Equipe de engenharia e administradores de infraestrutura.

Ferramentas envolvidas:
n8n (Error Trigger, Schedule Trigger, Code Nodes, IF), Google Sheets, Slack e Gmail.

Fluxo:
1. Capturar falhas operacionais ou disparar cronograma mensal de auditoria.
2. Extrair metadados e estruturar checklists de conformidade por meio de scripts JavaScript.
3. Registrar incidentes em planilhas, enviar alertas formatados em canais dedicados e rotear fluxos críticos condicionalmente para e-mails de engenharia.

Regras:
Segmentar incidentes conforme o nível de criticidade (true/false) e validar a integridade e rotatividade de tokens OAuth de forma periódica.

Explique quais nós do N8N devem ser utilizados e a lógica de funcionamento do workflow.

Arquitetura e Componentes dos Workflows
Gatilhos (Error Trigger / Schedule Trigger): Capturam eventos de falhas inesperadas ou iniciam o ciclo mensal de conformidade às 9:00 AM do dia 1 de cada mês.

Processamento (Code Nodes em JavaScript): Extraem metadados de erros e geram inventários contendo 4 credenciais principais (Google Sheets OAuth2, Google Drive OAuth2, Gmail OAuth2 e Slack Bot Token).

Armazenamento e Notificação (Google Sheets / Slack / Gmail):

Planilha Log_Erros_Sistema na aba Log_Incidentes.

Canal do Slack (#alertas-sistema via ID C0C0SJC0APL) com retorno "OK": verdadeiro.

Nó condicional (IF) para disparo de e-mails de urgência quando critico = true.

Dificuldades Superadas e Aprendizados
Mapeamento de Planilhas: Alinhamento de colunas resolvido com mapeamento dinâmico baseado em JSON.

Resolução de Canais no Slack: Substituição de nomes textuais por IDs diretos para contornar restrições de permissão de tokens de bot.

Validação de Caminhos Condicionais: Testes com estados booleanos (true/false) para isolar alertas operacionais de escalações críticas.

Evidências Visuais e Anexos (Automação)
Registro de Logs na Planilha:

Validação de Envio no Slack:

Checklist de Credenciais (Fluxo Inferior):

Cronograma e Esforço
Duração Total: 3 dias úteis de desenvolvimento e homologação.

Esforço Prático: Aproximadamente 12 a 15 horas de implementação técnica no n8n.

⚖️ Parte 2: Projeto Nexus Legal - Impactos Jurídicos na Gestão de Fatores de Riscos Psicossociais
Pesquisa dedicada à análise do enquadramento legal, conformidade trabalhista (Compliance) e gestão estratégica de riscos psicossociais no ambiente corporativo.

Objetivos Principais
Mapeamento Normativo: Analisar as diretrizes legais vigentes aplicáveis à saúde mental e prevenção de riscos ocupacionais.

Compliance Preventivo: Desenvolver diretrizes jurídicas para mitigar passivos trabalhistas associados ao adoecimento mental no trabalho.

Governança Organizacional: Integrar a gestão de fatores psicossociais às políticas de governança corporativa e segurança.

Áreas de Foco
Responsabilidade Civil e Trabalhista: Análise de jurisprudências e impactos de sinistros relacionados à saúde mental.

Normas Regulamentadoras: Alinhamento das práticas de gestão de pessoas às exigências legais de segurança e saúde ocupacional.

Direito Preventivo: Estratégias jurídicas voltadas para a criação de ambientes de trabalho hígidos e seguros.

📂 Estrutura do Repositório Local
Plaintext
/
├── README.md
├── workflows/
│   └── wf5-monitoramento-erros-credenciais.json
├── docs/
│   ├── legislacao-e-normas.md
│   └── analise-de-riscos.md
└── assets/
    ├── image_ce59eb.png
    ├── image_ce4bfa.png
    └── image_d84fea.png
📄 Como Contribuir e Licença
Contribuições: Sugestões de melhorias, artigos ou estudos de caso voltados ao Direito do Trabalho e Automação são bem-vindos via Pull Request.

Licença: Distribuído sob a licença MIT para fins acadêmicos e profissionais.
