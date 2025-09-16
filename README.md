# AI-Enhanced Marketing Attribution Analysis
Using AI-driven and traditional attribution models to optimize multi-channel marketing spend.

## Problem Statement
Marketing teams often run campaigns across multiple channels, including Paid Search, Social, Email, and Display. The challenge is understanding how each channel contributes to conversions so budgets can be allocated efficiently. This project compares traditional attribution models (Last-Touch, Linear) with AI-driven methods (Shapley value / ML-based attribution) to provide actionable insights for optimizing marketing spend.

### Key Questions
- Which marketing channels drive the most conversions?  
- How do AI-driven attribution models differ from traditional models in credit assignment?  
- How should the marketing budget be reallocated based on AI insights?

## Methods / Approach

### Traditional Attribution Models
1. **Last-Touch Attribution** – Assigns full credit to the final channel before conversion.  
2. **First-Touch Attribution** – Assigns full credit to the first channel in the user journey.  
3. **Linear Attribution** – Distributes credit equally across all channels in the conversion path.

### AI-Driven Attribution
1. **Shapley Value / ML-Based Attribution** – Uses machine learning models (e.g., XGBoost, Logistic Regression) to predict conversion probabilities. The Shapley value assigns credit to each channel based on its marginal contribution.  
2. **Optional: Time-Decay / Advanced Models** – Channels closer to the conversion receive higher credit than early touchpoints.

### Analysis Steps
- Load and clean the dataset (remove duplicates, handle missing values).  
- Explore data: total conversions, spend per channel, and conversion rates.  
- Apply attribution models to assign conversion credit per channel.  
- Compare results across models to identify undervalued or overvalued channels.  
- Generate actionable recommendations for budget allocation based on AI insights.

## Results / Visualizations
- **Last-Touch Attribution:** Search = XX%, Email = XX%, Display = XX%, Social = XX%  
- **Linear Attribution:** Search = XX%, Email = XX%, Display = XX%, Social = XX%  
- **AI Attribution (Shapley Values):** Search = XX%, Email = XX%, Display = XX%, Social = XX%

![Attribution Comparison Chart](visuals/attribution_chart.png)

## Insights & Recommendations
- Display advertising is undervalued in traditional models (AI shows it contributes XX% of conversions).  
- Reallocate 10% of Paid Search budget to Display to improve ROAS.  
- AI-driven attribution provides a more holistic view of the customer journey compared to Last-Touch.

## Next Steps / Future Work
- Incorporate time-decay attribution for additional insight.  
- Integrate real-time ad spend data for dynamic budget allocation.  
- Test AI models on multi-touch sequences over multiple campaigns.

