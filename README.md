# 🩺 Medical Document Q&A System

A prototype for extracting structured data from medical forms and answering questions based on the extracted content.

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Gradio](https://img.shields.io/badge/UI-Gradio-orange)

---

## 📌 Project Overview

This project was developed to address the **manual burden of extracting information from medical documents**. In real-world clinical environments, healthcare providers deal with large volumes of patient forms. The goal is to **automate information extraction and enable Q&A interaction with medical forms**, making workflows more efficient.

---

## 🎯 Objective

- Take an **image of a medical form**
- Extract structured data using OCR and layout detection
- Let users **ask questions** based on the document
- Return the **answer** visually and textually

---
> ⚠️ **Diagram Rendering Notice**: GitHub doesn't support Mermaid diagrams by default. Use [VSCode Mermaid Preview](https://marketplace.visualstudio.com/items?itemName=vstirbu.vscode-mermaid-preview) or compatible tools to render.

```mermaid
graph TD
  A[User Uploads Medical Form Image] --> B[Image Preprocessing]
  B --> C[Layout Detection (YOLO)]
  C --> D[OCR Text Extraction (Tesseract]
  D --> E[Convert to Structured Format (Regex/Pandas)]
  E --> F[Q&A Model (HuggingFace Transformers)]
  F --> G[Frontend Display (Gradio)]

