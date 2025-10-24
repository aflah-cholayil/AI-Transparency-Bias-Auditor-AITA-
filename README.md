# 🧠 AI Transparency & Bias Auditor (AITA)

### 📘 Project Overview
The **AI Transparency & Bias Auditor (AITA)** is a machine learning project focused on **identifying, measuring, and mitigating algorithmic bias** in AI models.  
It demonstrates how fairness metrics and corrective algorithms can be applied to ensure **ethical and transparent AI decision-making** across multiple domains.

---

### 🎯 Objectives
- Detect unfair patterns in AI predictions (like gender or race bias)
- Measure fairness using **Demographic Parity Difference (DPD)** and **Equalized Odds Difference (EOD)**
- Apply **bias mitigation** using the **Fairlearn Exponentiated Gradient algorithm**
- Maintain model accuracy while improving fairness

---

### 📊 Datasets Used
Synthetic datasets were generated to simulate real-world bias scenarios:
1. **Hiring Dataset** – explores gender bias in recruitment  
   Features: gender, degree, experience, selected (target)
2. **Loans Dataset** – explores racial bias in financial approvals  
   Features: race, income, credit_score, loan_approval (target)
3. **Students Dataset** – explores school-type bias in education  
   Features: school_type, parental_education, final_grade (target)

Each dataset contains approximately **2,000 records**.

---

### ⚙️ Tech Stack
- **Language:** Python  
- **Libraries:** pandas, numpy, scikit-learn, fairlearn, matplotlib  
- **Database:** MySQL (connected to Jupyter Notebook)  
- **IDE:** Jupyter / Google Colab  
- **Visualization:** Matplotlib / Power BI

---

### 🧩 Methodology
1. **Data Preprocessing**
   - Imported data from MySQL
   - Encoded categorical features (gender, race, school_type)
   - Normalized numerical features

2. **Model Development**
   - Trained a **Random Forest Classifier**
   - Used **Stratified Cross-Validation** to ensure balanced data distribution

3. **Fairness Measurement**
   - Calculated **DPD** and **EOD** using the Fairlearn library

4. **Bias Mitigation**
   - Applied **Exponentiated Gradient** method from Fairlearn
   - Retrained model to reduce bias while maintaining performance

5. **Post-Mitigation Analysis**
   - Compared before/after fairness metrics
   - Visualized improvements in fairness and accuracy

---

### 📈 Results Summary
| Dataset | DPD (Before → After) | EOD (Before → After) | Observation |
|----------|----------------------|----------------------|--------------|
| Hiring | 0.0772 → 0.0390 | 0.2135 → 0.1034 | Moderate improvement |
| Loans | 0.2546 → 0.0701 | 0.4400 → 0.1267 | Major bias reduction ✅ |
| Students | 0.0846 → 0.0110 | 0.1782 → 0.0568 | Mild improvement |

---

### 💡 Key Learnings
- AI models can unintentionally learn human or data bias.  
- Fairness metrics (DPD, EOD) are essential for ethical evaluation.  
- Fairlearn helps mitigate bias effectively without losing much accuracy.  
- Responsible AI practices build **trustworthy and transparent models**.

---


---

### 🧑‍💻 Author
**Aflah C**  
Email: aflahcholayil@gmail.com
🔗 https://www.linkedin.com/in/aflah-cholayil

---

### 🏁 Conclusion
The AI Transparency & Bias Auditor (AITA) successfully demonstrated that **machine learning models can be audited and corrected for fairness**.  
By using Fairlearn, the project achieved a balance between **accuracy and ethical responsibility**, contributing toward **trustworthy AI systems**.
