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
- LLMs: geram textos coerentes e relevantes em resposta aos comandos (_prompts_).
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
- Utilize tags ou Markdown
- Converse com o modelo (forneça feedbacks) 

---
# Vazamento do System Prompt do Claude 4

- [System Prompt](https://github.com/elder-plinius/CL4R1T4S/blob/main/ANTHROPIC/Claude_4.txt) - 22/05/2025

## Lições aprendidas:
- O prompt pode ser grande (15k+)
- Seções estruturadas por XML: <externa><interna></interna></externa>
- Uso de lógica condicional (muitos "if")
- Repetição das instruções importantes
- Ênfases com maiúsculas e um pouco de Markdown (#, ** e -)
- Restrições: "DO NOT", "Do not" e "don't"
- Exemplos: bons e maus

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
# Para saber mais:
[Prompting Guide 101 (Google)](https://workspace.google.com/learning/content/gemini-prompt-guide?hl=pt-BR)





---
# Perguntas?

linkedin.com/in/jespimentel

jespimentel.blogspot.com

github.com/jespimentel

pimentel@mpsp.mp.br