# 🌿 Plant Disease Classification

This project uses **YOLOv8** for **image classification** to identify various plant diseases across multiple crops. The model takes **leaf images as input** and classifies them into specific disease categories or healthy conditions.

---

## 🧪 Model Used

- **Model**: YOLOv8 Classification (`yolo classify`)
- **Task**: Image Classification *(not object detection)*
- **Framework**: [Ultralytics YOLOv8](https://docs.ultralytics.com/)

---

## 🌱 Classes (15 Total)

The model was trained on a labeled dataset containing the following crop–disease combinations:

### 🌽 Corn
- `Corn___Common_Rust`
- `Corn___Gray_Leaf_Spot`
- `Corn___Northern_Leaf_Blight`
- `Corn___HealthyInvalid` *(recommend renaming to `Corn___Healthy` for clarity)*

### 🥔 Potato
- `Potato___Early_Blight`
- `Potato___Late_Blight`
- `Potato___Healthy`

### 🌾 Rice
- `Rice___Brown_Spot`
- `Rice___Hispa`
- `Rice___Leaf_Blast`
- `Rice___Healthy`

### 🌿 Wheat
- `Wheat___Brown_Rust`
- `Wheat___Yellow_Rust`
- `Wheat___Healthy` *(was previously listed as `HealthyWheat` — fixed)*

---

## 📸 Classification Workflow

1. **Input**: Leaf image (Corn, Potato, Rice, Wheat)
2. **Preprocessing**: Image resized to match YOLOv8 input size
3. **Prediction**: YOLOv8 classifies the image into one of 15 labels
4. **Output**: Class label + confidence score

---

## 🧠 Why YOLOv8 for Classification?

Although YOLO is widely known for object detection, the **Ultralytics YOLOv8** version also supports image classification. It offers:

- ⚡ Fast training & inference
- ✅ High accuracy on custom datasets
- 🔄 Easy switching between tasks (detection/classification/segmentation)

---

## 📊 Results

### 🔍 Confusion Matrix
![confusion_matrix](https://github.com/user-attachments/assets/b3074cae-28f6-4589-bfab-f5ce00003a7b)

### 🧮 Normalized Confusion Matrix
![confusion_matrix_normalized](https://github.com/user-attachments/assets/13b062b9-a40b-437f-b6eb-02e46e39818e)

---

## 🖼️ Training & Validation Samples

| Training Batch 0 | Training Batch 1 | Validation Predictions |
|------------------|------------------|-------------------------|
| ![train_batch0](https://github.com/user-attachments/assets/32682190-0495-4d13-9cb1-74f8b32f0514) | ![train_batch1](https://github.com/user-attachments/assets/85083044-071c-40ac-a9e6-662a440aca0d) | ![val_batch1_pred](https://github.com/user-attachments/assets/2e7a793b-ddfa-4b78-83b2-bca3bdccd4c4) |

---

## 🏁 Final Results Summary

![results](https://github.com/user-attachments/assets/dc228486-4003-4515-9927-9eac15adcecb)

---


