# Dog Breed Recognition using Deep Learning

Final Year Project (BSc Cognitive Science, UNIMAS). A large benchmarking study that
trains and compares **multiple Convolutional Neural Network (CNN) architectures** for
classifying dog breeds from images, and measures how **image cropping**, **learning
rate** and **dataset size** affect accuracy.

## 🧠 Architectures compared

- AlexNet
- VGG
- GoogLeNet
- InceptionV3
- Inception‑ResNet
- DenseNet
- MobileNet

## 🧪 Experiment design

Each architecture is trained under a grid of conditions (≈145 notebooks in total):

- **Image preprocessing** — `Crop Image Result/` (dogs cropped from the photo) vs
  `Not Crop Image Result/` (full original image), to test whether cropping to the
  subject improves recognition.
- **Learning rate** — `0.001` and `0.01`.
- **Dataset size** — `250`, `500`, `750` and `1000` images per run.

`split train and test set.txt` documents how the data was divided into training and
testing sets.

## 📁 Repository layout

```
Crop Image Result/        # experiments on cropped dog images
Not Crop Image Result/    # experiments on full/uncropped images
split train and test set.txt
```

Notebook names follow the pattern `<Model><LearningRate>(<ImageCount>).ipynb`,
e.g. `AADenseNet0.001(1000).ipynb` = DenseNet, LR 0.001, 1000 images.

## 🛠️ Tech

- Python · Jupyter Notebook
- Deep‑learning CNNs via transfer learning
- Trained locally and on Kaggle / Google Colab

## ▶️ How to run

1. Open any notebook in Jupyter, Google Colab or Kaggle.
2. Point the data loader at your dog‑breed image dataset.
3. Run the cells to train the chosen architecture and view its accuracy.

> See **[Enhancing Dog Breed Classification with Feature Fusion of Pre‑trained CNNs](https://github.com/LingSy12/Enhancing-Dog-Breed-Classification-with-Feature-Fusion-of-Pre-trained-CNNs-and-Machine-Learning)**
> for the follow‑up Master's project that fuses CNN features with classical classifiers.
