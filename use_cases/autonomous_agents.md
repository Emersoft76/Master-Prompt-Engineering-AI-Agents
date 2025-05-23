# ✅ Caso de Uso: Agentes Inteligentes com IA | Use Case: Intelligent Agents with AI

## 📌 Objetivo | Goal
Demonstrar como criar agentes inteligentes que executam tarefas automaticamente, como buscar informações, realizar cálculos e muito mais.

Show how to create intelligent agents that automatically perform tasks, such as searching for information, performing calculations, and more.

---

## 🚀 Exemplo 1: Agente de Busca Inteligente | Example 1: Intelligent Search Agent

### 🔹 Prompt:
"Você é um agente de IA que busca informações sobre as últimas tendências em tecnologia."

"You are an AI agent that searches for the latest trends in technology."

### 🔹 Código de Exemplo (Python) | Example Code (Python)
```python
import openai

openai.api_key = "SUA_CHAVE_API_AQUI"

def buscar_tendencias():
    resposta = openai.Completion.create(
        engine="text-davinci-003",
        prompt="Liste as três últimas tendências em tecnologia.",
        max_tokens=100
    )
    return resposta.choices[0].text.strip()

print("Tendências:", buscar_tendencias())
```
🔹 Resultado Esperado | Expected Result:

 * Inteligência artificial generativa.
 
 * Computação quântica.

 * Realidade aumentada aplicada ao comércio.
---

## 🚀 Exemplo 2: Agente de Suporte ao Cliente | Example 2: Customer Support Agent

### 🔹 Prompt:
"Você é um assistente de IA que responde dúvidas de clientes. Ajude um cliente que esqueceu sua senha."

"You are an AI assistant that answers customer questions. Help a customer who forgot their password."

### 🔹 Código de Exemplo (Python) | Example Code (Python)
```python
def suporte_cliente():
    resposta = openai.Completion.create(
        engine="text-davinci-003",
        prompt="Um cliente esqueceu sua senha. Como posso ajudar?",
        max_tokens=100
    )
    return resposta.choices[0].text.strip()

print("Resposta do Suporte:", suporte_cliente())
```
🔹 Resultado Esperado | Expected Result:

"Prezado cliente, para redefinir sua senha, acesse o link 'Esqueci minha senha' na página de login e siga as instruções."

---
  
## ✅ Dicas para Agentes Inteligentes | Intelligent Agent Tips

* Defina claramente o papel do agente (busca, suporte, automação).

* Garanta que o agente tenha acesso seguro a APIs e informações externas.

* Utilize prompts claros para evitar respostas confusas.

* Clearly define the agent's role (search, support, automation).

* Ensure the agent has secure access to APIs and external information.

* Use clear prompts to avoid confusing responses.
---

