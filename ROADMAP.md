\# Roadmap – DevPilot-IDP



Este roadmap descreve as principais etapas de evolução do DevPilot-IDP, desde o MVP atual até funcionalidades mais avançadas de plataforma.



---



\## Fase 0 – MVP (estado atual)



\- \[x] Estrutura de projeto organizada em módulos:

&nbsp; - backend/

&nbsp; - frontend/

&nbsp; - devpilot-check/

&nbsp; - automation/

&nbsp; - infra/

\- \[x] API básica para:

&nbsp; - Criar solicitações de serviço

&nbsp; - Listar solicitações

&nbsp; - Listar tarefas de provisionamento

&nbsp; - Listar instâncias de serviços

\- \[x] Script de compliance simplificado (`devpilot-check/scanner.py`)

\- \[x] Portal Angular inicial para listar solicitações

\- \[x] README com visão geral e propósito do projeto



---



\## Fase 1 – Jornada do desenvolvedor e experiência



\*\*Objetivo:\*\* Tornar o DevPilot-IDP mais próximo da experiência real de uma plataforma interna moderna.



\- \[ ] Criar formulário completo no frontend para abertura de solicitações de serviço:

&nbsp; - Nome do serviço

&nbsp; - Time responsável

&nbsp; - Runtime

&nbsp; - Ambiente

&nbsp; - Flags (observabilidade, mensageria, etc.)

\- \[ ] Exibir timeline da solicitação com evolução de status

\- \[ ] Melhorar tela de listagem de instâncias:

&nbsp; - Campos de CPU, memória, replicas e status

\- \[ ] Documentar jornada do desenvolvedor em `docs/developer-journey.md`



---



\## Fase 2 – Automação e compliance



\*\*Objetivo:\*\* Aumentar a sensação de automação e governança leve.



\- \[ ] Integrar o `devpilot-check` com o backend:

&nbsp; - Endpoint para avaliar compliance de um serviço

\- \[ ] Permitir salvar resultados de compliance em banco de dados

\- \[ ] Criar endpoint agregado de "visão de plataforma":

&nbsp; - Quantidade de serviços

&nbsp; - Quantidade por ambiente

&nbsp; - Distribuição de status (RUNNING, DEGRADED, DOWN)

\- \[ ] Expor métricas de plataforma via Actuator



---



\## Fase 3 – Observabilidade e operação



\*\*Objetivo:\*\* Simular uma operação básica de plataforma em produção.



\- \[ ] Criar endpoint de "logs" simplificados para cada tarefa de provisionamento

\- \[ ] Criar tela no frontend para visualizar logs e status de tarefas

\- \[ ] Documentar padrões de logging e observabilidade

\- \[ ] Simular incidentes:

&nbsp; - Tarefas com status FAILED

&nbsp; - Sugestões de ações no frontend com base no erro



---



\## Fase 4 – Golden Paths e templates



\*\*Objetivo:\*\* Aproximar o projeto de um IDP real com criação de projetos base.



\- \[ ] Documentar estrutura de templates de serviço (ex.: Java Spring API)

\- \[ ] Criar estrutura de CLI simples (script) para gerar um serviço base:

&nbsp; - Pastas

&nbsp; - Configurações padrão

&nbsp; - Dependências mínimas

\- \[ ] Conectar o conceito de template ao formulário do frontend



---



\## Fase 5 – Experimentos e extensões futuras



\*\*Objetivo:\*\* Abrir espaço para evolução contínua.



\- \[ ] Simular atributos de mensageria (Kafka/SQS) nos metadados dos serviços

\- \[ ] Simular integração com ferramentas de code quality (SonarQube) via metadados

\- \[ ] Adicionar diagrama de arquitetura visual em `docs/architecture.md`

\- \[ ] Incluir testes automatizados de unidade no backend

\- \[ ] Incluir testes básicos de frontend (Angular)



---



Este roadmap pode ser ajustado a qualquer momento, conforme novas ideias de evolução para a plataforma surgirem.



