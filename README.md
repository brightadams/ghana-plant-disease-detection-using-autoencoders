## Transfer Learning for Ghanaian Crop Disease Detection: A Comparative Study of Autoencoder and ResNet
**This project was undertaken as part of a Machine Learning course at Dalhousie University.**

This repository explores the feasibility of using deep learning models for crop disease detection on mobile devices. The project compares the training performance of an autoencoder-based model and a ResNet model, considering factors crucial for mobile deployment:

**Model Size and Complexity:** Autoencoders are generally smaller and require less processing power compared to complex models like ResNet. This makes them potentially better suited for resource-constrained mobile devices.

**Real-world Considerations:** The study goes beyond model performance to consider the practical implications of model size and computational cost for real-world deployment on mobile devices.

**Research Question:**

How does the performance of an autoencoder-based model compare to a ResNet model for crop disease detection on mobile devices, considering factors such as model size and computational cost?

## Methodology

**Data:**

* Utilize a global dataset [PlantVillage](https://www.kaggle.com/code/vad13irt/plant-disease-classification/input) and a [Ghana-specific](https://www.kaggle.com/datasets/ohagwucollinspatrick/ghana-crop-disease) dataset of crop images.
* Preprocess images using techniques like resizing, normalization, and augmentation.

**Autoencoder:**

1. Train an autoencoder on the global dataset to learn meaningful features.
2. Extract the encoder part and use it as a feature extractor.
3. Train a classifier on the extracted features using the Ghana dataset.

**ResNet:**

Train a ResNet model directly on the Ghana dataset.

## Results

The autoencoder-based model significantly outperformed the ResNet model on the Ghana dataset during training as we run the models several times and had the same outcome. This can be attributed to the effectiveness of the autoencoder in learning robust features from the global dataset, which can be transferred to the specific task of Ghanaian crop disease detection.



## Conclusions

This study demonstrates the potential of autoencoder-based feature extraction for improving crop disease detection in Ghana. By using the knowledge gained from a large-scale global dataset, we can effectively address the challenges of limited data and computational resources in developing countries.
