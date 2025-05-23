# ✅ Tutorial Avançado: Agentes Inteligentes com IA | Advanced Tutorial: Intelligent Agents with AI

## 📌 Objetivo | Goal
Aprender a criar agentes inteligentes que executam tarefas automaticamente, como buscar informações na web ou processar comandos complexos.

Learn how to create intelligent agents that perform tasks automatically, such as fetching information from the web or processing complex commands.

---

## 🚀 Exemplo 1: Agente de Busca Automática | Example 1: Automated Search Agent

### 🔹 Prompt:
"Você é um agente de IA. Busque informações sobre as últimas notícias em inteligência artificial."

"You are an AI agent. Search for the latest news on artificial intelligence."

### 🔹 Código de Exemplo (Python) | Example Code (Python)
```python
import openai
import requests

openai.api_key = "SUA_CHAVE_API_AQUI"

def buscar_noticias():
    resposta = openai.Completion.create(
        engine="text-davinci-003",
        prompt="Liste as três últimas notícias sobre inteligência artificial.",
        max_tokens=150
    )
    return resposta.choices[0].text.strip()

print("Notícias de IA:", buscar_noticias())
```
🔹 Resultado Esperado | Expected Result:

"Resumo: A IA está transformando o mundo, com impacto em saúde, finanças e educação."

---

## 🚀 Exemplo 2: Geração Contínua de Ideias | Example 2: Continuous Idea Generation

### 🔹 Prompt:
"Gere cinco ideias de negócios relacionados a IA."

"Generate five business ideas related to AI."

### 🔹 Código de Exemplo (Python) | Example Code (Python)
```python
def gerar_ideias():
    resposta = openai.Completion.create(
        engine="text-davinci-003",
        prompt="Liste cinco ideias de negócios com IA.",
        max_tokens=100
    )
    return resposta.choices[0].text.strip()

print("Ideias de Negócios:", gerar_ideias())
```
🔹 Resultado Esperado | Expected Result:

 1. Assistente virtual de atendimento ao cliente.

 2. Ferramenta de diagnóstico médico com IA.

 3. Plataforma de educação personalizada com IA.

 4. Gerador de conteúdo para redes sociais.

 5. Analisador de sentimentos em redes sociais.
---

✅ Dicas para Automação | Automation Tips

* Defina claramente o objetivo do texto a ser gerado.

* Ajuste o max_tokens para controlar o tamanho da resposta.

* Use laços (loops) para gerar textos continuamente.

* Clearly define the goal of the text to be generated.

* Adjust max_tokens to control response length.

* Use loops to continuously generate text.
---
