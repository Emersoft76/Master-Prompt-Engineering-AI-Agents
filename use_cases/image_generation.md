# ✅ Caso de Uso: Geração de Imagens com IA | Use Case: Image Generation with AI

## 📌 Objetivo | Goal
Demonstrar como gerar imagens automaticamente utilizando IA.

Show how to generate images automatically using AI.

---

## 🚀 Exemplo 1: Criação de Imagens para Redes Sociais | Example 1: Social Media Image Creation

### 🔹 Prompt:
"Você é um assistente de IA que gera imagens para redes sociais. Crie uma imagem de um café quente em uma mesa de madeira."

"You are an AI assistant that generates images for social media. Create an image of a hot coffee on a wooden table."

### 🔹 Ferramenta Utilizada | Tool Used:
- DALL-E (OpenAI Image Generation API).

### 🔹 Código de Exemplo (Python) | Example Code (Python)
```python
import openai

openai.api_key = "SUA_CHAVE_API_AQUI"

response = openai.Image.create(
    prompt="A hot coffee on a wooden table",
    n=1,
    size="512x512"
)

image_url = response['data'][0]['url']
print("Imagem Gerada:", image_url)
```
🔹 Resultado Esperado | Expected Result:

Uma imagem de um café quente em uma mesa de madeira.

---

## 🚀 Exemplo 2: Imagem de Produto para E-commerce | Example 2: Product Image for E-commerce

### 🔹 Prompt:
"Crie uma imagem de um tênis esportivo branco em fundo transparente."

"Create an image of a white sports shoe on a transparent background."

### 🔹 Código de Exemplo (Python) | Example Code (Python)
```python
response = openai.Image.create(
    prompt="A white sports shoe on a transparent background",
    n=1,
    size="512x512"
)

image_url = response['data'][0]['url']
print("Imagem Gerada:", image_url)
```
🔹 Resultado Esperado | Expected Result:

Uma imagem de um tênis esportivo branco com fundo transparente.

---
