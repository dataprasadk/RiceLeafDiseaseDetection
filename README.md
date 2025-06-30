# Rice Leaf Disease Detection using Deep Learning

This project presents a deep learning-based solution for classifying rice leaf diseases into three categories using image data. The model leverages Convolutional Neural Networks (CNNs) and Transfer Learning (MobileNetV2, VGG16, ResNet50, EfficientNetB0) with fine-tuning to achieve production-level performance. The pipeline is designed to be scalable, reproducible, and ready for real-world deployment.

## 🧠 Problem Statement

Manual identification of rice leaf diseases is time-consuming, error-prone, and labor-intensive. Automating this process using computer vision can significantly assist farmers and agronomists in early detection and timely treatment.

This project aims to build a classification model that can accurately identify:
- Bacterial Leaf Blight
- Brown Spot
- Leaf Smut

## 📁 Project Structure

```
RiceLeafDiseaseDetection/
│
├── RiceLeaf_Project/                # Jupyter Notebooks
├── README.md
├── requirements.txt
└── .gitignore
```

## 🚀 Technologies Used

- Python 3.10+
- TensorFlow / Keras
- OpenCV
- NumPy / Pandas
- Matplotlib / Seaborn
- Scikit-learn

## 📊 Models Evaluated

| Model                   | Accuracy | Precision | Recall | F1-Score |
|-------------------------|----------|-----------|--------|----------|
| MobileNetV2 (Fine-Tuned)| 0.8333   | 0.8500    | 0.8333 | 0.8312   |
| MobileNetV2             | 0.7222   | 0.7349    | 0.7222 | 0.7253   |
| VGG16                   | 0.6111   | 0.5972    | 0.6111 | 0.5937   |
| ResNet50                | 0.3333   | 0.1111    | 0.3333 | 0.1667   |
| EfficientNetB0          | 0.3333   | 0.1111    | 0.3333 | 0.1667   |
| Custom CNN              | 0.3333   | 0.1111    | 0.3333 | 0.1667   |

> **Best Model**: Fine-Tuned MobileNetV2  
> **F1-Score**: 0.8312

## 📌 Key Features

- Reproducible pipeline with seed control
- Transfer learning with fine-tuning
- Augmentation and class-balanced split
- Exported in both `.h5` and TensorFlow SavedModel format
- Supports external image predictions

## 🛠️ How to Use

```bash
# Clone the repository
git clone https://github.com/<your-username>/RiceLeafDiseaseDetection.git
cd RiceLeafDiseaseDetection

# Create virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook
```

## 📈 Future Improvements

- Deployment as web/mobile app
- Grad-CAM based explainability
- Vision Transformer integration
- Multi-disease support across crops

## 🙋‍♂️ Author

**Prasad Kamble** 
