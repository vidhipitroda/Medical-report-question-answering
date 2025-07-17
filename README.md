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
1. 📤 User uploads a medical form image
2. 🧼 Image preprocessing (grayscale, contrast enhancement)
3. 🧭 Layout detection using  YOLO
4. 🔍 OCR text extraction using Tesseract
5. 🧾 Convert text into structured format
6. 🧠 Run Q&A model to find the answer to the user’s question
7. 🌐 Display result in Gradio interface with highlights

