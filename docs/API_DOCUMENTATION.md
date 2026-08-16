# 🔑 เอกสารแนะนำการเชื่อมต่อ PyGrassReal Cloud API (API Reference Guide)

PyGrassReal ให้บริการ API เชื่อมต่อกับระบบปัญญาประดิษฐ์ Multi-Agent และ Geometry Engine ในรูปแบบมาตรฐาน **OpenAI Compatible Endpoint** สามารถนำไปผสานการทำงานร่วมกับ Python SDK, LangChain, n8n, VSCode/Cursor, หรือโปรแกรม 3D CAD ได้อย่างง่ายดาย

---

## 🌐 Endpoint & Authentication

* **Base URL:** `https://api.pygrassreal.ai/v1`
* **Authorization Header:** `Bearer pgr_live_xxxxxxxxxxxxxxxxxxxxxxxx`

---

## 📋 รายการโมเดลที่พร้อมให้บริการ (Available Models)

| Model String | หน้าที่หลัก | Backend Engine | Pricing (Per 1M Tokens) |
| :--- | :--- | :--- | :--- |
| `pygrassreal/phralak1.5` | โค้ดเรขาคณิต 3D, Python, CAD Scripting | Gemini 3.5 Flash-Lite | In: $0.35 / Out: $1.50 |
| `pygrassreal/hanuman1.5` | ฐานความรู้สถาปัตยกรรม & กฎหมายอาคาร (RAG) | Gemini 3.1 Flash-Lite + RAG | In: $0.35 / Out: $1.50 |
| `pygrassreal/sampati1` | ดึงข้อมูลวัสดุและราคาตลาดสดจากอินเทอร์เน็ต | Google Search Grounding | In: $0.35 / Out: $1.50 |
| `pygrassreal/sida1.5` | เจนภาพแบบร่าง Perspective & Texture | Gemini 3.1 Flash Image | In: $0.71 / Out: $4.29 |
| `pygrassreal/nilapat1.5` | สร้าง 3D Mesh / Splats จาก Prompt | TripoSplat 3D Engine | $0.07143 / Generation |
| `pygrassreal/sadayu1.5` | เจนวิดีโอ Architectural Walkthrough | Veo 3.1 Lite | $0.0429 / วินาที (720p) |

---

## 💻 ตัวอย่างการเรียกใช้งานโค้ด (Code Examples)

### 1. การใช้งานผ่าน Python (OpenAI Client)
```python
from openai import OpenAI

client = OpenAI(
    base_url="https://api.pygrassreal.ai/v1",
    api_key="pgr_live_your_api_key_here"
)

response = client.chat.completions.create(
    model="pygrassreal/phralak1.5",
    messages=[
        {"role": "system", "content": "คุณคือ AI ผู้เชี่ยวชาญการเขียนสคริปต์ 3D CAD"},
        {"role": "user", "content": "สร้างฟังก์ชัน Python คำนวณพิกัดเสาเข็มแบบ Grid สำหรับอาคารทรงกลม"}
    ]
)

print(response.choices[0].message.content)
```

### 2. การใช้งานผ่าน cURL (Terminal)
```bash
curl https://api.pygrassreal.ai/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer pgr_live_your_api_key_here" \
  -d '{
    "model": "pygrassreal/hanuman1.5",
    "messages": [
      {"role": "user", "content": "ระยะร่นอาคารสูงตามกฎกระทรวงฉบับที่ 33 ต้องเว้นเท่าไหร่?"}
    ]
  }'
```

---

## 💳 การจัดการ Wallet & API Key
* ลงทะเบียนและรับ API Key ได้ที่: [https://api.pygrassreal.ai](https://api.pygrassreal.ai)
* ตรวจสอบ Usage & Logs แบบ Real-time ได้ในหน้า Developer Console
