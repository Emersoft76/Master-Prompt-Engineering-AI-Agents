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

"Notícia 1: Nova IA revoluciona o diagnóstico médico."

"Notícia 2: Ferramenta de IA melhora a análise de dados financeiros."

"Notícia 3: IA generativa é usada para criar conteúdo educacional."

---

## 🚀 Exemplo 2: Agente de Automação de Tarefas | Example 2: Task Automation Agent

### 🔹 Prompt:
"Você é um assistente de IA que agenda compromissos automaticamente. Agende uma reunião para amanhã às 15:00."

"You are an AI assistant that schedules appointments automatically. Schedule a meeting for tomorrow at 3:00 PM."

### 🔹 Código de Exemplo (Python) | Example Code (Python)
```python
from datetime import datetime, timedelta

def agendar_reuniao():
    data = datetime.now() + timedelta(days=1)
    horario = "15:00"
    return f"Reunião agendada para {data.strftime('%d/%m/%Y')} às {horario}."

print(agendar_reuniao())
```
🔹 Resultado Esperado | Expected Result:

"Reunião agendada para [DATA] às 15:00."

---

## ✅ Dicas para Agentes Inteligentes | Intelligent Agent Tips

* Defina claramente a função do agente (busca, automação, controle).

* Combine o uso de IA com bibliotecas externas (requests, datetime).

* Garanta que o agente seja seguro e não execute ações perigosas automaticamente.

* Clearly define the agent's function (search, automation, control).

* Combine AI with external libraries (requests, datetime).

* Ensure the agent is secure and does not perform dangerous actions automatically.
---
