# 📊 End-to-End A/B Testing & Experimentation Framework

A product-focused data science project demonstrating how to design, analyze, and interpret A/B experiments to support feature launch decisions using statistical evidence.

---

## 🚀 Project Overview

This project simulates a real-world product experimentation workflow used by data scientists and product analysts to evaluate whether a new feature should be launched.

A product team redesigned the primary call-to-action button on an e-commerce application:

- **Control (A):** Existing button design  
- **Treatment (B):** New “Buy Now” button design  

The business question addressed was:

> **Should the new button be launched to all users?**

Rather than focusing only on hypothesis testing, this project emphasizes **experiment design, uncertainty quantification, and decision-making**, which are central to applied data science in product teams.

---

## 🧠 Skills Demonstrated

- Experiment design & hypothesis formulation  
- Metric selection & practical significance (MDE)  
- A/B testing & statistical inference  
- Confidence intervals & risk assessment  
- Business-oriented decision making  
- Python-based data analysis & visualization  

---

## 🧪 Experiment Design

- **Experiment Type:** A/B Test  
- **Unit of Randomization:** Individual users  
- **Traffic Split:** 50% Control / 50% Treatment  
- **Sample Size:** 10,000 users per group  

### 📌 Primary Metric

**Conversion Rate**  
(Number of users who complete a purchase ÷ Number of users who visit)

---

## 🎯 Practical Significance (MDE)

The **Minimum Detectable Effect (MDE)** was defined *before analysis* as:

- **+0.5% absolute uplift in conversion rate**

This ensures that statistically significant results are also **business-relevant**.

---

## 🧬 Data Generation

Since real product data is unavailable, user behavior was simulated to reflect realistic e-commerce conditions:

- Binary outcome per user (converted / not converted)  
- Baseline conversion rate for the control group  
- Slightly higher conversion rate for the treatment group  

Simulation is commonly used for experimentation prototyping and learning.

---

## 📊 Statistical Analysis

### Test Used

**Two-Proportion Z-Test**

**Rationale:**
- Binary outcome variable  
- Two independent groups  
- Large sample size allows normal approximation  

### Hypotheses

- **H₀:** No difference in conversion rate between control and treatment  
- **H₁:** Conversion rates differ  

**Significance Level:** α = 0.05

---

## 📈 Results

| Metric | Control | Treatment |
|------|--------|----------|
| Conversion Rate | 9.61% | 10.78% |
| Absolute Uplift | — | +1.17% |

**Statistical Results**
- Z-score: 2.73  
- P-value: 0.0063  

---

## 🔍 Confidence Interval & Risk Assessment

A 95% confidence interval was calculated for the conversion rate uplift:

- **95% CI:** **[ +0.33%, +2.01% ]**

This allows stakeholders to:
- Understand uncertainty  
- Evaluate downside risk  
- Make informed launch decisions  

---

## ✅ Final Recommendation

✔ Statistically significant improvement  
✔ Practically meaningful uplift (> MDE)  
✔ Limited downside risk  

📢 **Decision:** Launch the new “Buy Now” button  

Post-launch monitoring is recommended to validate long-term impact.

---

## ⚠️ Assumptions & Limitations

- Data is simulated; real-world behavior may differ  
- No seasonality or traffic quality effects modeled  
- Assumes correct randomization and no experiment contamination  
- Results reflect short-term impact only  

---

## 🛠 Tech Stack

- Python  
- NumPy  
- pandas  
- SciPy  
- Matplotlib  

---

## 📚 Key Takeaways

- Experiments should be designed **before** data analysis  
- Statistical significance does not guarantee business value  
- Confidence intervals are critical for evaluating risk  
- Data scientists act as **decision partners**, not just analysts  

---

## 🔮 Future Improvements

- Power analysis & sample size planning  
- Bayesian A/B testing comparison  
- Segmented analysis (e.g., new vs returning users)  
- Sequential testing considerations  

---


