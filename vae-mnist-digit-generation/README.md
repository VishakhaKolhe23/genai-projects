# 🧠 VAE for Handwritten Digit Generation

## 📌 Project Overview

This project implements a **Variational Autoencoder (VAE)** using PyTorch to learn the distribution of handwritten digits and generate new digit images.

The model is trained on the MNIST dataset and demonstrates:

* Image reconstruction
* Latent space learning
* New image generation

---

## 🚀 Features

* Encoder-Decoder architecture
* Reparameterization trick
* Reconstruction of input images
* Generation of new handwritten digits

---

## 🧠 What is a VAE?

A **Variational Autoencoder (VAE)** is a generative model that learns the underlying probability distribution of data.

Unlike traditional autoencoders:

* It learns **mean (μ)** and **variance (σ²)**
* It generates **new data samples**, not just reconstruction

---

## ⚙️ How It Works

1. **Encoder**

   * Converts input image into:

     * Mean (μ)
     * Log Variance (log σ²)

2. **Reparameterization Trick**

   * Samples latent vector:

     * z = μ + ε * σ

3. **Decoder**

   * Converts latent vector back to image

4. **Loss Function**

   * Reconstruction Loss (BCE)
   * KL Divergence (regularization)

---

## 📊 Results

### ✅ Reconstruction

* The model successfully reconstructs input images
* Reconstructed images are slightly blurred due to probabilistic nature

### 🎨 Generation

* New handwritten digits are generated from random latent vectors
* Generated digits resemble real digits but may be slightly noisy

---

## 🔍 Observations

* The model learns meaningful representations in latent space
* Increasing epochs improves clarity of generated digits
* Blurriness occurs due to averaging effect in probabilistic decoding

---

## 🛠 Tech Stack

* Python
* PyTorch
* NumPy
* Matplotlib

---

## 📷 Output

* Top Row → Input Images
* Middle Row → Reconstructed Images
* Bottom Row → Newly Generated Images

<img width="1725" height="601" alt="image" src="https://github.com/user-attachments/assets/7145f7c2-22b5-49d4-bd42-dc28cffb4526" />


---

## 📚 Learning Outcome

* Understood how generative models work
* Learned latent space representation
* Implemented VAE from scratch in PyTorch

---

## ▶️ How to Run

```bash
pip install torch torchvision matplotlib numpy
```

Run the notebook in Google Colab or Jupyter Notebook.

---

## 🔗 Future Improvements

* Train for more epochs
* Use convolutional VAE (ConvVAE)
* Improve image sharpness

---

## 👩‍💻 Author

Vishakha Kolhe
