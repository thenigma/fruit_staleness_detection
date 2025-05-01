# 🍌🍅 Fruit Freshness Classification using MobileNetV2

This project uses deep learning and transfer learning (MobileNetV2) to classify **bananas** and **tomatoes** into freshness levels: **Raw**, **Fresh**, and **Stale**. The goal is to help reduce food wastage by identifying the edibility stage of fruits using image-based classification.

---

## 🔍 Problem Statement

Fruits like bananas and tomatoes go through visible ripening and spoiling stages. This project builds a lightweight classification system that automates freshness detection from images, helping with early sorting and reducing food waste.

---

## 📁 Project Modules

1. **Fruit Type Prediction**  
   Classifies an image as either a *Banana* or a *Tomato*.

2. **Banana Freshness Classification**  
   Labels banana images as: `Raw`, `Fresh`, or `Stale`.

3. **Tomato Freshness Classification**  
   Labels tomato images as: `Raw`, `Fresh`, or `Stale`.

4. **Combined Classification System**  
   First detects fruit type, then applies the relevant freshness model, and outputs a final label (e.g., `Fresh Banana`, `Stale Tomato`).

---

## 🧠 Model Information

- **Base Model**: MobileNetV2 (pre-trained on ImageNet)
- **Framework**: TensorFlow / Keras
- **Input Image Size**: 224x224
- **Dataset**: Manually captured smartphone images, divided into 6 classes:

| Category            | Images |
|---------------------|--------|
| Raw Banana          | 37     |
| Fresh Banana        | 37     |
| Stale Banana        | 37     |
| Raw Tomato          | 37     |
| Fresh Tomato        | 37     |
| Stale Tomato        | 37     |

> Each class is split into **25 training**, **7 validation**, and **5 test** images.

---

## 🚀 How to Run

1. **Clone the repository:**

```bash
git clone https://github.com/your-username/fruit-freshness-classification.git
cd fruit-freshness-classification
```

2. Install dependencies
   
```bash
   pip install -r requirements.txt
```

3. Run prediction on an image:
   
```bash
   python predict_combined.py --image path_to_your_image.jpg
```

| Model                  | Accuracy |
|------------------------|----------|
| Fruit Type Classifier  | 100%     |
| Banana Freshness       | 93.33%   |
| Tomato Freshness       | 93.33%   |
| Combined Classifier    | 93%      |

##🧪 Future Improvements
- Add more real-world, varied images
- Train on larger datasets
- Extend to more fruits/vegetables
- Deploy as a mobile or web application
- Enable real-time classification from camera

##👤 Author
**Ved Patil**

📧 [vedpatil5303@gmail.com](mailto:vedpatil5303@gmail.com)
