# 🧪 Protocolo de Avaliação Dinâmica (Context-Aware)

Este prompt serve para calibrar o nível do usuário. A IA não deve "inventar" tópicos aleatórios se já estivermos no meio de um estudo, mas sim desafiar o entendimento atual.

---

**COPIE E COLE O PROMPT ABAIXO:**

> "Ritchie, ative o **Modo de Avaliação Dinâmica**. Analise nossa conversa recente e siga o fluxo abaixo:
>
> **PASSO 1: Identificação de Contexto**
> * **Cenário A (Estamos conversando sobre um tema?):** Se eu já estiver fazendo perguntas sobre algo (ex: Docker, Promises, SQL), NÃO mude de assunto. Gere uma pergunta desafiadora **sobre esse tema específico** para testar se eu entendi a profundidade ou apenas a sintaxe.
> * **Cenário B (Sessão Nova/Vazia?):** Se não há contexto recente, faça uma **Varredura Diagnóstica**. Escolha um dos pilares da nossa stack (Node/TS/Arquitetura) e mande uma pergunta para medir meu nível atual.
>
> **PASSO 2: A Pergunta (O Desafio)**
> * Não faça quiz de 'O que é?'.
> * Crie um **Mini-Cenário**: "Imagine que [Contexto Pessoal/Projeto Lucienne] precisa de X..."
> * Se o tema for **Código**, me dê um snippet com um 'code smell' (erro de padrão) sutil e pergunte o que está errado segundo nossos docs de Clean Code.
> * Se o tema for **Carreira**, me coloque numa 'saia justa' de entrevista.
>
> **PASSO 3: O Feedback**
> * Aguarda minha resposta.
> * Se eu acertar: Elogie brevemente e suba a régua (dê um cenário mais complexo sobre o mesmo tema).
> * Se eu errar: Explique o conceito e me indique qual arquivo em `sources/` eu deveria reler."
