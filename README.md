# 🧙‍♂️ Ritchie: The AI Senior Mentor Guide

![Status](https://img.shields.io/badge/Status-Active-success)
![Knowledge Strategy](https://img.shields.io/badge/Strategy-Knowledge_as_Code-blueviolet)
![Focus](https://img.shields.io/badge/Focus-Seniority_Acceleration-orange)
![Tech Stack](https://img.shields.io/badge/Stack-Node_%7C_TS_%7C_Docker-green)

> *"UNIX is basically a simple operating system, but you have to be a genius to understand the simplicity."* — **Dennis Ritchie**

---

## O que é este projeto?

O **Ritchie AI Guide** não é apenas uma lista de estudos. É um projeto de **Engenharia de Conhecimento** projetado para transformar documentação estática (vídeos, docs, artigos) em um **Contexto Ativo** para Inteligências Artificiais.

Ao invés de consumir conteúdo passivamente, eu estruturei as melhores referências do mercado (Clean Code, SOLID, Arquitetura Hexagonal) em arquivos Markdown otimizados (`sources/`). Quando alimentados em uma LLM (como o Google NotebookLM ou Gemini), esses arquivos criam a persona de um **Mentor Sênior** que:

1. Conhece minha stack tecnológica profundamente.
2. Realiza Code Reviews baseados em princípios rígidos de engenharia.
3. Me guia na tomada de decisões arquiteturais.

## Por que "Ritchie"?

O nome é uma homenagem a **Dennis Ritchie**, criador da linguagem C e do sistema Unix. Ele representa a fundação, a simplicidade e a importância de entender como as coisas funcionam "debaixo do capô". Este guia busca trazer essa mesma solidez para o meu aprendizado de Back-End Moderno.

## Estrutura do Conhecimento

O repositório aplica o conceito de **"Knowledge as Code"**, versionando o conhecimento como se fosse software:

```text
/sources
  ├── /tech-stack       # O "Manual Técnico" (Node.js, Docker, TS, DBs)
  ├── /architecture     # A "Constituição" (Clean Code, SOLID, Design Patterns)
  └── /soft-skills      # O "Guia de Carreira" (Postura, Comunicação, Mercado)
```


## Como Utilizar: Setup em 3 Passos

Para ativar o mentor "Ritchie" em uma IA como o Google NotebookLM ou Gemini, siga este fluxo que separa claramente o **Contexto** da **Instrução**.

### Passo 1: Fornecer o Contexto (Sources)

A IA precisa da base de conhecimento. Faça o upload de **todos os arquivos `.md`** localizados dentro das pastas em `/sources` para a área de fontes da sua IA.

- `sources/tech-stack/`
- `sources/architecture/`
- `sources/soft-skills/`

Estes arquivos funcionam como a "biblioteca" do mentor, contendo todos os padrões e tecnologias que ele deve dominar.

### Passo 2: Ativar a Persona (Prompt)

Para que a IA assuma a personalidade e as diretrizes do mentor sênior, copie o conteúdo completo do arquivo abaixo e **cole como a primeira mensagem no chat**:

- `prompts/core-persona/system_prompt.md`

Este prompt instrui a IA a agir como "Ritchie", um especialista exigente e focado nos padrões definidos nos seus arquivos-fonte.

### Passo 3: Interagir com o Mentor

Com o contexto carregado e a persona ativada, você pode começar a interagir. Seja específico e direto.

**Exemplo de prompt de uso:**

> *"Ritchie, recebi uma nova demanda para criar um microsserviço de notificações. Com base na nossa documentação de arquitetura, qual padrão (REST, gRPC ou outro) você recomendaria e por quê? Detalhe os trade-offs."*

Este processo garante que a IA não apenas tenha acesso à informação, mas que atue sobre ela com a intencionalidade que você definiu.
