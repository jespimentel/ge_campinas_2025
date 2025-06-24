---

marp: true

---

# IA APLICADA À PROMOTORIA DE JUSTIÇA 
## Prática e engenharia de prompt para o Ministério Público

José Eduardo de Souza Pimentel

GE "Campos Salles" | Campinas, 26/06/2025

---

# Objetivos

- Visão geral sobre o tema
- Noções de "Engenharia de Prompt"
- Aplicações práticas: Agentes, GEMs e GPTs
- Dicas para a implementação

---

# Fora do escopo (mas possível com LLMs)

- Obtenção de hashes e manipulação de arquivos
- Obtenção de frames e tratamento de imagens
- Análise de dados
- Brainstorm
- Encadeamento de prompts
- Etc... (é um "canivete suíço")

## Disponível em: [ESMP](https://mpspbr.sharepoint.com/sites/acervo-videos-stream/Documentos%20Compartilhados/Forms/AllItems.aspx?id=%2Fsites%2Facervo%2Dvideos%2Dstream%2FDocumentos%20Compartilhados%2FESMPSP%2FEventos%2F2025%5FIA%20Generativa%20na%20Promotoria%5FAprendizados%2C%20Limita%C3%A7%C3%B5es%20e%20o%20que%20Funciona%20Agora&p=true&ga=1) e [Apostila](https://github.com/jespimentel/ia_gen_na_promotoria/raw/main/apostila/IA_Gen_Promotoria_Pimentel.pdf) 

---

# Slides

![QR code do site](img/qr_ge_campinas_2025.png)

<https://jespimentel.github.io/ge_campinas_2025/>

---

# Repositório dos prompts deste GE: 

<https://github.com/jespimentel/ge_campinas_2025/tree/main/prompts>

---

# O que são modelos de linguagem

## Visão geral

- Modelos aprendem como as informações se organizam e estão estatisticamente distribuídas no corpus de treinamento
- LLMs: geram textos coerentes e relevantes em resposta aos comandos (**prompts**)
- Não possuem conhecimentos factuais

---

## Privacidade

- Conhecer termos de uso e opções opt-in ou opt-out dos provedores

## Alucinação

- Modelos não possuem compreensão real dos assuntos
- Respostas plausíveis (baseadas em padrões probabilísticos)
- Em regra, não verificam a veracidade ou a completude das informações

## Sugestões:

- Conferir as informações geradas
- Não utilizar como única fonte de pesquisa
- Estar cientes das limitações da tecnologia

---

# Regulamentação

- PCA nº 0000416-89.2023.2.00.0000 (j. 21/06/2024)
- Resolução nº [615/2025 - CNJ](https://atos.cnj.jus.br/files/original1555302025031467d4517244566.pdf)
	- assinatura ou cadastro privado (se não tiver solução corporativa)
	- neste caso, proibido em dados sigilosos ou protegidos por segredo de justiça
- Críticas:
	- solução de produtividade pessoal
	- assimetria com Defensores/Advogados

---

# Modelos. Qual escolher?

- Copilot
- Gemini (*)
- ChatGPT
- NotebookLM 
- Perplexity
- Outros

---

# Engenharia de prompt

- **Contexto**: fornece informações situacionais que ajudam o modelo a compreender melhor o cenário sobre o qual ele aplicará as instruções.
- **Dados de entrada**: informação ou arquivo fornecido à IA para processamento.
- **Persona**: define o papel do modelo (exemplo: "Você é um promotor de justiça.")
- **Tarefas**: define as tarefas que o modelo deve executar (exemplos: "analise", "compare", "liste", "reescreva", “resuma de forma estruturada”). 
- **Formato de saída**: orienta o modelo sobre a forma de apresentar a resposta (exemplos: "em formato de tabela", "como uma lista de pontos (bullet points)", "em linguagem formal", "com no máximo 2 parágrafos", "na forma do(s) exemplo(s) fornecido(s)"). 
---

# Dicas para a elaboração de bons prompts:

- Comece simples
- Divida tarefas complexas
- Dê um papel ao modelo
- Adicione contexto relevante
- Use instruções claras, específicas e diretas
- Forneça exemplos
- Diga o que não fazer
- Utilize tags (<tag></tag>) e/ou Markdown (#, ** e -)
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

# Estratégias

- Corretor de peças (prompt básico)
- Audiência de custódia (resultado formatado)
- MPU (placeholder + separação fato/fundamento)
- Resumidor de IP (uso de exemplos no prompt)
- Peças processuais (roteiro a ser seguido)
- Denunciador "preguiçoso" (uso de base de conhecimento)

---

# Análise de um processo com o NotebookLM

- Visão geral
- Tipos de fontes
- Documento de resumo
- Mapa mental
- Linha do tempo
- Conversa aprofundada (personalização)

---

# Visual Law

- Infográficos
- Linha do tempo
- Esquemas (com Mermaid)

---

# Dicas de implementação

- Casos simples
- Criação de agentes "especializados"
- Nova configuração de peças:
	- fatos
	- fundamentos jurídicos
	- identificação dos casos reaproveitáveis (recuperação)
- GoogleKeep (ou equivalente)
	- BD de prompts e aprendizado compartilhado
	- BD de teses e julgados  

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