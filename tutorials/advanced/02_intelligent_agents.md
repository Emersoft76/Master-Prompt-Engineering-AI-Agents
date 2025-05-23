
---

## **📁 tutorials/advanced/02_intelligent_agents.md (Tutoriais Avançados - Agentes Inteligentes - PT/EN)**

```markdown
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
