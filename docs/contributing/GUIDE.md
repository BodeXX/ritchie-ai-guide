# 👷 Guia de Contribuição (Contributing Guide)

Obrigado pelo interesse em contribuir com o **Ritchie AI Guide**!
Este documento define os padrões para garantir que nossa base de conhecimento continue limpa, organizada e útil para mentoria via IA.

---

## 🚀 Como Contribuir (Fluxo Git)

Para contribuir, seguimos o fluxo padrão de Pull Requests do GitHub (Fork & Branch Workflow):

1.  **Faça um Fork** deste repositório para sua conta.
2.  **Crie uma Branch** para sua feature ou correção:
    ```bash
    git checkout -b feature/nome-da-sua-contribuição
    # Exemplo: git checkout -b docs/adiciona-video-clean-arch
    ```
3.  **Faça as alterações** seguindo os padrões abaixo.
4.  **Commit suas mudanças** (usamos *Conventional Commits*):
    ```bash
    git commit -m "docs(tech-stack): adiciona referência sobre NestJS"
    # Padrões: feat, fix, docs, refactor, style, test
    ```
5.  **Faça o Push** para seu fork:
    ```bash
    git push origin feature/nome-da-sua-contribuição
    ```
6.  **Abra um Pull Request (PR)** no repositório original descrevendo o que você adicionou e o porquê.

---

## 📐 Padrões de Conteúdo

A IA depende de uma estrutura rígida para entender o contexto. Não quebre o padrão.

### 1. Adicionando Links (`sources/`)
Nunca adicione apenas a URL. A IA precisa saber *sobre o que* é aquele link para recomendá-lo no momento certo.

* **❌ Errado:**
    `- https://youtube.com/watch?v=...`
* **✅ Correto:**
    `- [Título do Vídeo ou Artigo](URL) - Uma frase descrevendo o conceito chave abordado (ex: "Explica a diferença entre Docker Images e Containers").`

### 2. Criando Tasks (`prompts/tasks/`)
Se você criou um prompt novo (ex: simulador de entrevista), ele deve ser "Copy-Paste Ready".
* Comece com um título H1 (`#`).
* Inclua uma breve descrição.
* Coloque o prompt dentro de um bloco de citação (`> "Texto..."`) ou code block para facilitar a cópia.

---

## 🔍 Checklist do Code Review (Antes de abrir PR)
Antes de submeter, verifique:
- [ ] Removi numerações automáticas (ex: "Video 01")?
- [ ] Os links estão funcionando?
- [ ] O commit segue o padrão convencional (`tipo(escopo): mensagem`)?
- [ ] A documentação está em Markdown limpo?

---
<div align="center">
  <sub>Dúvidas? Abra uma <strong>Issue</strong> para discutirmos antes de codar!</sub>
</div>
