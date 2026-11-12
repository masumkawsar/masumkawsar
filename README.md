<h1 align="center">Md Masum Kawsar</h1>

<p align="center">
  <b>IoT Systems · Edge AI &amp; TinyML · IoT Security · Embedded Machine Learning · Low-Cost Sensing</b><br>
  BSc in Computer Science &amp; Engineering, Daffodil International University, Bangladesh (2026)
</p>

<p align="center">
  <a href="mailto:masumkawsarpavel@gmail.com"><img src="https://img.shields.io/badge/Email-masumkawsarpavel%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/Seeking-PhD%20in%20IoT%20%2F%20Edge%20AI-2ea44f?style=flat" alt="Seeking PhD">
</p>

---

### 🔬 About me

I build **low-cost IoT systems that run machine learning directly on microcontrollers**. My work goes from the
hardware (circuit design, sensor calibration, hand-wired ESP32 prototypes) to the data (long field
deployments, open datasets) to the model (TinyML exported as C code and benchmarked on the device), and
I evaluate it with careful statistics (nested grouped cross-validation, multiple seeds, Wilcoxon tests with Holm correction).

I am looking for a **PhD position in IoT / Edge AI / IoT Security in the USA**, where I want to work on:

- **Reliable TinyML on cheap sensors**: models that stay accurate when sensors drift, age and change with humidity
- **IoT intrusion detection that works on real networks**, not only on the dataset it was trained on
- **Explainable, resource-aware ML** for devices with kilobytes of memory and microseconds per decision

---

### 📌 Research projects

#### 1. Low-Cost Indoor Air Quality Monitoring and Short-Term Forecasting on ESP32 (TinyML)
*Submitted to SN Computer Science*

- Designed and hand-wired an **ESP32 + Winsen MP-135 MOS gas sensor + DHT22** monitor; collected **46,897 readings over 17 days** in an occupied room in Dhaka
- Built a **humidity- and temperature-compensated, drift-robust relative Pollution Index** using a rolling 3-hour baseline
- Deployed a **60-tree LightGBM model as ~60 KB of C code on the ESP32 (86 µs per forecast)**, cutting forecast error by **13–16%** against a persistence baseline at 2, 5 and 10-minute horizons
- Class accuracies of **93.7%, 87.9% and 82.4%**; dataset, firmware and live dashboard are open

📂 [Dataset (DOI 10.5281/zenodo.23888099)](https://github.com/masumkawsar/indoor-air-quality-esp32-dataset) · 🌐 [Live dashboard web app](https://github.com/masumkawsar/room-air-monitor)

#### 2. Local Labels Beat Public Data: Cross-Network Evaluation of Lightweight, Explainable IoT Intrusion Detectors
*Submitted to SN Computer Science*

- Evaluated **five model families and nine microcontroller-sized models** on **four public NetFlow-v2 datasets**, over 10 seeds with Holm-corrected Wilcoxon tests
- Showed that detectors with **0.94 MCC within a dataset fall to about zero on other networks** (62% of cross-dataset pairs below 0.5 ROC-AUC) and explained why with **SHAP and distribution-shift analysis**
- With only **1,000 local labels**, a **405-byte depth-4 decision tree reached 0.79 MCC**, beating tuned Random Forest and XGBoost (≤ 0.76), and classified a flow in **2.4 µs on an ESP32**

📂 [Code, notebook and ESP32 benchmark](https://github.com/masumkawsar/iot-ids-cross-network)

#### 3. Explainable Glaucoma Detection from Retinal Fundus Images
*Submitted to Network Modeling Analysis in Health Informatics and Bioinformatics*

- Compared SVM, XGBoost, DenseNet121 and EfficientNetB3 on ~6,000 fundus images, using HOG, LBP and color-histogram features, transfer learning and **Grad-CAM**
- **DenseNet121: 90.33% accuracy, 97.13 AUC**; deployed as *GlaucomaDetect*, a Flask web app

#### 4. Environmental Sound Classification with Optimized ANN and SVM
*Published in INDJCST, 2026*

- 80-dimensional MFCC features on UrbanSound8K; **94.81% (ANN)** and **94.66% (SVM)** test accuracy with KerasTuner and GridSearchCV
- Deployed as *UrbanSoundAI*, a Flask app with waveform, Mel-spectrogram and MFCC views

---

### 📄 Publications

1. M. A. Mridu, **M. M. Kawsar**. "Comparative Study of Optimized ANN and SVM Models for Environmental Sound Classification with Practical Web-Based Deployment." *Indian Journal of Computer Science and Technology (INDJCST)*, Vol. 5, Issue 2, pp. 904–910, 2026. [doi:10.59256/indjcst.20260502098](https://doi.org/10.59256/indjcst.20260502098)
2. **M. M. Kawsar**. "Low-Cost Indoor Air Quality Monitoring and Short-Term Forecasting on ESP32 Using a Humidity-Compensated MOS Sensor and TinyML." *Submitted to SN Computer Science.*
3. **M. M. Kawsar**. "Local Labels Beat Public Data: Cross-Network Evaluation of Lightweight and Explainable IoT Intrusion Detectors." *Submitted to SN Computer Science.*
4. M. A. Mridu, **M. M. Kawsar**. "Comparative Evaluation of Machine Learning and Transfer-Learning-Based Deep Learning Models for Explainable Glaucoma Detection from Retinal Fundus Images." *Submitted to NetMAHIB.*

---

### 🛠️ Hardware projects

- **Smart Water Level Monitor & Automatic Pump Control**: ESP32 + ultrasonic sensor, OLED display, automatic pump control, buzzer alert, remote monitoring over Blynk IoT
- **Obstacle-Avoiding Robot Car**: Arduino + ultrasonic sensor + motor driver, autonomous navigation

---

### 🧰 Skills

**IoT & Embedded**<br>
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat&logo=espressif&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00878F?style=flat&logo=arduino&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=cplusplus&logoColor=white)
![Blynk](https://img.shields.io/badge/Blynk_IoT-23C48E?style=flat)
![TinyML](https://img.shields.io/badge/TinyML-on--device_inference-FF6F00?style=flat)

Circuit design & prototyping · Sensor interfacing & calibration (MOS gas, ultrasonic, temperature/humidity) · Humidity compensation · Model-to-C export · IoT intrusion detection

**Machine Learning**<br>
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=flat&logo=keras&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-337AB7?style=flat)
![LightGBM](https://img.shields.io/badge/LightGBM-9ACD32?style=flat)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)

Time-series forecasting · Explainable AI (SHAP, Grad-CAM) · Transfer learning · Nested grouped cross-validation · Statistical testing (Wilcoxon, Holm) · MCC / ROC-AUC / Macro-F1

**Tools**<br>
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
![Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=flat&logo=googlecolab&logoColor=black)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat&logo=visualstudiocode&logoColor=white)

---

<p align="center"><i>Open to PhD opportunities and research collaborations in IoT, Edge AI and IoT security. Feel free to reach out.</i></p>
