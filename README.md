# 📊 Payment Acceptance EDA

**One-line summary:** What problem you solved and why it matters.

---

## 🧠 Business Problem
Explain this like you're talking to a stakeholder, not a data scientist.

- What decision needed to be made?
- Why was this a problem?
- What happens if nothing changes?

**Example:**  
Online payments were experiencing a decline in authorisation rates in certain countries, leading to lost revenue and customer friction.

---

## 📁 Data
- **Source:** (internal dataset / public dataset / Kaggle / etc.)
- **Time period:** Jan 2023 – Dec 2024
- **Grain:** Transaction-level
- **Rows:** ~2.5M
- **Target variable:** `IS_AUTHORISED`

### Key Features
| Feature | Description |
|------|------------|
| HAS_THREE_DS | Whether transaction required 3DS |
| issuer_country_name | Card issuer country |
| amount | Transaction amount |
| card_type | Debit / Credit |

---

## 🔍 Exploratory Data Analysis (EDA)

Key questions explored:
- How does authorisation rate differ by country?
- What is the impact of 3DS on approval rates?
- Are declines concentrated in certain segments?

### Example Insight
> France shows a **12–15pp lower auth rate** for 3DS transactions compared to non-3DS, suggesting over-application of 3DS.

📈 Example visual:

![Auth Rate by Country](../../Images/project-thumb.png)

---

## 🧪 Methodology
Steps taken:
1. Data cleaning and validation
2. Feature engineering (binning amounts, risk flags)
