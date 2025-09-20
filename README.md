# Project Churn Prediction and Churn solving in Telecoms

  

เป็นโปรเจคที่เขียนด้วย Python และใช้โมเดล Machine learning ในการหาคำตอบว่าปัจจัยใดที่ผลต่อการเลิกใช้งานของผู้ใช้และสามารถต่อยอดวิธีแก้ไขสำหรับลดปัญหาการเลิกใช้บริการของผู้ใช้ต่อผู้ให้บริการเครื่อข่ายมือถือ

## ติดตั้ง Library
```bash
pip install pandas scikit-learn matplotlib seaborn numpy kagglehub imbalanced-learn xgboost
```
## Dataset

ข้อมูลที่นำมาใช้

```bash

https://www.kaggle.com/datasets/blastchar/telco-customer-churn/data

```

โดยเป็นข้อมูลของผู้ใช้บริการที่ถูกบันทึกไว้โดยมีแบบยังใช้งานบริการอยู่ และ เลิกใช้บริการไปแล้ว

![image_alt](https://github.com/Alanno25/Project-Churn-prediction/blob/074ef43258df20e7e90c11149ba40d2c4bc2a9d1/dataset%20churn.png)
จำนวน 7043 แถวและ 21 หัวข้อ


---


ข้อมูลจำนวนผู้ใช้งาน 5174 คนและผู้ที่ยกเลิกการใช้งาน 1869 คน



![image_alt](https://github.com/Alanno25/Project-Churn-prediction/blob/1fac95ac28ec08449f2f3bed959e1d1cefac1c84/Chrun%20count.png)

![image_alt](https://github.com/Alanno25/Project-Churn-prediction/blob/81e72e28438e5c3da668f4c2f5584ca384d5c59e/Distribution%20of%20Churn.png)

โดยมีสัดส่วนของผู้ใช้เพศชาย-หญิงดังนี้

![image_alt](https://github.com/Alanno25/Project-Churn-prediction/blob/eb4245063a69919cf31d6af0c33832689dc0f10d/gender%20churn%20count.png)





1.  **Problem Statement**: ปัญหาคืออะไร ทำไมต้องแก้

2.  **Dataset**: ข้อมูลมาจากไหน มีหน้าตาเป็นอย่างไร

3.  **Methodology**: อธิบายขั้นตอนที่คุณทำแบบสรุป (เช่น Data Cleaning -> EDA -> Feature Engineering -> Modeling -> Evaluation)

4.  **Key Findings**: สิ่งที่ค้นพบจาก EDA คืออะไร? Feature ไหนที่ดูมีผลกับ Churn บ้าง?

5.  **Model Results**: สรุปผลโมเดลที่ดีที่สุด ทำไมถึงเลือกตัวนี้? Metric ที่ได้คือเท่าไหร่?

6. **How to Run**: ขั้นตอนการรันโปรเจกต์ของคุณ



