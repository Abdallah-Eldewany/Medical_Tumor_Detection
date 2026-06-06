# Brain Tumor Detection Application

This project is a Brain Tumor Detection system that uses MRI images to classify whether a brain tumor is present or not. The main goal was to create a deep learning model capable of accurate predictions, and to provide an interactive web interface for demonstration purposes.

---

## 📊 Dataset & Preprocessing

The dataset used is from Kaggle and contains labeled MRI images divided into two categories: **"Tumor"** and **"No Tumor"**.
* Images were preprocessed and resized to a uniform size of **150x150 pixels** to feed into the neural network.

---

## 🤖 Model Architecture & Training

For the model, I used **VGG16** pretrained on ImageNet as the base, freezing its layers to retain learned features. On top of this, I added custom layers including:
* Fully connected layer
* Dropout for regularization
* Final **sigmoid** layer for binary classification

The model was trained using **early stopping** to prevent overfitting and a **model checkpoint** to save the best-performing model automatically.

---

## 💻 Web Interface & Deployment

I also developed a **Streamlit-based** web interface that allows users to upload MRI images and get real-time predictions. 
To make the application accessible online, I integrated **ngrok**, which creates a secure tunnel to the local server so anyone with the link can interact with the interface.

---

## 🛠️ Tech Stack & Requirements

The project uses Python libraries including:
* **TensorFlow / Keras** for modeling
* **Streamlit** for the web interface
* **pyngrok** for temporary online access

This setup makes the system easy to run locally or share for demonstration purposes, while keeping sensitive information like the ngrok token secure.

---

## 💡 Summary

Overall, this project demonstrates end-to-end AI application development: from dataset preprocessing and model training to creating an accessible web interface with live predictions.
