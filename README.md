# 🧪 A/B Testing — Optimizing Eniac’s Homepage Button

## 🎯 Goal

Eniac receives thousands of daily visitors, but only **~2%** click the main **“SHOP NOW”** button on the iPhone banner.

The objective was to test whether changing the **button color and text** could increase the **Click-Through Rate (CTR)** and improve the first step of the purchase funnel.

---

## 🎨 Versions Tested

| Version | Color | Text |
|---|---|---|
| A | White | SHOP NOW |
| B | Red | SHOP NOW |
| C | White | SEE DEALS |
| D | Red | SEE DEALS |

This setup allows measuring the effect of **color**, **text**, and their **combination**.

---

## 🧪 Experiment Design

- Random assignment of visitors  
- ~5,000 visitors per version  
- Primary metric: **CTR = Clicks / Visits**  
- Significance level: **α = 0.05**  
- Statistical test: **Chi-Square test**  
- Post-hoc analysis with **Bonferroni correction**

---

## 📊 Statistical Approach

CTR is based on **click / no-click** (categorical data).  
Therefore, a **Chi-Square test** was used to determine whether click behavior depends on button design.

---

## 🧠 Key Concepts Used in This Project

- **Sampling & Bias** — Random visitor assignment to ensure unbiased results  
- **Central Limit Theorem (CLT)** — Enables reliable inference from large samples  
- **Confidence Intervals** — Estimate where the true CTR likely lies  
- **Hypothesis Testing** — Decide if observed differences are real or random  
- **Chi-Square Test** — Appropriate for click / no-click (categorical) data  
- **Type I & Type II Errors** — Balance between false positives and missed improvements  
- **Multiple Comparison Correction** — Bonferroni method to identify the true best version

---

## 🏆 Key Findings

**Final Decision:** **Version A** (White + “SHOP NOW”) is the winner.

**Why?**

- The Chi-Square test confirmed that real differences exist between the versions.  
- Post-hoc analysis showed **Version A and Version C are not statistically different in CTR**.

**After the click**

Although Version C attracted many clicks, users did not continue the journey as effectively.  
Version A provided a **more consistent and reliable user path** after the initial click.

---

## 💡 Business Insight

Optimizing for **CTR alone** would have led to the wrong decision.  
A broader view of user behavior in the funnel was necessary to select the best design.

---


## 📽 Presentation Slides

A short presentation summarizing the experiment design, statistical analysis, and business conclusions is included in this repository.

You can find it here:  
📁 `slides/Eniac_AB_Testing_Presentation.pdf`

---


## 🛠 Tools

Python, Pandas, SciPy, Hypothesis Testing, A/B Testing principles
