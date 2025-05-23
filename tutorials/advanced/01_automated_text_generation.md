# ✅ Tutorial Avançado: Geração de Texto Automatizada | Advanced Tutorial: Automated Text Generation

## 📌 Objetivo | Goal
Aprender como criar textos automaticamente utilizando IA, configurando o modelo para gerar conteúdo de forma contínua e ajustável.

Learn how to automatically generate text using AI, configuring the model to generate content continuously and adjustably.

---

## 🚀 Exemplo 1: Geração Automática de Resumos | Example 1: Automatic Summary Generation

### 🔹 Prompt:
"Você é um assistente de IA especializado em resumir textos. Gere um resumo para o texto a seguir: [TEXTO AQUI]."

"You are an AI assistant specialized in summarizing texts. Generate a summary for the following text: [TEXT HERE]."

### 🔹 Código de Exemplo (Python) | Example Code (Python)
```python
import openai

openai.api_key = "SUA_CHAVE_API_AQUI"

def gerar_resumo(texto):
    resposta = openai.Completion.create(
        engine="text-davinci-003",
        prompt=f"Resuma o seguinte texto: {texto}",
        max_tokens=150
    )
    return resposta.choices[0].text.strip()

texto_exemplo = "A inteligência artificial está revolucionando o mundo, com aplicações em diversas áreas, como saúde, finanças e educação."
resumo = gerar_resumo(texto_exemplo)
print("Resumo:", resumo)
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
