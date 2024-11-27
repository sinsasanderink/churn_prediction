# Telecom Customer Churn Prediction

## Problem Statement

In the highly competitive telecom industry, customers can easily switch between service providers, leading to an average annual churn rate of **15-25%**. Since acquiring a new customer is **5-10 times more expensive** than retaining an existing one, reducing customer churn is crucial for telecom companies.

The goal of this project is to **predict which customers are at high risk of churn** by analyzing customer-level data from a leading telecom firm. By building predictive models, we aim to identify the main indicators of churn and provide actionable insights to improve customer retention strategies.

## Customer Lifecycle Phases

1. **Good Phase**: The customer is satisfied and exhibits normal usage behavior.
2. **Action Phase**: The customer begins to experience issues or considers competitors, showing changes in behavior.
3. **Churn Phase**: The customer has decided to leave the service.

Our analysis focuses on detecting customers in the **action phase** to proactively implement retention strategies.

## Approach

1. **Data Analysis and Preprocessing**:
   - Explored and cleaned the dataset.
   - Handled class imbalance (churn rate at **10.19%**).
   - Engineered features based on usage patterns, recharge behavior, and customer demographics.

2. **Model Building**:
   - Developed various machine learning models, including tree-based models (Random Forest, CatBoost) and regression models (Logistic Regression).
   - Performed hyperparameter tuning and cross-validation to optimize model performance.

3. **Model Evaluation**:
   - Evaluated models using metrics like **accuracy**, **recall**, **precision**, and **ROC-AUC score**.
   - Prioritized **recall for churners** to ensure that most potential churners are correctly identified.

## Best Model: Random Forest Classifier

### Why It's the Best

The **Random Forest classifier** emerged as the best-performing model for predicting customer churn:

- **Highest Churner Recall**: Achieved a recall of **76%**, correctly identifying the majority of customers likely to churn.
- **Balanced Performance**: Maintained an overall accuracy of **81%**, offering a good balance between detecting churners and correctly classifying non-churners.
- **Strong ROC-AUC Score**: Scored **0.8517**, indicating good discriminative ability between churners and non-churners.
- **Interpretability**: Allows for easier interpretation of feature importance, aiding in actionable business decisions.

By prioritizing churner recall, this model aligns with the business objective of minimizing customer attrition through proactive engagement and targeted interventions.

## Key Findings

### Important Features Influencing Churn

1. **Zero Call Usage**:
   - Churn rate of **72.4%** among customers with zero call usage.
   - Indicates significant disengagement from voice services.

2. **Declining ARPU (Average Revenue Per User)**:
   - Customers with **ARPU ≤ 100** have a **24.5%** churn rate.
   - A declining ARPU pattern shows a **18.82%** churn rate.

3. **Recharge Frequency and Amount**:
   - **46.3%** of churners had significant recharge drops (>50% decrease).
   - Low recharge frequency correlates with a **23.2%** churn rate.

4. **Tenure**:
   - Customers with tenure **less than 6 months** have the highest churn rate at **22.9%**.
   - Emphasizes the need for early engagement with new customers.

5. **Usage Patterns**:
   - **Voice Usage**: Outgoing calls below 38.7 minutes lead to a **30.7%** churn rate.
   - **Data Usage**: Significant declines in 2G and 3G usage among churners.

6. **High-Value Customers**:
   - Lower churn rate of **5.6%** compared to **11.5%** for regular customers.
   - Highlighting the importance of retaining high-value segments.

## Business Recommendations

### 1. Engage Low Usage Customers

- **Personalized Communication**: Reach out to customers with declining usage to understand their needs.
- **Incentivize Usage**: Offer bonuses like extra minutes or data to encourage increased usage.
- **Service Education**: Provide guidance on maximizing plan benefits.

### 2. ARPU Stabilization Initiatives

- **Customized Plans**: Tailor plans to offer better value for customers with declining ARPU.
- **Loyalty Discounts**: Implement programs rewarding long-term customers.
- **Upselling Opportunities**: Introduce value-added services suited to customer needs.

### 3. Enhance Recharge Experience

- **Recharge Reminders**: Send timely notifications about low balances.
- **Simplify Recharge Process**: Improve user experience on recharge platforms.
- **Recharge Incentives**: Offer discounts for consistent or higher recharge amounts.

### 4. Improve Onboarding for New Customers

- **Welcome Packages**: Provide helpful information and introductory offers.
- **Proactive Support**: Assign representatives to assist with initial setup.
- **Feedback Mechanisms**: Capture and address concerns promptly.

### 5. Retention Strategies for High-Value Customers

- **Exclusive Offers**: Provide special deals and early access to new services.
- **Personal Account Managers**: Strengthen relationships through dedicated support.
- **Recognition Programs**: Acknowledge loyalty with special events or communications.

### 6. Stimulate Service Usage

- **Bundled Services**: Combine voice, data, and other services at discounted rates.
- **Promotional Campaigns**: Target low usage periods with special promotions.
- **Content Partnerships**: Offer exclusive content to incentivize data usage.

### 7. Contract and Plan Improvements

- **Flexible Contracts**: Allow plan adjustments without penalties.
- **Long-Term Incentives**: Encourage longer contracts with added benefits.
- **Transparent Policies**: Build trust through clear contract terms.

### 8. Enhance Service Quality

- **Network Investments**: Improve infrastructure in high churn areas.
- **Quality Monitoring**: Address service issues proactively.
- **Customer Support Excellence**: Resolve issues quickly and effectively.

## Actionable Insights

### Identify High-Risk Customer Segments

- **Low Usage Customers**: Monitor for minimal or no recent usage.
- **Declining ARPU/Recharges**: Track significant drops in revenue and recharge behavior.
- **New Customers with Low Engagement**: Focus on customers within their first year showing low engagement.

### Implement Targeted Marketing Campaigns

- **Personalized Messaging**: Address specific needs of each high-risk segment.
- **Multi-Channel Outreach**: Utilize SMS, email, and app notifications.
- **Test and Optimize**: Use A/B testing to refine strategies.

### Develop Predictive Churn Models

- **Data-Driven Monitoring**: Continuously analyze key indicators.
- **Real-Time Alerts**: Notify retention teams of high-risk behaviors.
- **Continuous Improvement**: Update models with new data for accuracy.

### Enhance Customer Feedback Loops

- **Surveys and Feedback Forms**: Regularly gather customer insights.
- **Net Promoter Score (NPS)**: Measure loyalty and identify detractors.
- **Feedback Analysis**: Utilize analytics to understand customer sentiments.

### Strengthen Customer Relationships

- **Engagement Programs**: Foster community through forums or events.
- **Educational Content**: Help customers maximize service value.
- **Proactive Issue Resolution**: Address potential problems before they escalate.

### Optimize Pricing and Plan Structures

- **Flexible Pricing Models**: Adapt plans to meet varying needs.
- **Competitive Analysis**: Ensure offerings remain attractive in the market.
- **Value Communication**: Clearly articulate plan benefits.

### Leverage Cross-Selling Opportunities

- **Complementary Services**: Offer relevant add-ons.
- **Bundling Discounts**: Encourage multiple service subscriptions.
- **Behavioral Targeting**: Promote services based on usage patterns.

## Conclusion

By focusing on the key drivers of churn and implementing targeted strategies, the telecom company can significantly reduce churn rates, improve customer satisfaction, and enhance profitability. The Random Forest model provides a robust tool for predicting churn, enabling proactive retention efforts that align with business objectives.

---

*Prepared by Ursina Sanderink, Data Scientist*
