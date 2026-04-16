# 🚀 InternVCC

> 🚗 OCR System for Vehicle Registration Certificates (Giấy chứng nhận đăng ký xe)

---

## 📌 Overview

**InternVCC** is an AI-powered OCR system designed to automatically extract information from **Vietnamese vehicle registration certificates**.

The system combines:

* 🔍 Object Detection (detect text regions)
* 🔤 OCR (text recognition)
* 🧠 Post-processing (format & normalize output)

👉 Goal:
Reduce manual data entry and improve accuracy in digitizing vehicle documents.

---

## 🧠 Key Features

* 📄 Detect key fields in vehicle registration documents
* 🔤 Recognize Vietnamese text using OCR models
* ⚡ End-to-end pipeline: Image → Structured Data (JSON)
* 📊 Evaluation with OCR metrics (CER, WER)
* 🧩 Modular architecture (easy to extend)

---

## 🔄 Pipeline

```mermaid id="8d9v4r"
flowchart LR
    A[Input Image] --> B[Preprocessing]
    B --> C[Text Detection (YOLO)]
    C --> D[Crop Text Regions]
    D --> E[Text Recognition (OCR)]
    E --> F[Post-processing]
    F --> G[Structured Output (JSON)]
```

---

## 📊 Evaluation Metrics

* **CER (Character Error Rate)**
* **WER (Word Error Rate)**
* **Precision / Recall (Detection)**
* **mAP (for detection model)**

---

## 📦 Dataset

* 📄 Vehicle Registration Certificate Images
* 🏷️ Annotation:

  * Bounding boxes (for detection)
  * Text labels (for OCR)

---

## 📈 Workflow

```id="y91lf4"
Data Collection → Annotation → Training → Evaluation → Inference → Deployment
```

---

## 📌 TODO

* [ ] Improve OCR accuracy for low-quality images
* [ ] Deploy API service
* [ ] Build web interface
* [ ] Optimize inference speed

---

## 🤝 Contributing

Contributions are welcome!

---

## 📄 License

MIT License

---

## 👤 Author

**Pham Hoang Long**

* 📧 [plongzoro@gmail.com](mailto:plongzoro@gmail.com)
* 💻 https://github.com/GolDDragon1702

---

## ⭐ Acknowledgements

* Open-source OCR & Detection communities
* Internship mentors
* Vietnamese document datasets

---
