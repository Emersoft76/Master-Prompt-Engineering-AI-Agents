# ✅ Tutorial Avançado: Integração com APIs | Advanced Tutorial: API Integration

## 📌 Objetivo | Goal
Aprender a integrar IA com APIs externas para buscar dados em tempo real.

Learn how to integrate AI with external APIs to fetch real-time data.

---

## 🚀 Exemplo: Integração com API de Clima | Example: Weather API Integration

### 🔹 Código de Exemplo (Python) | Example Code (Python)
```python
import requests

def obter_clima(cidade):
    api_key = "SUA_CHAVE_API_CLIMA_AQUI"
    url = f"http://api.openweathermap.org/data/2.5/weather?q={cidade}&appid={api_key}&lang=pt_br"
    resposta = requests.get(url)
    dados = resposta.json()
    clima = dados["weather"][0]["description"]
    temperatura = dados["main"]["temp"] - 273.15  # Convertendo de Kelvin para Celsius
    return f"O clima em {cidade} é {clima} com temperatura de {temperatura:.2f}°C."

print(obter_clima("São Paulo"))
```
🔹 Resultado Esperado | Expected Result:

"O clima em São Paulo é nublado com temperatura de 25.34°C."

---
