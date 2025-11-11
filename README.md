# 🧠 Deepfake Video Detection  

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)  
[![Framework](https://img.shields.io/badge/Framework-Django-green.svg)](https://www.djangoproject.com/)  
[![DeepLearning](https://img.shields.io/badge/Deep%20Learning-PyTorch-red.svg)](https://pytorch.org/)  
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  
[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://github.com/sadiyabhokare/Deepfake_Video_Detection/pulls)  

---

## 1. Introduction  
This project focuses on detecting **deepfake videos** using **Deep Learning** architectures such as **ResNeXt** and **LSTM**.  
The system leverages **transfer learning**, where a pretrained **ResNeXt CNN** extracts spatial features from video frames, and an **LSTM layer** models temporal dependencies to classify videos as *real* or *fake*.  

---

## 2. Directory Structure  
```

Deepfake_Video_Detection
├── Django Application
│     └── Web interface for uploading and predicting videos.
│
├── Model Creation
│     └── Scripts and notebooks for building and training
│         the ResNeXt + LSTM model.
│
├── Documentation
│     └── Reports, datasets, and analysis details.

````

### Components  
1. **Django Application**  
   - A web-based interface where users can upload videos for deepfake detection.  
   - The trained model runs on the backend and displays whether the video is *real* or *fake*.  

2. **Model Creation**  
   - Implements **ResNeXt** for high-level spatial feature extraction.  
   - Uses an **LSTM layer** to analyze sequential frame information.  
   - Trained and validated on a curated dataset of real and fake videos.  

3. **Documentation**  
   - Contains detailed reports, research insights, and experimental analyses.  

---

## 3. Tools & Technologies  
- **Python 3.10+**  
- **PyTorch** — Deep Learning framework for model development  
- **ResNeXt** — Pretrained CNN used for feature extraction  
- **LSTM** — Sequential modeling for video frame analysis  
- **Django** — Web framework for the detection interface  
- **NumPy / Pandas / Matplotlib** — For data processing and visualization  

---

## 4. Results  

| Model Name | Videos | Frames | Accuracy (%) |
|-------------|---------|---------|---------------|
| `model_84_acc_10_frames_final_data.pt` | 6000 | 10 | 84.21 |
| `model_87_acc_20_frames_final_data.pt` | 6000 | 20 | 87.79 |
| `model_89_acc_40_frames_final_data.pt` | 6000 | 40 | 89.35 |
| `model_90_acc_60_frames_final_data.pt` | 6000 | 60 | 90.59 |
| `model_91_acc_80_frames_final_data.pt` | 6000 | 80 | 91.49 |
| `model_93_acc_100_frames_final_data.pt` | 6000 | 100 | **93.58** |

---

## 5. How to Run the Project  

### 🛠️ Setup Instructions  
1. **Clone the repository**  
   ```bash
   git clone https://github.com/sadiyabhokare/Deepfake_Video_Detection.git
   cd Deepfake_Video_Detection
````

2. **Create a virtual environment**

   ```bash
   python -m venv venv
   source venv/Scripts/activate  # On Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Django server**

   ```bash
   python manage.py runserver
   ```

5. **Access the application**
   Open your browser and go to:
   👉 `http://127.0.0.1:8000/`

---

## 6. Future Enhancements

* Integration of transformer-based video models (e.g., ViViT, TimeSformer).
* Optimization for **real-time deepfake detection**.
* Expansion to include **audio and image deepfake detection**.
* Integration with **cloud APIs** for scalable deployment.

---

## 7. Contributors ✨

* [**Sadiya Bhokare**](https://github.com/sadiyabhokare)
* [**Contributor 2 Name**](https://github.com/username2)
* [**Contributor 3 Name**](https://github.com/username3)
* [**Contributor 4 Name**](https://github.com/username4)

---

⭐ **If you found this project helpful, don’t forget to give it a star on GitHub!**
