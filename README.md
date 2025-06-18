# 🎨 Painting Style Transfer using GAN

**Computer Vision | 6th Semester CSE**

**Group Members:**  
- Abhikalp Srivastava (B521002)
- Axa Gemini Lakra (B121010)  
- Shruti Swarupa Dhar (B121056)  

**Faculty Advisor:** Mr. Sarthak Padhi  
**IIIT Bhubaneswar** • **April 2024**

---

## 🚀 Project Overview

This repository implements **CycleGAN**‑based painting style transfer, transforming your photographs into Monet‑style masterpieces and back again. Leveraging unpaired image‑to‑image translation, our model learns style mappings without requiring exact photo–painting pairs.

---

## 🔍 Key Features

- **Dual Generators & Discriminators:**  
  - Photo → Monet and Monet → Photo translation  
  - Adversarial feedback for realistic, high‑fidelity outputs

- **Cycle‑Consistency & Identity Loss:**  
  - Enforce content preservation  
  - Prevent mode collapse

- **Quantitative Metrics:**  
  - PSNR & SSIM evaluations  
  - Generator & discriminator loss tracking

---

## 🛠️ Getting Started

### 1. Clone the Repo
```bash
git clone https://github.com/<username>/painting-style-transfer-gan.git
cd painting-style-transfer-gan
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Prepare Data
- Download the `monet2photo` dataset from Kaggle
- Place `trainA/`, `trainB/`, `testA/`, `testB/` folders under `data/`

### 4. Train the Model
```bash
python train.py \
  --epochs 30 \
  --batch_size 1 \
  --lr 2e-4 \
  --lambda_cycle 10 \
  --beta1 0.5
```

### 5. Evaluate & Visualize
```bash
python evaluate.py --data_dir data/testA --output_dir results/
```

---

## 📊 Results & Samples

**Photo → Monet-style**

**Monet-style → Photo**

---

## 📂 Attachments
- Project Report: `docs/Painting_Style_Transfer_Report.pdf`
- Presentation Slides: `docs/Painting_Style_Transfer_Presentation.pptx`

**Completed: April 19, 2024**

---

## 🤝 Contributing
1. Fork the repo  
2. Create a feature branch (`git checkout -b feature/XYZ`)  
3. Commit your changes (`git commit -m "Add XYZ"`)  
4. Push to your branch (`git push origin feature/XYZ`)  
5. Open a Pull Request

---

## 📜 License
This project is released under the MIT License. See `LICENSE` for details.

---
