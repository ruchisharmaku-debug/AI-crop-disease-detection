# 🥔 AI Potato Crop Disease Detection

An end-to-end Deep Learning web application built with **TensorFlow/Keras** and **Streamlit** to detect viral diseases in potato crops from leaf images. The entire model training and deployment pipeline runs seamlessly on **Google Colab** using a **Cloudflare Tunnel**.

---

## 🔗 Live Links
* **🌐 Live Streamlit Web App:** [Open App](https://george-riding-angeles-corporations.trycloudflare.com) *(Active while Google Colab runtime is running)*


---

## 📌 Overview
Viral infections in potato crops can severely reduce yield if not identified early. This project uses a Convolutional Neural Network (CNN) trained on leaf imagery (`nirmalsankalana/potato-viral-disease-dataset`) to classify potato leaves into four categories with confidence scores:
* `Potato___healthy`
* `Potato___leafroll_virus`
* `Potato___mosaic_virus`
* `Potato___spindle_tuber_viroid`

---

## 🛠️ Tech Stack
* **Deep Learning:** TensorFlow, Keras (CNN)
* **Data Processing & Visualization:** NumPy, Matplotlib, Pillow (PIL), KaggleHub
* **Web UI:** Streamlit
* **Cloud & Hosting:** Google Colab (T4 GPU), Cloudflare Tunnel (`cloudflared`)

---

## 📂 Repository Structure
* `Crop disease detection_model_pred.ipynb` — Complete Google Colab notebook containing dataset download, preprocessing, CNN model training, model serialization (`crop_disease_model.h5`), and Streamlit deployment commands.

---

## 🚀 How to Run on Google Colab
1. Open `Crop disease detection_model_pred.ipynb` in **Google Colab** (select **T4 GPU** runtime for faster training).
2. Run the dataset download (`kagglehub`), preprocessing, and model training cells.
3. Run the `model.save("crop_disease_model.h5")` cell to export the trained model.
4. Run the `%%writefile app.py` cell to generate the Streamlit web interface.
5. Run the `cloudflared` tunnel cell to generate a live public URL and upload a leaf image for instant disease prediction.

---

## 👩‍💻 Author
**Ruchi Sharma**  
GitHub: [@ruchisharmaku-debug](https://github.com/ruchisharmaku-debug)
