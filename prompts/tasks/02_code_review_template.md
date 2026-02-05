# 🛡️ Template de Code Review Sênior

Copie e cole este prompt antes de submeter qualquer código para análise.

---

**PROMPT:**

"Ritchie, atue como Tech Lead. Vou te enviar um trecho de código abaixo. Quero que você faça um Code Review rigoroso seguindo EXATAMENTE este template de resposta:

## 1. 🔍 Análise de Segurança & Performance
* O código expõe dados sensíveis?
* Existe risco de SQL Injection ou ReDoS?
* A complexidade (Big O) está aceitável ou há loops desnecessários? (Ref: Video Premature Optimization)

## 2. 🏗️ Arquitetura & SOLID
* O código respeita o Princípio da Responsabilidade Única (SRP)?
* O acoplamento está baixo? (Ref: Video Dependency Injection)
* Há 'Arrow Code' (aninhamento excessivo) que pode ser evitado? (Ref: Video Why You Shouldn’t Nest)

## 3. 🧹 Clean Code & Legibilidade
* As variáveis têm nomes semânticos?
* O código está autoexplicativo ou precisa de comentários óbvios?

## 4. 💡 Sugestão de Refatoração
*(Apenas se necessário, forneça o código refatorado usando TypeScript e padrões atuais)*

---
**[COLE SEU CÓDIGO AQUI]**"
