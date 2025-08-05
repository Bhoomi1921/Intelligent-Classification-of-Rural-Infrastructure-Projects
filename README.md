# IBM SkillsBuild 4-Week Internship on AI & Cloud Technologies

This repository presents the capstone project completed during the **IBM SkillsBuild 4-Week Internship on AI & Cloud Technologies**. This prestigious internship was jointly offered by **IBM SkillsBuild**, **AICTE**, and the **Edunet Foundation**, and aimed at solving real-world challenges using AI and Cloud.

The internship focused on hands-on learning, project-based problem solving, and skill development using the IBM Cloud ecosystem, including IBM Watsonx.ai and AutoAI.

## 📝 Table of Contents
- [Intern Details](#intern-details)
- [About the Internship](#about-the-internship)
- [Project: Intelligent Classification of Rural Infrastructure Projects](#project-intelligent-classification-of-rural-infrastructure-projects)
  - [Problem Statement](#problem-statement)
  - [Proposed Solution](#proposed-solution)
- [⚙️ Technology Stack](#️-technology-stack)
- [🚀 System Development Workflow](#-system-development-workflow)
- [📊 Algorithm & Deployment](#-algorithm--deployment)
- [📈 Results](#-results)
- [📁 Repository Contents](#-repository-contents)

---

## 👩‍💻 Intern Details
- **Name:** BHOOMI GUPTA  
- **Institute:** BANASTHALI VIDYAPITH  
- **Specialization:** Artificial Intelligence  
- **Internship Duration:** 15th July 2025 – 7th August 2025  
- **Internship ID:** INTERNSHIP_1748937226683eaa0a58abc  
- **AICTE Student ID:** STU674206d94e43f1732380377  

---

## 📖 About the Internship
This 4-week internship provided an in-depth understanding of AI and cloud technologies. It included:
- **IBM Cloud** registration and hands-on practice
- **AI & Machine Learning** fundamentals and project work
- **Watsonx.ai & AutoAI** for model experimentation
- **Mentor-led sessions** and masterclasses

**Certification Criteria:**
- Participation in all weekly sessions  
- Completion of at least 2 IBM SkillsBuild courses  
- Final project submission and evaluation

---

## 💡 Project: Intelligent Classification of Rural Infrastructure Projects

### 🧩 Problem Statement
The **Pradhan Mantri Gram Sadak Yojana (PMGSY)** includes various rural development schemes like PMGSY-I, PMGSY-II, and RCPLWEA. Classifying projects into these schemes manually is inefficient, error-prone, and non-scalable.

### ✅ Proposed Solution
An **AI-powered classification system** was built using IBM Watsonx.ai to automatically categorize rural road projects into the correct PMGSY scheme using attributes like cost, length, state, and project duration. The final model was deployed as a web service for real-time predictions.

---

## ⚙️ Technology Stack
- **Cloud Platform:** IBM Cloud
- **AI Platform:** IBM Watsonx.ai Studio
- **AutoML Engine:** IBM AutoAI
- **Core Technologies:**
  - Python
  - Pandas, NumPy
  - Scikit-learn, XGBoost
  - Matplotlib (for EDA)
  - Watsonx SDK

---

## 🚀 System Development Workflow
1. **Data Collection:**  
   - Source: [AI Kosh PMGSY Dataset](https://aikosh.indiaai.gov.in/web/datasets/details/pradhan_mantri_gram_sadak_yojna_pmgsy.html)  
   - Included fields like project cost, road length, state, scheme label, etc.

2. **Preprocessing & Feature Engineering:**  
   - Handled missing values and encoded categorical data  
   - Derived features such as cost per km, project duration  

3. **Model Training with AutoAI:**  
   - Launched AutoAI experiment with 10 pipelines  
   - Pipeline 10 using **Random Forest Classifier** performed best  

4. **Model Deployment:**  
   - Exported the model to Watsonx Deployment Space  
   - REST API enabled real-time prediction using JSON input  

---

## 📊 Algorithm & Deployment

- **Selected Algorithm:** `Random Forest Classifier`  
- **Why Random Forest?**  
  - High accuracy for structured/tabular data  
  - Handles mixed feature types  
  - Robust to class imbalance

- **Input Features Used:**
  - `STATE_NAME`
  - `DISTRICT_NAME`
  - `LENGTH_OF_ROAD_WORK_SANCTIONED`
  - `COST_OF_WORKS_SANCTIONED`
  - `NO_OF_ROAD_WORK_SANCTIONED`
  - `EXPENDITURE_OCCURED`
  - `LENGTH_OF_ROAD_WORK_COMPLETED`
  - `NO_OF_ROAD_WORKS_COMPLETED`

- **Output:**  
  - Predicted Scheme Label (e.g., PMGSY-I, II)  
  - Confidence Score (e.g., 90% for Pipeline #10)

---

## 📈 Results

### 🔹 Prediction Results with Confidence
![Prediction Results Table View](assets/Screenshot%202025-08-03%20174314.png)

> **Prediction Examples:**
- PMGSY-II → 91%  
- PMGSY-I → 90%  

## 📁 Repository Contents
| File                                                                                     | Description                          |
| ---------------------------------------------------------------------------------------- | ------------------------------------ |
| `Intelligent_Classification_PMGSY.ipynb`                                                 | Final Jupyter notebook with pipeline |
| `Bhoomi_Gupta_4_Week_IBM_AI_and_Cloud_Internship.pdf`                                    | Project presentation                 |
| `Intelligent_Classification_of_Rural_Infrastructure_Project_Deployment_test_result.json` | Sample JSON output                   |
| `README.md`                                                                              | This documentation file              |
