# 🚢 Titanic Passenger Insights Dashboard
## Overview  

This repository contains a **dashboard** visualizing the Titanic passenger dataset using enhanced, human-readable categories. It highlights key survival patterns by class, age group, gender, embarkation port, and family size.

## Dataset (Enhanced Columns)  

The source dataset has been enriched with the following new columns and also I changed Datatypes of all columns where needed

- **Survived_Label** – categorical survival status: `Survived` / `Dead` (instead of `1` / `0`)  
- **Pclass_Status** – passenger class as `Upper Class`, `Middle Class`, `Lower Class` (instead of `1`, `2`, `3`)  
- **Age_Bucket** – age categories:  
  - `Adolescent` (0-15) 
  - `Youngster` (16-30)  
  - `Adult` (31–45)  
  - `Old` (46+)  
- **Family_Size** – number of relatives aboard (SibSp + Parch+1), describing group size

## 🚀 Objectives

- Provide a clear visual dashboard to explore survival patterns on the Titanic  
- Demonstrate how **gender**, **passenger class**, **age**, and **family size** affected survival chances  
- Improve raw data readability with conversational categorical columns  
- Enable interactive filtering via slicers for `Pclass_Status` and `Sex`

## 🧠 Key Insights

- Total passengers: **891**; **342 survived**, **549 dead** (~38% survival)  
- **Lower Class (Third Class)** had the highest mortality (~68%), while **Upper Class (First Class)** had the best survival (~40%)  
- Age-wise:  
  - **Youngsters** had the highest number of survivors (~117), followed by **Adults (~102)** and **Adolescents (~101)**  
  - The **Elderly** (Old) had the fewest survivors (~22)  
- **Gender & Family Size**: Females traveling alone (family size = 1) had the highest survival count (~99); survival decreased for larger groups, especially among males  
- **Port of Embarkation**:  
  - Survival counts: Southampton ~219, Cherbourg ~93, Queenstown ~30  
  - Mortality counts: Southampton ~427, Cherbourg ~75, Queenstown ~47  

## 📊 Dashboard Layout

1. Summary cards: Total passengers, Dead & Survived  
2. Survival/mortality breakdown by class  
3. Survivals per age bucket (bar chart)  
4. Survivals by gender & family size (bar chart)  
5. Survival & mortality counts by embarkation port  
6. Overall survival vs. death rate (pie chart)  
7. Gender-wise survival trend  
8. Interactive filters: *Pclass_Status*, *Sex*

## 🛠 Tools & Techniques

| Component         | Tools / Methods                                                                 |
|------------------|---------------------------------------------------------------------------------|
| Dashboard platform| Excel                                                                           |
| Feature engineering| Created `Survived_Label`, `Pclass_Status`, `Age_Bucket`, `Family_Size`         |
| Visualization     | Bar charts, pie charts, trend lines, slicers using best practices               |
| Workflow          | EDA → Feature engineering → Data transformation → Dashboard modeling             |

---
