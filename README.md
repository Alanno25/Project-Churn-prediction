# Project Churn Prediction 

เป็นโปรเจคที่เขียนด้วย Python และใช้โมเดล Machine learning ในเพื่อหาคำตอบว่าปัจจัยใดที่มีผลต่อการเลิกใช้บริการ (Churn) ของผู้ใช้บรืการ เพื่อให้สามารถวางแผนวิธีแก้ไขสำหรับลดปัญหาการเลิกใช้บริการ และดำเนินการเพื่อรักษาลูกค้าไว้ได้


## Table of Contents
* Project Overview
* Problem Statement
* Data Source
* Key Feature & Insights
* Methodology
* Technologies Used
* How to Run the Project
* Results & Model Performance
* Future Enhancements
* Contact 

## Project Overview
โปรเจคนี้ใช้ข้อมูลจากเว็บไซต์ kaggle เพื่อใช้ทำการสร้างโมเดลทำนายการ Churn โมเดลนี้ช่วยให้สามารถระบุลูกค้าที่มีความเสี่ยงสูงเพื่อช่วยป้องกันการสูญเสียลูกค้า

## Problem Statement
* ปัญหาการสูญเสียลูกค้า (Customer Churn) ที่ส่งผลกระทบต่อรายได้ของบริษัท
* โปรเจคนี้มุ่งเน้นในการสร้าง Predictive Model เพื่อทำนายลูกค้าที่มีแนวโน้มที่จะยกเลิกบริการในอนาคต

## Data Source

### Data Set 
```bash
WA_Fn-UseC_-Telco-Customer-Churn.csv
```


### Source

```bash

https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data

```
### Description 
มีจำนวน 21 Column
* customerID  รหัสลูกค้า
* gender เพศ
* SeniorCitizen ผู้สูงอายุ
* Partner คู่ครอง
* Dependents ผู้อยู่ในความดูแล
* tenure ระยะเวลาที่ใช้บริการ
* PhoneService บริการโทรศัพท์
* MultipleLines มีหลายเบอร์โทร
* InternetService ประเภทของบริการอินเทอร์เน็ต
* OnlineSecurity บริการรักษาความปลอดภัยออนไลน์
* OnlineBackup บริการสำรองข้อมูลออนไลน์
* DeviceProtection บริการคุ้มครองอุปกรณ์
* TechSupport บริการช่วยเหลือทางเทคนิค
* StreamingTV บริการสตรีมมิ่งทีวี
* StreamingMovies บริการสตรีมมิ่งภาพยนตร์
* Contract ประเภทสัญญา
* PaperlessBilling รับบิลแบบกระดาษ
* PaymentMethod วิธีชำระเงิน
* MonthlyCharges ค่าบริการรายเดือน
* TotalCharges ค่าบริการทั้งหมด
* Churn การเลิกใช้บริการ

## Key Features & Insights(ทำอันนี้)
พบว่าลูกค้าที่มีระยะเวลาที่ใช้บริการสั้นๆ และ มีประเภทสัญญาแบบรายเดือนนั้น มีอัตราการ Churn ที่สูงกว่าการใช้บริการที่ระยะยาว และ ประเภทสัญญาแบบรายปี 

![image_alt](https://github.com/Alanno25/Project-Churn-prediction/blob/2971766ce4764ddf2bfda496f038f5328d999437/tenure%20churn.png)

![image_alt](https://github.com/Alanno25/Project-Churn-prediction/blob/2971766ce4764ddf2bfda496f038f5328d999437/tenure%20churn.png)

## Methodology (ขั้นตอนในการทำงาน)

### 1. Data Preprocessing
การจัดการข้อมูลโดยการแปลงค่าของหัวข้อที่มีตัวเลือก 2 อย่างให้เป็นตัวเลข และ ใช้ One Hot Encoder แปลงค่าของหัวข้อที่มีตัวเลือกมากกว่า 2 อย่างให้เป็นตัวเลขทั้งหมด
รูป encode

### 2. Exploratory Data Analysis 
การวิเคราะห์ข้อมูลเบื้องต้นโดยนำข้อมูลที่แปลงค่าแล้วมาแสดงในรูปแบบต่างๆเพื่อหาความสัมพันธ์ที่เกี่ยวข้องกับปัญหา
รูป plot


### 3. Feature Engineering 
การหา Feature ที่มีความสำคัญจากข้อมูลที่มีอยู่เพื่อนำไปสร้างโมเดล Machine Learning
รูป feature selection 

### 4. Model Building
-   **Baseline Model:** เช่น Logistic Regression
    
-   **Advanced Models:** เช่น RandomForest, XGBoost

### 5. Model Evaluation
การประเมินประสิทธิภาพของโมเดลด้วย Metrics ต่างๆเพื่อตัดสินใจในการเลือกโมเดลที่จะนำไปใช้
รูป evaluation

## Technologies Used

-   **Programming Language:** Python
    
-   **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, XGBoost
    
-   **Tools:** Jupyter Notebook, VS Code


## **How to Run the Project**

ส่วนนี้สำคัญมากสำหรับคนที่อยากจะเอาโค้ดเราไปรันต่อ

1.  **Clone the repository:**
    ```
    git clone <URL_ของ_Repo>
    
    ```
    
2.  **Install dependencies:**
    ```
    pip install -r requirements.txt
    
    ```
    
3.  **Run the notebook:**
    ```
    jupyter notebook Churn_Prediction_Notebook.ipynb
    
    ```
## **Results & Model Performance**

สรุปผลลัพธ์ของโมเดลที่ได้ 📊📈

-   **Best Model:** XGBoost
    
-   **Accuracy:** 80%
    
-   **Precision:** 75%
    
-   **Recall:** 85%
    
-   **F1-Score:** 80%
    
-   **Confusion Matrix:**
    

**อธิบาย:** อธิบายความหมายของแต่ละ Metrics สั้นๆ เช่น "**Recall** สูงบ่งชี้ว่าโมเดลสามารถระบุลูกค้าที่มีแนวโน้มจะ Churn ได้ดี"


## Future Enhancements

-   "ลองใช้ Deep Learning Models (เช่น Neural Networks)"
    
-   "นำข้อมูลใหม่ๆ มาเพิ่ม เช่น ข้อมูลการโทรออก, การใช้แอปพลิเคชัน"
    
-   "สร้างเป็น Web Application (เช่น Stream lit หรือ Flask) เพื่อให้ทีมอื่นใช้งานได้ง่ายขึ้น"

## Contact

ส่วนนี้ไว้สำหรับคนที่อยากจะติดต่อเราได้ 📩

-   **ชื่อ:** นาย ศุภณัฐ นฤนาทมนตรี  (Mr. Supanut Narunartmontree)
    
-   **Email:** supanut.narunartmontree@gmail.com
    
-   **LinkedIn:** URL ของ LinkedIn

```bash
pip install pandas scikit-learn matplotlib seaborn numpy kagglehub imbalanced-learn xgboost
```
