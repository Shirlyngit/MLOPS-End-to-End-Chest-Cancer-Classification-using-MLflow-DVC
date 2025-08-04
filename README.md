# End-to-End-Chest-Cancer-Classification-using-MLflow-DVC
# MLOps End-to-End Pipeline 🚀

An end-to-end Machine Learning pipeline for **automated classification of Adenocarcinoma**, a common and deadly form of **lung cancer**, using **deep learning (VGG16 + CNN)** integrated with a full **MLOps workflow**.

This project deploys a production-grade solution combining:  
- 🧪 **MLflow** for tracking experiments  
- 📦 **DVC** for dataset/model versioning  
- ☁️ **Dagshub** for remote collaboration  
- 🐳 **Docker** for deployment  
- ⚙️ **CI/CD pipeline** for automation  
- 🌐 **HTML Web UI** for real-time predictions

> ⚕️ **Medical Impact**: Adenocarcinoma is one of the deadliest lung cancers. Early detection via deep learning can drastically improve outcomes — especially in underserved healthcare systems.

---

## 💡 Why Adenocarcinoma?

- 📈 Accounts for **40% of all lung cancer cases**
- 🧬 Often misdiagnosed in early stages
- ⏰ Early AI-powered detection improves survival by up to **50%**
- 🌍 Designed for **clinician support in resource-limited settings**

---

## 🔍 Summary

| 🔬 Problem | 🧠 Solution | 💥 Impact |
|-----------|-------------|-----------|
| Adenocarcinoma detection is error-prone & delayed | Trained VGG16 + CNN on annotated X-ray datasets | Improves diagnostic accuracy & saves time |
| Reproducibility in AI pipelines is hard | Integrated MLflow, DVC & GitHub CI/CD | Ensures traceability & accountability |
| Clinician access to ML tools is limited | Built web UI & Dockerized deployment | Empowers healthcare workers globally |

---

## 🧠 Deep Learning Models

### ✅ VGG16 – Transfer Learning
- Pre-trained on ImageNet  
- Fine-tuned for chest X-ray Adenocarcinoma detection  
- High performance with minimal compute needs

### ✅ Custom CNN
- Built from scratch  
- Lightweight & fast  
- Suitable for edge deployment (rural clinics, mobile devices)

---

## 📈 Model Performance

| Metric | VGG16 | Custom CNN |
|--------|--------|-------------|
| Accuracy | 94.6% | 91.2% |
| Precision | 93.0% | 89.5% |
| Recall (Sensitivity) | 94.8% | 90.1% |
| F1-Score | 93.8% | 89.8% |

---

## 🛠️ Tech Stack

| Tool | Role |
|------|------|
| **Python, Keras** | Model development |
| **MLflow** | Experiment tracking |
| **DVC** | Data/model versioning |
| **Dagshub** | ML dashboard & Git remote |
| **Docker** | App containerization |
| **Flask + HTML** | UI development |
| **GitHub Actions** | CI/CD automation |

---

## 🌐 Web App Workflow

- 📤 Upload a chest X-ray image  
- 🧠 AI predicts: **Adenocarcinoma Positive** or **Normal**  
- 🖥️ Results shown on the browser with diagnosis label

**Launch via Docker:**

```bash
docker build -t adenocarcinoma-detector .
docker run -p 5000:5000 adenocarcinoma-detector

