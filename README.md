<div align="center">

<a href="https://pygrassreal.ai">
  <img src="assets/logo.png" alt="PyGrassReal Logo" width="220" height="auto" />
</a>

# PyGrassReal
### Next-Generation AI-Driven 3D Computational Design Platform

[![License: Proprietary](https://img.shields.io/badge/License-Commercial%20%2F%20Proprietary-red.svg)](#-license--terms-of-service)
[![Platform](https://img.shields.io/badge/Platform-Web%20%7C%20Windows%20%7C%20iOS%20%7C%20Android%20%7C%20CLI-success)](#-downloads--installation-hub)
[![3D Engine](https://img.shields.io/badge/3D%20Engine-Three.js%20%7C%20Gaussian%20Splats-orange)](#)
[![AI Benchmark](https://img.shields.io/badge/AI%20Benchmark-Rank%20%231%20(49.67%25)-brightgreen)](#-live-ai-benchmark-leaderboard)
[![API Service](https://img.shields.io/badge/API-Pay--As--You--Go-blue)](#-official-api-cloud--pay-as-you-go-pricing)

[🌐 Official Website](https://pygrassreal.ai) • [📦 Download Desktop Installer](#-downloads--installation-hub) • [🔑 Get API Key](https://api.pygrassreal.ai) • [📖 Documentation](docs/API_DOCUMENTATION.md) • [💬 Contact Sales](mailto:admin@pygrassreal.ai)

---

### *"Transforming 3D Architectural & Engineering Visions into Reality with Multi-Agent AI Power"*

</div>

---

## 🌟 Why PyGrassReal?

PyGrassReal is a next-generation 3D Computational Design platform that seamlessly bridges **3D CAD**, **Photorealistic 3D Gaussian Splatting**, and an **Autonomous Multi-Agent AI Reasoning Team**.

### 🚀 Key Highlights
1. **🤖 Multi-Agent AI Reasoning Team**:
   - Specialized AI agents automatically research architectural data, generate precise geometry scripts, and validate engineering integrity.
2. **🏆 #1 Benchmark Accuracy (Industry Leader)**:
   - Evaluated against global frontier models on 3D CAD, Geometry Scripting, and Node Workflows. **`phralak-1.5` ranked #1 overall with 49.67% accuracy** and an astonishing **49.50% in Visual Node Workflows**, outperforming Gemini, Claude, and ChatGPT.
3. **🧊 Photorealistic 3D Gaussian Splatting & WebGL Engine**:
   - Smoothly render massive point clouds, 3D meshes, and real-time Gaussian splats directly in the browser and desktop environment.
4. **🔄 Real-Time Dynamic 3D Adjustments**:
   - Dynamically manipulate complex architectural facades, structural elements, and geometric patterns with instantaneous feedback.
5. **🏢 Unified Cross-Platform Suite**:
   - Work effortlessly across Web Cloud, Desktop Installer (.exe), Mobile Apps (iOS/Android), and the PGR Studio IDE Extension.

---

## 🏆 Live AI Benchmark Leaderboard

<div align="center">

![AI Benchmark Designer & Leaderboard](assets/benchmark-chart.svg)

*Live interactive evaluation scores verified at **[pygrassreal.ai/dashboard/benchmark](https://pygrassreal.ai/dashboard/benchmark)***

</div>

---

## 📦 Downloads & Installation Hub

We offer flexible deployment options across desktop, cloud, mobile, and developer tooling:

### 1. 💻 Windows Desktop Application
Optimized for maximum 3D rendering throughput, large Gaussian splat files, and offline capability.
* 📥 **[Download PyGrassReal Setup (.exe)](https://github.com/PYGRASSREAL/PyGrassReal-Showcase/releases/latest)** *(Latest build available in Releases)*
* **Installation Steps:**
  1. Download and run `pygrassreal-windows-setup.exe`.
  2. Follow the NSIS setup wizard to choose your installation directory.
  3. Launch **PyGrassReal** from the desktop shortcut and start creating!

---

### 2. 🌐 Web Cloud Platform
Instant access from modern web browsers without local installation:
* 🔗 Access online at: **[https://pygrassreal.ai](https://pygrassreal.ai)**
* Compatible with Chrome, Edge, Safari, and Firefox.

---

### 3. ⌨️ PGR CLI (Command-Line Interface)
Developer-friendly CLI tool to synchronize parameters, project assets, and cloud pipelines:
```bash
# Install globally via npm
npm install -g pgr-cli

# Login and initialize workspace
pgr_bin login
pgr_bin init
pgr_bin publish
```

---

### 4. 🧩 PyGrassReal Studio (VSCode Extension)
Connect your Python scripts and Grasshopper definitions directly to PyGrassReal:
* Search for **`PyGrassReal Studio`** in the VSCode Extension Marketplace.
* Or install the standalone `.vsix` from Releases.

---

### 5. 📱 Mobile Application (iOS & Android)
Monitor 3D projects and review design assets on the go:
* **Android:** Download `.apk` installer from GitHub Releases or Google Play.
* **iOS:** Available via Apple TestFlight / App Store.

---

## 🔑 Official API Cloud & Pay-As-You-Go Pricing

PyGrassReal provides high-performance API access to its AI Reasoning Team and Computational Geometry Engine via **OpenAI-compatible endpoints (`https://api.pygrassreal.ai/v1`)**. Transparent Pay-As-You-Go pricing based on verified token and compute metrics:

### 📊 Official Model Pricing Table

| Client Model String | Core Specialization & Capability | Input Price / 1M Tokens | Output Price / 1M Tokens | Unit Cost |
| :--- | :--- | :---: | :---: | :---: |
| **`pygrassreal/phralak1.5`** | **Geometry Code Engine:** Generates 3D CAD scripts, Python, Rhino & Grasshopper | **$0.35** | **$1.50** | — |
| **`pygrassreal/hanuman1.5`** | **Domain Knowledge RAG:** Architectural standards, building codes & CAD API docs | **$0.35** | **$1.50** | — |
| **`pygrassreal/sampati1`** | **Real-Time Web Search:** Live market materials, supplier pricing & web grounding | **$0.35** | **$1.50** | + Search fee |
| **`pygrassreal/sida1.5`** | **AI Concept Rendering:** Architectural perspective generation & material textures | **$0.71** | **$4.29** | $85.71 / 1M img tokens (~$0.04/img) |
| **`pygrassreal/matchanu1.5`** | **3D Generation:** Prompt-to-3D Mesh & Gaussian Splat generation | — | — | **$0.07143** / Model |
| **`pygrassreal/sadayu1.5`** | **Cinematic Video:** Architectural camera walkthrough animation | **$0.36** | **$2.14** | **$0.04286** / sec (720p), **$0.07143** / sec (1080p) |

### ⚡ OpenAI-Compatible Quickstart

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
        {"role": "user", "content": "Generate a Python function to compute UV coordinates for a double-curved facade."}
    ]
)

print(response.choices[0].message.content)
```

```bash
# cURL Example
curl https://api.pygrassreal.ai/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer pgr_live_your_api_key_here" \
  -d '{
    "model": "pygrassreal/phralak1.5",
    "messages": [
      {"role": "user", "content": "Generate a 3D structural beam calculation script in Python"}
    ]
  }'
```

> 💳 **Manage API Keys & Wallet Balance:** [PyGrassReal Developer Console](https://api.pygrassreal.ai)

---

## 💼 Target Audience & Enterprise Use Cases

* 🏛️ **Architects & Computational Designers**: Rapidly iterate complex 3D facades and structural forms with AI assistance.
* 🏗️ **Structural & BIM Engineers**: Automate structural loads, solar analysis, and geometric rule verification.
* 🎓 **Software Developers & Researchers**: Integrate geometry generation into custom pipelines via Python SDK, CLI, and Edge APIs.

---

## 📜 License & Terms of Service
* **Software Ownership:** PyGrassReal software, AI agent architectures, and cloud APIs are **Commercial & Proprietary Software**. All rights reserved by PyGrassReal.
* **Permitted Use:** Licensed for official downloads and authenticated API access according to subscribed usage tiers.
* **Restrictions:** Reverse engineering, decompiling, reselling, or unauthorized commercial reproduction is strictly prohibited.

---

## 🔒 Security & Enterprise Infrastructure
* **End-to-End Encryption:** All project data and model assets are encrypted via TLS 1.3 in transit and AES-256 at rest.
* **Enterprise Identity & Access Control:** Enterprise-grade authentication and strict Row-Level Security (RLS) policies.
* **Global High-Availability Network:** Distributed globally with automated load balancing and 99.9% uptime SLA.

---

## 📞 Contact & Enterprise Inquiries
For custom enterprise deployments, dedicated model hosting, or partnership opportunities:
* 🌐 **Website:** [https://pygrassreal.ai](https://pygrassreal.ai)
* 📧 **Email:** [admin@pygrassreal.ai](mailto:admin@pygrassreal.ai)
