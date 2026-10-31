# CV-porject-# CIFAR-10 Image Classification — End-to-End Computer Vision Project

## 1. Problem Statement
Automatically classify small colour images into 10 categories (airplane, automobile,
bird, cat, deer, dog, frog, horse, ship, truck). Image classification is the base of
applications such as object recognition, content moderation and visual search.

## 2. Dataset
CIFAR-10: 60,000 colour images of 32×32 pixels (50,000 train, 10,000 test), 6,000 per class.# CIFAR-10 Image Classification — End-to-End Computer Vision Project

## 1. Problem Statement
Automatically classify small colour images into 10 categories (airplane, automobile,
bird, cat, deer, dog, frog, horse, ship, truck). Image classification is the base of
applications such as object recognition, content moderation and visual search.

## 2. Dataset
CIFAR-10: 60,000 colour images of 32×32 pixels (50,000 train, 10,000 test), 6,000 per class.
Downloaded automatically through `tf.keras.datasets`.

## 3. Pipeline
1. **Data loading** – CIFAR-10 train/test split; 10% of train used for validation.
2. **Preprocessing** – pixel values scaled to [0, 1].
3. **Augmentation** – random horizontal flip, rotation and zoom (reduces overfitting).
4. **Model** – CNN with 3 blocks (2×Conv + BatchNorm + MaxPool + Dropout), then Dense(256) + Dropout(0.5) + Softmax.
5. **Training** – Adam optimizer, sparse categorical cross-entropy, EarlyStopping and ReduceLROnPlateau.
6. **Evaluation** – accuracy, loss curves, precision/recall/F1 per class, confusion matrix.
7. **Deployment** – Streamlit web app for uploading an image and getting a prediction.

## 4. How to Run
```bash
pip install -r requirements.txt
python train.py          # trains, evaluates, saves cifar10_cnn.keras + plots in outputs/
streamlit run app.py     # launches the web app
```

## 5. Results
- Test accuracy: ___
- Training curves: `outputs/training_curves.png`
- Confusion matrix: `outputs/confusion_matrix.png`
- Classification report: `outputs/classification_report.txt`

## 6. Observations
- Classes like cat/dog and automobile/truck are most often confused because of visual similarity.
- Augmentation, BatchNorm and Dropout reduced the gap between training and validation accuracy.

## 7. Limitations & Future Work
- Images are only 32×32; higher resolution would help.
- Transfer learning (e.g. MobileNetV2, ResNet50) could raise accuracy above 90%.
- Could be extended to object detection (YOLO) or deployed via FastAPI/Docker.

## 8. Project Structure
```
cv_project/
├── train.py            # full training + evaluation pipeline
├── app.py              # Streamlit deployment app
├── requirements.txt
├── README.md           # project report
└── outputs/            # plots & reports (generated)
```# CIFAR-10 Image Classification — End-to-End Computer Vision Project

## 1. Problem Statement
Automatically classify small colour images into 10 categories (airplane, automobile,
bird, cat, deer, dog, frog, horse, ship, truck). Image classification is the base of
applications such as object recognition, content moderation and visual search.

## 2. Dataset
CIFAR-10: 60,000 colour images of 32×32 pixels (50,000 train, 10,000 test), 6,000 per class.
Downloaded automatically through `tf.keras.datasets`.

## 3. Pipeline
1. **Data loading** – CIFAR-10 train/test split; 10% of train used for validation.
2. **Preprocessing** – pixel values scaled to [0, 1].
3. **Augmentation** – random horizontal flip, rotation and zoom (reduces overfitting).
4. **Model** – CNN with 3 blocks (2×Conv + BatchNorm + MaxPool + Dropout), then Dense(256) + Dropout(0.5) + Softmax.
5. **Training** – Adam optimizer, sparse categorical cross-entropy, EarlyStopping and ReduceLROnPlateau.
6. **Evaluation** – accuracy, loss curves, precision/recall/F1 per class, confusion matrix.
7. **Deployment** – Streamlit web app for uploading an image and getting a prediction.

## 4. How to Run
```bash
pip install -r requirements.txt
python train.py          # trains, evaluates, saves cifar10_cnn.keras + plots in outputs/
streamlit run app.py     # launches the web app
```

## 5. Results
- Test accuracy: ___
- Training curves: `outputs/training_curves.png`
- Confusion matrix: `outputs/confusion_matrix.png`
- Classification report: `outputs/classification_report.txt`

## 6. Observations
- Classes like cat/dog and automobile/truck are most often confused because of visual similarity.
- Augmentation, BatchNorm and Dropout reduced the gap between training and validation accuracy.

## 7. Limitations & Future Work
- Images are only 32×32; higher resolution would help.
- Transfer learning (e.g. MobileNetV2, ResNet50) could raise accuracy above 90%.
- Could be extended to object detection (YOLO) or deployed via FastAPI/Docker.

## 8. Project Structure
```
cv_project/
├── train.py            # full training + evaluation pipeline
├── app.py              # Streamlit deployment app
├── requirements.txt
├── README.md           # project report
└── outputs/            # plots & reports (generated)
```

Downloaded automatically through `tf.keras.datasets`.

## 3. Pipeline
1. **Data loading** – CIFAR-10 train/test split; 10% of train used for validation.
2. **Preprocessing** – pixel values scaled to [0, 1].
3. **Augmentation** – random horizontal flip, rotation and zoom (reduces overfitting).
4. **Model** – CNN with 3 blocks (2×Conv + BatchNorm + MaxPool + Dropout), then Dense(256) + Dropout(0.5) + Softmax.
5. **Training** – Adam optimizer, sparse categorical cross-entropy, EarlyStopping and ReduceLROnPlateau.
6. **Evaluation** – accuracy, loss curves, precision/recall/F1 per class, confusion matrix.
7. **Deployment** – Streamlit web app for uploading an image and getting a prediction.

## 4. How to Run
```bash
pip install -r requirements.txt
python train.py          # trains, evaluates, saves cifar10_cnn.keras + plots in outputs/
streamlit run app.py     # launches the web app
```

## 5. Results
- Test accuracy: ___
- Training curves: `outputs/training_curves.png`
- Confusion matrix: `outputs/confusion_matrix.png`
- Classification report: `outputs/classification_report.txt`

## 6. Observations
- Classes like cat/dog and automobile/truck are most often confused because of visual similarity.
- Augmentation, BatchNorm and Dropout reduced the gap between training and validation accuracy.

## 7. Limitations & Future Work
- Images are only 32×32; higher resolution would help.
- Transfer learning (e.g. MobileNetV2, ResNet50) could raise accuracy above 90%.
- Could be extended to object detection (YOLO) or deployed via FastAPI/Docker.

## 8. Project Structure
```
cv_project/
├── train.py            # full training + evaluation pipeline
├── app.py              # Streamlit deployment app
├── requirements.txt
├── README.md           # project report
└── outputs/            # plots & reports (generated)
```
