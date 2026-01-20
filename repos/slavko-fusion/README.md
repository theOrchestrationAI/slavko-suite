<p align="center">
  <img src="https://img.shields.io/badge/🔗-SlavkoFusion%201.0-9333ea?style=for-the-badge" />
</p>

<h1 align="center">🔗 SlavkoFusion 1.0</h1>

<p align="center">
  <strong>Multimodal Integration Layer</strong><br/>
  <em>Unified Feature Extraction for Text, Image, PDF & Code</em>
</p>

<p align="center">
  <a href="https://github.com/theOrchestrationAI/slavko-fusion/releases"><img src="https://img.shields.io/badge/version-1.0.0-00ff88?style=for-the-badge" alt="Version" /></a>
  <a href="https://ollama.com/mladen-gertner/slavkofusion-v1"><img src="https://img.shields.io/badge/Ollama-mladen--gertner-white?style=for-the-badge&logo=ollama" alt="Ollama" /></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-Apache%202.0-blue?style=for-the-badge" alt="License" /></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/🇭🇷-Made%20in%20Zagreb-000?style=for-the-badge" />
  <img src="https://img.shields.io/badge/👁️-Vision%20Enabled-f59e0b?style=for-the-badge" />
</p>

---

## 🎯 Overview

**SlavkoFusion 1.0** is the multimodal integration layer of the S.L.A.V.K.O.™ orchestration system. It unifies feature extraction across text, images, documents, and code into a consistent output schema for downstream processing.

---

## 🚀 Quick Start

```bash
# Run with Ollama (Vision Model)
ollama run mladen-gertner/slavkofusion-v1

# Process Image
curl -X POST http://localhost:11434/api/generate \
  -d '{
    "model": "mladen-gertner/slavkofusion-v1",
    "prompt": "Extract features from this document",
    "images": ["base64_encoded_image"]
  }'
```

---

## 🎨 Supported Modalities

| Modality | Formats | Capabilities |
|----------|---------|--------------|
| **Text** | plain, markdown, html | Semantic extraction |
| **Image** | png, jpeg, webp | OCR, object detection |
| **Document** | pdf, docx | Layout analysis |
| **Code** | all languages | AST parsing |
| **UI Mockup** | Figma, Sketch | Component detection |

---

## 🔬 Features Extracted

```json
{
  "modality": "text|image|document|code|mixed",
  "extraction": {
    "raw_text": "...",
    "structured_content": {},
    "entities": []
  },
  "features": {
    "semantic_embedding": [],
    "keywords": [],
    "topics": [],
    "complexity_score": 0.0-1.0
  },
  "vision": {
    "objects_detected": [],
    "text_extracted": "",
    "layout_analysis": {}
  },
  "code": {
    "language": "...",
    "ast_summary": {},
    "dependencies": []
  }
}
```

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────┐
│           SLAVKOFUSION 1.0              │
│      Multimodal Integration Layer       │
└─────────────────────────────────────────┘
              │
    ┌─────────┼─────────┐
    ▼         ▼         ▼
┌───────┐ ┌───────┐ ┌───────┐
│ Text  │ │Vision │ │ Code  │
│Extract│ │Extract│ │Extract│
└───────┘ └───────┘ └───────┘
    │         │         │
    └─────────┼─────────┘
              ▼
      ┌─────────────┐
      │  Unified    │
      │  Features   │
      └─────────────┘
```

---

## 📞 Contact

**Mladen Gertner** — FormatDisc™, Zagreb, Croatia  
📧 mladen@formatdisc.hr | 🌐 [formatdisc.hr](https://formatdisc.hr)

---

<p align="center">
  <sub>© 2026 FormatDisc™, vl. Mladen Gertner — All Rights Reserved</sub>
</p>
