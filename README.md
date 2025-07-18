# Cd-Wise: An AI-Powered Mobile Application for Cadmium Risk Management in Vegetables

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Platform](https://img.shields.io/badge/Platform-Android-green.svg)](#installation)
[![Language](https://img.shields.io/badge/Language-Java-orange.svg)](#technical-stack)

**Authors:** [Your Name/Team Name]  
**Institution:** Laboratory of Environmental Ecological Health, Xiangtan University

This repository contains the official mobile application, **Cd-Wise**, developed as a practical implementation of the research detailed in the paper: *"The development of the 'Cd-Wise' app for human health risk assessment, dietary recommendations, and planting structure adjustment of cadmium in Chinese vegetables Based on machine learning"*.

**Cd-Wise** is an intelligent mobile tool designed to empower consumers, farmers, and researchers in managing the health risks associated with cadmium (Cd) contamination in vegetables. Leveraging machine learning models, the app provides a comprehensive suite of features from prediction to actionable guidance.

---

## ⏬ Downloads

You can download the latest installable APKs directly from this repository:

-   [**Cd Wise (English Version)**](./Cd%20Wise.apk)
-   [**镉无忧 (Original Chinese Version)**](./镉无忧.apk)

## ✨ Key Features

The application is built upon three core modules, each powered by custom-trained machine learning models:

### 1. 🔬 Cadmium Content Prediction
-   **Intelligent Prediction:** Utilizes a regression model (trained with TensorFlow Lite) to predict the cadmium concentration (mg/kg) in various vegetables based on geographical, seasonal, and species-specific data.
-   **Smart Feature Filling:** Implements a similarity-based imputation mechanism to intelligently fill in missing environmental parameters (e.g., soil pH, organic matter), enhancing prediction accuracy even with incomplete user input.
-   **Immediate Risk Assessment:** Compares the predicted Cd content against established standards (e.g., CAC) to provide an instant risk level classification (None, Low, Medium, High).

### 2. ❤️ Human Health Risk Assessment
-   **Personalized THQ Calculation:** Employs four distinct classification models (for urban/rural and male/female populations) to assess the Target Hazard Quotient (THQ), providing a personalized non-carcinogenic health risk evaluation.
-   **Dietary Safety Guidance:** Based on the calculated risk level, the app generates tailored dietary recommendations, suggesting which vegetables to consume freely, which to limit, and which to avoid.
-   **Visual Data Analysis:** Presents complex risk data through intuitive charts, illustrating the influence of different factors (e.g., body weight, daily intake) on the overall health risk.

### 3. 🌱 Planting Optimization Advice
-   **Comprehensive Soil Assessment:** Analyzes soil parameters (either user-provided or intelligently imputed) to determine the cadmium pollution level and bioavailability.
-   **Smart Crop Recommendation:** Recommends suitable, low-cadmium-accumulating vegetable species based on the soil's risk factor.
-   **Actionable Improvement Strategies:** Provides scientific and practical advice on soil remediation techniques, such as pH adjustment, organic matter management, and the application of passivating agents, to reduce cadmium uptake by plants.

---

## 🛠️ Technical Stack & Architecture

-   **Platform:** Android (Java)
-   **Machine Learning:** TensorFlow Lite for on-device inference.
-   **Models:**
    -   **VCd Model:** A regression model for predicting vegetable cadmium content.
    -   **THQ Models:** Four separate multi-class classification models for health risk assessment.
-   **Data Management:**
    -   **Model Assets (`/assets/models`):** Includes JSON files for category mappings, pre-trained model feature lists, and the similarity database for smart feature filling.
    -   **Local Storage:** SQLite and Room Persistence Library for storing user prediction history.
-   **UI/UX:** Android XML Layouts with Material Design components.
-   **Data Visualization:** [MPAndroidChart](https://github.com/PhilJay/MPAndroidChart) library for rendering bar and pie charts.

---

## 📲 Installation

1.  Download the `Cd Wise.apk` file from this repository.
2.  On your Android device, navigate to the downloaded file.
3.  You may need to enable "Install from unknown sources" in your device's security settings.
4.  Tap the file and follow the on-screen instructions to install the application.

## 📜 License

This project is licensed under the Apache License 2.0. See the [LICENSE](./LICENSE) file for details.

---

## 🎓 Citation

If you use this application or its underlying research in your work, please cite our paper:



---

> © 2025 Laboratory of Environmental Ecological Health, Xiangtan University. All Rights Reserved.
