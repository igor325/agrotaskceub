Projeto AgroTask
Curso: Ciência de Dados (UniCEUB) Disciplina: Projeto Integrador Ildo Semestre: 2º Semestre de 2025

1. Visão Geral
O AgroTask é um sistema de gestão de atividades (SGA) focado no agronegócio. O projeto atua como um intermediário inteligente entre o software de gestão JetBov e a API do WhatsApp (Meta).

O objetivo é automatizar a comunicação de tarefas (alimentação, vacinação, manejo) do gestor para os funcionários de campo, permitindo o envio de alertas e o recebimento de confirmações de execução, tudo centralizado em um painel de controle.

2. Objetivo Atual
Com base no levantamento de requisitos (RFs e RNFs) e na modelagem inicial do banco de dados (ERD e SQL), o objetivo atual do projeto é construir o núcleo funcional da aplicação (MVP - Minimum Viable Product).

Isso inclui:

Backend: Implementar a arquitetura RESTful (RNF07) e o CRUD (Criar, Ler, Atualizar, Deletar) para as entidades principais: User (Funcionários) e Activity (Tarefas).

Autenticação: Criar o sistema de login seguro (RNF02 - JWT) para os AdminAccount (Gestores).

Integrações (Spike/Prova de Conceito): Estabelecer as conexões iniciais com as APIs do JetBov e do WhatsApp (Meta) para validar a comunicação.

Frontend (Wireframes): Desenvolver os protótipos de tela (wireframes) do painel de gestão, conforme definido nos "Próximos Passos" (RNF01, RNF08).

3. Papéis da Equipe (Sugestão)
Para organizar o desenvolvimento, sugerem-se os seguintes papéis:

Product Owner (PO) & Tech Lead: Carlos Mateo Wall

Scrum Master & Backend Developer: Joao Victor Moura

Backend Developer (Foco: Integração JetBov & Regras de Negócio): Lucas Leandro

Frontend Developer & UX/UI (Foco: Wireframes e Painel): Jamille G.

DBA & Backend Developer (Foco: Integração WhatsApp & Notificações): Igor de Souza

4. Backlog da Sprint 1 (Sprint de Fundação)
O objetivo desta Sprint é construir a fundação técnica e as primeiras funcionalidades essenciais do painel de administração.

4.1. Débitos Técnicos (Infraestrutura)
[ ] T01: Configurar o repositório Git do projeto.

[ ] T02: Configurar o ambiente de desenvolvimento backend (ex: Node.js/Express, Python/Django, etc.) seguindo o padrão RESTful (RNF07).

[ ] T03: Configurar e inicializar o banco de dados PostgreSQL (RNF06).

[ ] T04: Aplicar o schema inicial do banco de dados (Tabelas: User, AdminAccount, Activity, ActivityUsers, MessageTemplate).

4.2. Histórias de Usuário (Features)
[ ] US01 (Gestor): Como Gestor, eu quero poder me autenticar (login) no painel de administração para acessar o sistema com segurança (RF01, RNF02).

[ ] US02 (Gestor): Como Gestor, eu quero poder cadastrar, visualizar, editar e deletar (CRUD) um Funcionário (Usuário) (RF01, RF08).

[ ] US03 (Gestor): Como Gestor, eu quero poder cadastrar, visualizar, editar e deletar (CRUD) uma Atividade agropecuária (RF03, RF08).

[ ] US04 (Gestor): Como Gestor, eu quero poder atribuir uma Atividade a um ou mais Funcionários (RF08).

4.3. Pesquisa (Spikes)
[ ] SPK01 (Dev): Como Desenvolvedor, eu quero pesquisar e estabelecer a conexão inicial com a API do JetBov para listar rebanhos (Prova de Conceito) (RF02).

[ ] SPK02 (Dev): Como Desenvolvedor, eu quero pesquisar e configurar a API do Meta (WhatsApp) para enviar uma mensagem de teste "Olá, Mundo" (Prova de Conceito) (RF04, RNF04).

4.4. UX/UI
[ ] UX01 (Gestor): Como Gestor, eu quero um wireframe (protótipo) de baixa fidelidade da tela de login e do dashboard principal (painel de gestão) (RNF01, RNF08).
