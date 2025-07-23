# 🚗 Carvana Semantic Segmentation with U-Net

This repository contains a solution for performing **semantic segmentation** on car images using the U-Net architecture. The project is inspired by the [Carvana Image Masking Challenge](https://www.kaggle.com/competitions/carvana-image-masking-challenge) hosted by Kaggle.

---

## 🧠 Problem Statement

The objective is to segment the car from the background in high-resolution images. This is a pixel-level classification problem, where the model must learn to differentiate car pixels from the non-car background.

---

## 📁 Dataset

- High-resolution car images
- Corresponding binary masks (car vs background)

The data is typically structured as:
```
├── train/
│   ├── image1.jpg
│   ├── image2.jpg
├── masks/
│   ├── image1_mask.gif
│   ├── image2_mask.gif
```

---

## 🛠️ Model

We use the **U-Net architecture**, which is highly effective for biomedical and general-purpose segmentation tasks.

### Model Highlights:
- Contracting path for encoding spatial features
- Expanding path for upsampling and fine-grained segmentation
- Skip connections for preserving spatial information

---

## 📊 Evaluation Metric

- **Dice Coefficient (F1 Score for Segmentation)**  
Used to evaluate the overlap between predicted and ground truth masks:
```
Dice = (2 * |A ∩ B|) / (|A| + |B|)
```

---

## 🔧 Requirements

- Python ≥ 3.7
- NumPy
- PyTorch
- OpenCV / PIL
- Matplotlib
- tqdm

Install dependencies using:

```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. Clone the repo:
```bash
git clone https://github.com/Doaa-Helal/carvana-unet.git
cd carvana-unet
```

2. Run the notebook:
```bash
jupyter notebook caravana-semantic-segmentation-with-unet.ipynb
```

---

## 📌 Results

- Achieved a high dice score after training on the Carvana dataset
- Effective segmentation even in complex backgrounds

---

## 🤝 Contributors

- [Doaa Helal](https://github.com/Doaa-Helal)
- Feel free to open pull requests or suggest improvements!

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
