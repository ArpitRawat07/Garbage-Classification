# Garbage-Classification
Here’s a concise and informative GitHub repository description and README section for your project:

---

## 🗑️ Waste Classification using EfficientNetB7

This project is an end-to-end image classification system that leverages TensorFlow and EfficientNetB7 from TensorFlow Hub to classify images of various types of waste. It combines **general trash types** (like plastic, metal, glass, etc.) and **e-waste** (like batteries, keyboards, mobile phones, etc.) for improved waste segregation and recycling automation.

### 📂 Datasets Used

* [Trash Type Image Dataset](https://www.kaggle.com/datasets/farzadnekouei/trash-type-image-dataset)
* [E-Waste Image Dataset](https://www.kaggle.com/datasets/akshat103/e-waste-image-dataset)

Both datasets were preprocessed, cleaned, and merged into a unified training and testing set.

### ✅ Features

* Utilizes **EfficientNetB7** (pre-trained) as a feature extractor for high accuracy with low training cost.
* Multi-class classification of 16 waste categories.
* Uses **TensorFlow Hub** and **ImageDataGenerator** for streamlined image preprocessing.
* Model saving/loading and custom image prediction with visualization.
* TensorBoard integration for training monitoring.

### 🧠 Classes

* E-waste: Battery, Keyboard, Microwave, Mobile, Mouse, PCB, Player, Printer, Television, Washing Machine
* Trash: Cardboard, Glass, Metal, Paper, Plastic, Trash

### 📈 Training

* Images resized to `256x256`
* Batch size: `32`
* Loss: `categorical_crossentropy`
* Optimizer: `Adam`
* Accuracy and loss tracked on validation set
* Training logs available via TensorBoard

### 🖼️ Prediction & Visualization

You can load and predict on custom images using the `pred_and_plot` function.
Example:

```python
pred_and_plot(loaded_model, "path_to_image.jpg", class_names)
```

### 💾 Model

The trained model is saved as:

```
updated_efficientnet_model.h5
```

---

Let me know if you’d like me to generate a full `README.md` file with setup instructions, usage examples, and model performance metrics.
