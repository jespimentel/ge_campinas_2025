---
marp: true
---
# IA APLICADA À PROMOTORIA DE JUSTIÇA 
## Prática e engenharia de prompt para o Ministério Público

José Eduardo de Souza Pimentel

GE Campinas - 26/06/2025

---
# Objetivos

- Visão geral sobre processamento de linguagem natural
- Noções de engenharia de prompt
- Criação de Agentes, GEMs e GPTs para a Promotoria
- Outras aplicações

---

# Repositório dos prompts do GE: 

## https://github.com/jespimentel/ge_campinas_2025

---

# O que são modelos de linguagem

## Visão geral

- Modelos aprendem como as informações se organizam e estão estatisticamente distribuídas no _corpus_ de treinamento.
- LLMs: geram textos coerentes e relevantes em resposta aos comandos (_prompts_).
- Não possuem conhecimentos factuais.

---

## Privacidade

- Conhecer termos de uso e opções opt-in ou opt-out dos provedores

## Alucinação
- Modelos não possuem compreensão real dos assuntos
- Respostas plausíveis (baseadas em padrões probabilísticos)
- Em regram não verificam a veracidade ou a completude das informações

## Sugestões:
- Conferir as informações geradas
- Não utilizar como única fonte de pesquisa
- Estar cientes das limitações da tecnologia

---

# Regulamentação

- PCA nº 0000416-89.2023.2.00.0000 (j. 21/06/2024)
- Resolução nº 332/2020 (atualiz. em 18/02/2025)
	- assinatura ou cadastro privado (se não tiver solução corporativa)
	- neste caso, proibido em dados sigilosos ou protegidos por segredo de justiça
- Crítica: solução de produtividade pessoal

---
# Modelos. Qual escolher?

- Copilot
- Gemini (*)
- ChatGPT
- NotebookLM 
- Perplexity
- Outras

---
# Engenharia de prompt

- **Contexto**: fornece informações situacionais que ajudam o modelo a compreender melhor o cenário sobre o qual ele aplicará as instruções.
- **Dados de entrada**: informação ou arquivo fornecido à IA para processamento.
- **Persona**: define o papel do modelo (exemplo: "Você é um promotor de justiça.")
- **Tarefas**: define as tarefas que o modelo deve executar (exemplos: "analise", "compare", "liste", "reescreva", “resuma de forma estruturada”). 
- **Formato de saída**: orienta o modelo sobre a forma de apresentar a resposta (exemplos: "em formato de tabela", "como uma lista de pontos (bullet points)", "em linguagem formal", "com no máximo 2 parágrafos", "na forma do(s) exemplo(s) fornecido(s)"). 
---
# Dicas:

- Comece simples
- Divida tarefas complexas
- Dê um papel ao modelo
- Adicione contexto relevante
- Use instruções claras, específicas e diretas
- Forneça exemplos
- Diga o que não fazer
- Utilize XML e/ou Markdown
- Converse com o modelo (forneça feedbacks) 

---
# "Vazamento" do System Prompt da Anthropic

- [System Prompt do Claude 4](https://github.com/elder-plinius/CL4R1T4S/blob/main/ANTHROPIC/Claude_4.txt) - 22/05/2025

**Lições aprendidas:**
- O prompt pode ser grande (15k+)
- Seções estruturadas por XML: <externa><interna></interna></externa>
- Emprego de "intenções declarativas" (capacidades e limitações)
- Uso de lógica condicional (muitos "if")
- Repetição das instruções importantes
- Ênfases com maiúsculas e um pouco de Markdown (#, ** e -)
- Restrições: "DO NOT", "Do not" e "don't"
- Exemplos: bons e maus

---

# Construção de Agentes (Copilot), GEMs e GPTs

- Especificidades
- Capacidades
- Pros e Cons

---

# Análise de um processo com o NotebookLM

- Visão geral
- Tipos de fontes
- Documento de resumo
- Mapa mental
- Linha do tempo
- Conversa aprofundada (personalização)

---

# _Visual law_

- Infográficos
- Linha do tempo
- Esquemas (com Mermaid)

---
# Para saber mais:

[A IA GENERATIVA NA PROMOTORIA (Pimentel)](https://github.com/jespimentel/ia_gen_na_promotoria/raw/main/apostila/IA_Gen_Promotoria_Pimentel.pdf)

[Prompting Guide 101 (Google)](https://workspace.google.com/learning/content/gemini-prompt-guide?hl=pt-BR)

[What Is ChatGPT Doing … and Why Does It Work? (Stephen Wolfram)](https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/)


---

# Perguntas? Obrigado!

linkedin.com/in/jespimentel

jespimentel.blogspot.com

github.com/jespimentel

pimentel@mpsp.mp.br