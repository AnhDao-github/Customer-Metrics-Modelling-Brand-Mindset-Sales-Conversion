# ☕ Customer Metrics Modelling: Brand Mindset & Sales Conversion

## 📊 Project Overview
To bridge the gap between marketing activity and financial performance, this project moves beyond lagging sales data to build a comprehensive **Customer Metrics Model** for Café Dulcis, a specialty coffee shop in Lappeenranta. 

By analyzing the relationship between marketing variables and customer brand perception, this data reveals a critical strategic misalignment: current advertising efforts are negatively impacting *Brand Liking*, which the model identifies as the sole metric that successfully converts into sales. This project decodes specific customer mindset dynamics (Potential, Stickiness, and Responsiveness) to optimize marketing investments and secure sustainable revenue growth.

**[👉 View the full HTML Data Report here](https://anhdao-github.github.io/Caf-Dulcis-Marketing-Mindset-Sales-Conversion-Analysis/)**

## 🛠️ Tech Stack & Methodology
* **Language:** R
* **Libraries:** `tidyverse`, `tseries`, `vars`, `R6`
* **Modelling Techniques:**
  * **Autoregressive (AR) Modelling:** Applied to calculate metric "Stickiness" (the decay rate and endurance of consumer mindset).
  * **Log-Linear Regression:** Applied to calculate short-term marketing "Responsiveness" and sales "Conversion."
  * **Gap Analysis:** Applied to calculate market "Potential."

## 💡 Key Modelling Insights

### 1. Market Potential (Room for Growth)
* **Brand Awareness (77.6%):** Massive room for growth; modeled as the top top-of-funnel priority.
* **Brand Consideration (73.5%):** High potential; efforts here will yield strong returns.
* **Brand Liking (25.9%):** Highly saturated; the model indicates that investing more capital here will result in diminishing returns.

### 2. Metric Stickiness (Volatility vs. Endurance)
* **Brand Consideration (76.3%) & Liking (76.0%):** Highly sticky. Gains made in these metrics are stable and enduring without needing constant financial reinforcement.
* **Brand Awareness (43.1%):** Highly volatile. Without continuous marketing presence, the model shows consumers quickly forget the brand.

### 3. Responsiveness & Conversion
* **The Advertising Problem:** Current advertising has a negative, statistically significant impact on Brand Liking (coeff = -0.0526, p = 0.0429). 
* **The Sales Driver:** Direct short-term sales responsiveness to promotions/ads is flat. The model proves Brand Liking is the primary customer metric that actually converts into revenue.

## 🎯 Strategic Action Plan

Based on the quantitative outputs of the customer metrics model, Café Dulcis must pivot its strategy:

1. **🚨 Stop Current Ad Spend:** Current ads actively hurt Brand Liking. Immediately pause campaigns and redesign creative content to reflect a premium, high-quality specialty coffee experience.
2. **🚀 Drive Consideration (Best ROI):** Consideration offers the best combination of high growth potential and high stickiness. Shift budget to compelling trial promotions (e.g., first-time discounts, local partnerships).
3. **👀 Maintain Continuous Awareness:** Because awareness decays rapidly (low stickiness), utilize low-cost, "always-on" visibility tactics like local SEO and organic social media rather than expensive, short-burst campaigns.
4. **🤝 Leverage Existing Brand Liking:** Since Liking is already saturated, lean into product excellence. Implement referral programs to incentivize highly satisfied customers to act as organic lead generators.

## 📂 Repository Contents
* `/data`: Contains the `CafeDulcis.csv` dataset.
* `/notebooks`: The R Markdown (`.Rmd`) script detailing the regression models and AR calculations.
* `/docs`: The knitted HTML report showcasing the full analysis.
