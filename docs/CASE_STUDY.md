# Project Case Study: Ritchie AI Framework
> **Subtítulo:** Engenharia de Conhecimento aplicada à Mentoria de Carreira Sênior.

## 1. O Problema
O autoestudo em programação sofre de dois problemas crônicos:
* **Passividade:** Consumir vídeos e artigos sem ser desafiado.
* **Falta de Feedback Sênior:** Não ter quem diga "isso funciona, mas é má arquitetura".

Os chats de IA genéricos (ChatGPT/Gemini) ajudam, mas sofrem de alucinação e falta de contexto específico sobre a stack e o nível do usuário.

## 2. A Solução: Knowledge as Code
O **Ritchie** é um framework de mentoria construído sobre o conceito de *Knowledge as Code* (Conhecimento como Código). Ao invés de usar prompts soltos, o projeto estrutura o conhecimento em um repositório Git organizado, servindo como **Dataset Curado** para uma LLM (Google NotebookLM).

O objetivo não é apenas "tirar dúvidas", mas simular a experiência de trabalhar lado a lado com um Tech Lead exigente.

## 3. Arquitetura do Sistema
O projeto é dividido em três camadas lógicas que alimentam a janela de contexto da IA:

### Camada 1: Sources (A Verdade Técnica)
Arquivos Markdown que atuam como a "memória de longo prazo" do mentor.
* **Tech Stack:** Referências oficiais de Node.js, Docker e TypeScript.
* **Architecture:** Princípios de Clean Code, SOLID e Design Patterns.
* **Roadmap & Nivelamento:** A trilha de estudos (`learning_path.md`) se inicia com os fundamentos de lógica (`00_logic_fundamentals.md`), garantindo uma base sólida até para iniciantes. Isso impede que a IA pule etapas cruciais.

### Camada 2: Core Persona (O Comportamento)
Um System Prompt rigoroso (`01_system_prompt.md`) injetado como arquivo-fonte. Ele reescreve o comportamento padrão da IA para:
* Proibir respostas prontas (força o raciocínio socrático).
* Usar analogias personalizadas (ex: mecânica de motos).
* Cobrar postura profissional.

### Camada 3: Tasks (As Ferramentas de Interação)
Scripts prontos (Prompts) que o usuário executa para mudar o modo de operação da IA:
* **Dynamic Assessment:** A IA gera perguntas de entrevista baseadas no histórico recente.
* **Crisis Simulator:** Gera logs de erro fictícios para treino de debugging.
* **Senior Code Review:** Checklist automatizado de segurança e performance.

## 4. Diferenciais Técnicos (Why it works)
* **Context Grounding:** A IA só responde baseada nos arquivos `.md` fornecidos, eliminando alucinações comuns de IAs genéricas.
* **Single Source of Truth:** A manutenção do conhecimento é feita via Git. Se uma tecnologia muda (ex: Node 20 para 22), basta atualizar o arquivo `.md` e a IA se atualiza automaticamente.
* **Scalability:** O modelo permite adicionar novos módulos (ex: Front-End, DevOps) apenas criando novas pastas em `/sources`.

## 5. Resultados
O projeto transformou o processo de estudo passivo em um **Ambiente de Treinamento Ativo**, onde o desenvolvedor é constantemente avaliado, corrigido e desafiado por uma IA que conhece profundamente seu contexto e objetivos.
