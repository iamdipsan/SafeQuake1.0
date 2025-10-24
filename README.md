## QuakeSafe v1.0 Overview

The idea for this project came when I was reading an article about earthquakes in Nepal. Nepal is a country that's prone to earthquakes. The Gorkha earthquake of 2015 took many lives and destroyed multiple buildings.  

Many houses still have damages, and people live in them, which is extremely dangerous. Cracks and weak structural surfaces could cause life-threatening issues if another earthquake strikes in the future.

Hiring an engineer to assess the damage is expensive, and doing it on your own is a hassle. Therefore, our goal with this project is to use the power of AI so that a normal person with a phone or a computer can independently analyze damages in their house.  

We are just starting out on this project. This is the **first version (v1.0)** of the application and so we started as a **web application**. We have plans to move to a **mobile application** in the future.

- - -

## 💻 Demo
A demo web application **will be available soon**.  
Users will be able to upload images of house walls and receive predictions on the presence of cracks.

- - -

## 🏗️ Methodology & Architecture
We trained a deep learning model to detect surface cracks in concrete structures. The model we used was **EfficientNetB0 with transfer learning**, providing a strong balance of accuracy and efficiency.  

Model training has been completed, and we are currently working to integrate it into a web interface.  

We hope this will help people quickly and safely assess their house walls without needing expensive professional inspection.

- - -

## 📂 Datasets
**Concrete Crack Images for Classification**  
- 40,000 labeled images of concrete surfaces  
- Two categories: `Crack` and `No Crack`  
- Images are RGB and resized to 224×224 pixels  

- - -

## 📊 Model Performance
The model **achieved** high accuracy in detecting structural cracks.

| Model | Dataset | Accuracy | Precision | Recall | F1-Score |
|--------|----------|-----------|------------|---------|-----------|
| EfficientNetB0 | Validation Set | 99.91% | 0.9987 | 0.9995 | 0.9991 |

**Confusion Matrix**

|                | Predicted No Crack | Predicted Crack |
|----------------|--------------------|-----------------|
| True No Crack  | 4075               | 5               |
| True Crack     | 2                  | 3918            |

**Prediction Confidence**  
- **No Crack:** 0.0023  
- **Crack:** 0.9987  

- - -

## ⚙️ Current Status
- ✅ Model training completed  
- 🚧 Frontend development in progress  
- 🚧 Backend integration in progress  

- - -

## 🎯 Ongoing Improvements
We are continuously working to make QuakeSafe more useful and user-friendly. Over time, we plan to:  

- Add support for scanning an entire building using multiple images  
- Detect cracks with severity levels (minor, moderate, severe)  
- Provide visual crack highlighting and localization on images  
- Generate PDF reports for building inspections  
- Develop a mobile-friendly version for on-site analysis  
- Integrate building layouts and floor plans for more comprehensive assessments  

These upgrades will make the application more powerful and easier for users to safely assess their homes.

- - -

## 💬 Feedback and Support
For feedback, issues, or support, please open an issue

- - -

## 📜 License
This project is licensed under the **MIT License**.
