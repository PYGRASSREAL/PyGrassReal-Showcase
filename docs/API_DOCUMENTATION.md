# 🔑 PyGrassReal Cloud API Reference Guide

PyGrassReal provides high-performance API endpoints compatible with the **OpenAI Standard Format**. You can seamlessly integrate it into Python SDKs, LangChain, n8n, VSCode/Cursor, and CAD software environments.

---

## 🌐 Endpoint & Authentication

* **Base URL:** `https://api.pygrassreal.ai/v1`
* **Authorization Header:** `Bearer pgr_live_xxxxxxxxxxxxxxxxxxxxxxxx`

---

## 📋 Available Model Endpoints

| Model String | Specialization | Input (per 1M) | Output (per 1M) |
| :--- | :--- | :---: | :---: |
| `pygrassreal/phralak1.5` | 3D Geometry scripts, Python & CAD modeling | $0.35 | $1.50 |
| `pygrassreal/hanuman1.5` | Architectural RAG & building standards | $0.35 | $1.50 |
| `pygrassreal/sampati1` | Live web search grounding & market pricing | $0.35 | $1.50 |
| `pygrassreal/sida1.5` | Perspective sketching & texture generation | $0.71 | $4.29 |
| `pygrassreal/nilapat1.5` | Prompt-to-3D mesh & Gaussian Splats | $0.07143 / Model | — |
| `pygrassreal/sadayu1.5` | Architectural video walkthroughs | $0.36 | $2.14 (Video: $0.04286 / sec) |

---

## 💻 Code Examples

### 1. Python (OpenAI Client)
```python
from openai import OpenAI

client = OpenAI(
    base_url="https://api.pygrassreal.ai/v1",
    api_key="pgr_live_your_api_key_here"
)

response = client.chat.completions.create(
    model="pygrassreal/phralak1.5",
    messages=[
        {"role": "system", "content": "You are an expert computational CAD assistant."},
        {"role": "user", "content": "Generate a Python script to compute foundation grid coordinates for a circular tower."}
    ]
)

print(response.choices[0].message.content)
```

### 2. cURL (Terminal)
```bash
curl https://api.pygrassreal.ai/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer pgr_live_your_api_key_here" \
  -d '{
    "model": "pygrassreal/hanuman1.5",
    "messages": [
      {"role": "user", "content": "What are the standard setback requirements for high-rise residential towers?"}
    ]
  }'
```

---

## 💳 Manage Keys & Balance
* Manage API keys and pre-fund credits at: [https://api.pygrassreal.ai](https://api.pygrassreal.ai)
* View real-time usage statistics and invocation logs in the developer dashboard.
