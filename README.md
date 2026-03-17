# ♻️ Smart Waste Segregation System (Vishudh)

An AI-powered smart waste segregation system that classifies waste into categories and automates sorting using computer vision and embedded systems.

---

## 🚀 Overview

This project combines **Machine Learning + IoT + Automation** to detect and segregate waste into categories like:

* 🟢 Organic
* 🔵 Recyclable
* 🔴 Hazardous

The system uses a trained deep learning model for classification and integrates with hardware (Raspberry Pi, motors, servo) to physically sort waste.

---

## 🧠 Key Features

* ✅ Image-based waste classification using deep learning
* ✅ Lightweight **TFLite model (INT8 quantized)** for edge deployment
* ✅ Real-time inference on CPU (no GPU required)
* ✅ Automated sorting using conveyor + servo mechanism
* ✅ Incremental model training support
* ✅ Dataset analysis and balancing utilities

---

## 🏗️ System Architecture

1. Capture waste image
2. Run ML model inference
3. Predict waste category
4. Trigger hardware (servo + conveyor)
5. Sort waste into correct bin

---

## 🧪 Model Training

Train the model using:

```bash
python 3_class_train.py
```

* Uses **MobileNetV2 (Transfer Learning)**
* CPU-optimized training
* Outputs:

  * `.keras` model
  * `.tflite` quantized model

📄 Reference: 

---

## 🔁 Model Update (Incremental Learning)

Update model with new data:

```bash
python update_model.py
```

* Fine-tunes existing model
* Prevents retraining from scratch
* Uses low learning rate + early stopping

📄 Reference: 

---

## 🔍 Model Testing (Inference)

Run prediction on an image:

```bash
python 3_class_test.py
```

* Uses **TFLite INT8 model**
* CPU-efficient inference
* Outputs predicted class + confidence

📄 Reference: 

---

## 📊 Dataset Analysis

Check dataset distribution:

```bash
python check_balance.py
```

📄 Reference: 

---

## 🤖 Hardware Integration (Raspberry Pi)

Run the smart sorting system:

```bash
python rasp_file_1.py
```

### Components Used:

* Raspberry Pi
* Servo Motor
* Conveyor Motor
* Camera Module

### Functionality:

* Captures live image
* Classifies waste
* Moves servo to correct bin
* Controls conveyor belt

📄 Reference: 

---

## ⚙️ Technologies Used

* Python
* TensorFlow / Keras
* TensorFlow Lite
* OpenCV
* ONNX Runtime
* Raspberry Pi GPIO

---

## 📈 Future Improvements

* Add more waste categories
* Improve model accuracy with larger dataset
* Deploy mobile app interface
* Real-time cloud monitoring dashboard
* Edge AI optimization for faster inference

---

## 🌍 Impact

This project contributes to:

* Smart cities 🌆
* Sustainable waste management ♻️
* Automation in environmental systems
