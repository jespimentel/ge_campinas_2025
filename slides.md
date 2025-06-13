---
marp: true
---
# IA APLICADA À PROMOTORIA DE JUSTIÇA 
## Prática e engenharia de prompt para o Ministério Público

José Eduardo de Souza Pimentel

GE Campinas - 26/06/2025

---
## Apostila:
## https://jespimentel.github.io/ia_gen_na_promotoria

## Repositório dos prompts do GE: 
## https://github.com/jespimentel/ge_campinas_2025

---

# O que são modelos de linguagem

## Visão geral

- Modelos aprendem como as informações se organizam e estão estatisticamente distribuídas no _corpus_ de treinamento.
- LLMs: geram textos coerentes e relevantes em resposta aos comandos dos usuários (_prompts_).
- Não possuem conhecimentos factuais.

## Alucinações
- Respostas baseadas nos padrões probabilísticos aprendidos durante o treinamento

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

- **Contexto**: fornece informações de fundo ou situacionais que ajudam o modelo a entender melhor o cenário e a aplicar corretamente as instruções.
- **Instruções**: define as tarefas que o modelo deve executar (exemplos: "analise", "compare", "liste", "reescreva", “resuma de forma estruturada”). 
- **Dados de entrada**: consistem no material específico sobre o qual a instrução deve operar (exemplo: texto legal, peças de um inquérito civil, um acórdão)
- **Tipo de saída esperada**: orienta o modelo sobre a forma de apresentar a resposta (exemplos: "em formato de tabela", "como uma lista de pontos (bullet points)", "em linguagem formal", "com no máximo 2 parágrafos", "na forma do template fornecido"). 
---
# Dicas:

- Comece simples
- Dê um papel à LLM
- Adicione contexto relevante
- Divida tarefas complexas
- Use instruções claras e diretas
- Seja específico e forneça exemplos
- Diga o que não fazer
- Dê feedbacks ao modelo
- Utilize tags ou Markdown

---

# Construção de agentes, GEMs e GPTs


---

# Análise de um processo com o NotebookLM

---

# _Visual law_

- Infográficos
- Linha do tempo
- Esquemas (DOT e Mermaid)

---
# Perguntas?

linkedin.com/in/jespimentel
jespimentel.blogspot.com
github.com/jespimentel

pimentel@mpsp.mp.br