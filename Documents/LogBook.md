

---

# 📝 LOG BOOK  
#### 1.1 Background & Motivation  
- Climate change and resource consumption are pressing global concerns.  
- Individuals lack awareness of how daily habits impact carbon emissions.  




#### 1.2 Problem Statement  
- There’s a scarcity of user-friendly, real-time, personalized carbon footprint tracking systems.  

#### 1.3 Objectives  
- Estimate personal carbon emissions from travel, food, energy, and waste inputs.  
- Provide category-wise breakdown and reduction suggestions.  
- Deploy an interactive, lightweight Streamlit-based web app.  


## 📅 Weekly Progress

| Week | Date Range       | Tasks Completed                                     | Next Steps                         |
|------|------------------|-----------------------------------------------------|-------------------------------------|
| 1    | 19/8/24 - 24/8/24| Introduction: Background, Motivation             | Finalize problem statement         |
| 2    | 30/8/24 - 3/8/24| Introduction: Problem Statement, Objectives      | Literature survey planning         |
| 3    | 10/10/24 - 15/10/24  | Literature Survey: Reviewed carbon tracking tools| Analyze model gaps                 |
| 4    | 15/11/24 - 21/12/24 | Proposed System: Architecture, input-output flow | Finalize tech stack & libraries    |
| 5    | 2/1/25 - 5/1/25| Requirements: Streamlit setup, dataset sourcing  | Design input forms & layout        |
| 6    | 10/1/25 - 17/1/25| Methodology: Model training, feature selection   | Integrate trained model into UI    |
| 7    | 19/1/25 - 22/1/25| Module 1: UI Design with Streamlit              | Add interactive charts & visual UI |
| 8    | 1/2/25 - 15/2/25| Module 2: Prediction logic, model integration  | Work on emission breakdown visuals |
| 9    | 1/3/25 - 10/3/25| Module 3: Carbon category summaries, testing   | Optimize & debug app               |
| 10   | 3/4/25 - 25/4/25| Outcome: Final testing, report writing          | Deployment & documentation         |


---

## Chapter 2: Literature Survey  

### 2.1 Existing Systems  
- Tools like Pawprint, JouleBug, and Carbonfootprint.com exist.  
- Most are commercial or region-specific.  

### 2.2 Research Gaps  

#### 2.2.1 Missing Features  
1. *Customizability*: Few systems tailor calculations to local data.  
2. *Offline Capability*: Most solutions require continuous internet.  
3. *Model Transparency*: Calculations are often black-box.  
4. *Visualization*: Limited use of clear, interactive charts.  

#### 2.2.2 Summary Table  
| Feature               | Existing Tools     | Ideal Goal     | Gap        |
|-----------------------|--------------------|----------------|------------|
| Personalization       | Partial            | Full           | Moderate   |
| Offline Usability     | Rare               | Yes            | High       |
| Open-source Access    | Rare               | Required       | High       |
| Visual Reports        | Basic Pie Charts   | Rich Interactivity | High  |

---

## Chapter 3: Proposed System

### 3.1 Architecture

- *Input Module*: Collects user data (travel, energy, waste, food habits)
- *Processing Module*: Uses a trained ML model to predict carbon emissions
- *Output Module*: Displays emission breakdown (charts), eco-tips, and feedback

### 3.2 Technology Stack

- *Frontend*: Streamlit  
- *Backend*: Python  
- *Modeling*: Scikit-learn (.sav model for prediction)  
- *Visualization*: Matplotlib , PIL



##### 3.2.1 System Overview  
![System Architecture](doc/system_architecture.png)  

---

## Chapter 4: Implementation

### 4.1 Phase 1 (Completed)
#### UI & Data Preprocessing
- Designed the homepage with structured input forms
- Created intuitive sections: *Personal Info, Travel, Energy, Waste, Food*
- Sidebar layout implemented for smooth user navigation
- Performed *data cleaning, normalization*, and missing value handling
- Conducted *Exploratory Data Analysis (EDA)*:
  - Visualized distribution of carbon contributors
  - Identified high-emission patterns across user categories

### 4.2 Phase 2 (Completed)
#### Model Training
- Used preprocessed data to train a Machine Learning model
- Model predicts *annual carbon footprint (in tons CO₂e)* based on user inputs
- Covered main domains: *Travel, Electricity, Food, Waste*
- Evaluated performance using metrics like *R² score, MAE*
- Tuned hyperparameters for optimal accuracy

### 4.3 Phase 3 (Upcoming)
#### Deployment & Integration
- Plan to integrate the application into a *government or public-facing portal* as a *carbon survey tool*


## 🔧 Software & Hardware Requirements
- Software: Python 3.x, Streamlit, Pandas, Scikit-learn, Matplotlib  
- Hardware: Local machine with 4GB+ RAM, browser-based execution  

---

## ✅ Outcomes & Deliverables  
- Fully functional Carbon Footprint Tracker  
- Real-time CO₂e estimation  
- Personalized charts and eco-friendly suggestions  
- Report export and share functionality  

---

## 📚 References  
1. IPCC Guidelines for National Greenhouse Gas Inventories  
2. “Carbon Footprint Estimation Methods” – IEEE Access  
3. Streamlit Documentation  
4. Dataset Source: [UCI ML Repository](https://archive.ics.uci.edu)
