# plant-disease-classification
This project uses YOLOv8 for image classification to identify various plant diseases across multiple crops. The model takes leaf images as input and classifies them into specific disease categories or healthy conditions.
🧪 Model Used
Model: YOLOv8 Classification (yolo classify)

Type: Image Classification (not object detection)

Framework: Ultralytics YOLOv8

🌿 Classes (15 Total)
The model was trained on a labeled dataset containing the following crop-disease combinations:

🌽 Corn:
Corn___Common_Rust

Corn___Gray_Leaf_Spot

Corn___Northern_Leaf_Blight

Corn___HealthyInvalid (you may want to rename this to just Corn___Healthy for clarity)

🥔 Potato:
Potato___Early_Blight

Potato___Late_Blight

Potato___Healthy

🌾 Rice:
Rice___Brown_Spot

Rice___Hispa

Rice___Leaf_Blast

Rice___Healthy

🌿 Wheat:
Wheat___Brown_Rust

Wheat___Yellow_Rust

Wheat___Healthy (looks like HealthyWheat might be a typo in your original list)

📸 Classification Workflow
Input: Leaf image (from corn, potato, rice, or wheat).

Preprocessing: Image resized to fit YOLOv8 input requirements.

Prediction: YOLOv8 assigns the image to one of the 15 class labels.

Output: Predicted class with confidence score.

🧠 Why YOLOv8 for Classification?
Although YOLO is known for object detection, Ultralytics' YOLOv8 also supports image classification tasks. It provides:

Fast training and inference

High accuracy on labeled image datasets

Easy switching between detection/classification/segmentation

✅ Example Prediction
Input Leaf Image	Predicted Class	Confidence
rice_leaf.jpg	Rice___Brown_Spot	94.6%
potato_leaf.jpg	Potato___Early_Blight	91.3%
