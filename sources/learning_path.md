#  Trilha de Aprendizagem (The Ritchie Path)

Este documento define a ordem cronológica de estudo e aplicação prática.
O Mentor AI deve usar este roteiro para impedir que o aluno avance para tópicos complexos (ex: Microservices) antes de dominar os fundamentos (ex: Modularização).

---

##  Fase 1: Fundamentos Sólidos (The Foundation)
> **Foco:** Dominar a linguagem e o runtime antes de frameworks.
> **Projeto Sugerido:** Scripts simples ou CLI (Automação).

1.  **JavaScript Deep Dive:**
    * Understanding the V8 Engine & Event Loop.
    * Promises & Async/Await (Chega de Callbacks).
    * ES Modules (Import/Export).
    * *Ref: `tech-stack/02_backend_reference.md` (Node.js & JavaScript)*

2.  **Node.js Core:**
    * File System (fs), HTTP Module, Streams.
    * Gerenciamento de Pacotes (npm/yarn).

     **Definition of Done (DoD):**
* Consigo explicar o Event Loop sem gaguejar?
* Sei criar um servidor HTTP sem usar Express?

---

##  Fase 2: Construção de APIs Profissionais
> **Foco:** Estrutura, Tipagem e Protocolos.
> **Projeto Sugerido:** API do Projeto Lucienne (CRUD de Livros).

1.  **TypeScript Integration:**
    * Configuração do `tsconfig.json`.
    * Interfaces vs Types.
    * Tipagem de Express Request/Response.
    * *Ref: `tech-stack/02_backend_reference.md` (TypeScript)*

2.  **RESTful Mastery:**
    * Verbos HTTP (GET, POST, PUT, DELETE, PATCH).
    * Status Codes (2xx, 4xx, 5xx) e tratamento de erros.
    * Middlewares (Auth, Validation).

3.  **Dockerização Inicial:**
    * Criar Dockerfile para a API Node.
    * Rodar a aplicação isolada em container.
    * *Ref: `tech-stack/02_backend_reference.md` (Infraestrutura & Docker)*

     **Definition of Done (DoD):**
* Minha API valida dados de entrada (Zod/Joi)?
* O projeto roda com um único comando `docker run`?

---

## Fase 3: Persistência e Dados
> **Foco:** Modelagem Relacional e Integridade.

1.  **PostgreSQL & SQL:**
    * Modelagem de tabelas (Relacionamentos 1:N, N:N).
    * Queries puras vs ORM (Prisma/TypeORM).
    * Migrations (Versionamento de Banco).
    * *Ref: `tech-stack/02_backend_reference.md` (Banco de Dados)*

2.  **Integração Docker Compose:**
    * Subir API + Banco Postgres juntos via Compose.

    **Definition of Done (DoD):**
* Consigo fazer um JOIN complexo?
* Se eu apagar o container do banco, os dados persistem (Volumes)?

---

## Fase 4: Arquitetura e Qualidade (O Pulo para Sênior)
> **Foco:** Manutenibilidade, Testes e Design Patterns.
> **Projeto Sugerido:** Refatoração do Bot WhatsApp ou Garimpo Smart.

1.  **Clean Code & Refactoring:**
    * Eliminar "Magic Numbers" e funções gigantes.
    * Aplicar Dependency Injection.
    * *Ref: `architecture/03_clean_code_standards.md`*

2.  **Design Patterns & SOLID:**
    * Aplicar SRP (Single Responsibility) nos Controllers.
    * Implementar Repository Pattern (Desacoplar do Banco).

3.  **Testes Automatizados:**
    * Unit Tests (Jest/Vitest).
    * Integration Tests.

     **Definition of Done (DoD):**
* Meu código passa no "Code Review Template" do Ritchie?
* Consigo trocar o banco de dados sem reescrever a regra de negócio?

---

##  Fase 5: Carreira e Expansão
> **Foco:** Soft Skills e Visão de Negócio.

1.  **Comunicação Técnica:**
    * Escrever documentação de API (Swagger/OpenAPI).
    * Melhorar README dos projetos.
    * *Ref: `soft-skills/04_career_guide.md`*

2.  **System Design (Básico):**
    * Cache (Redis), Filas (RabbitMQ/Kafka) - *Próximos passos*.
