# Detroit-Blight-Ticket-Compliance

(https://www.kaggle.com/c/detroit-blight-ticket-compliance)

Blight violations are issued by the city to individuals who allow their properties to remain in a deteriorated condition. Every year, the city of Detroit issues millions of dollars in fines to residents and every year, many of these fines remain unpaid. Enforcing unpaid blight fines is a costly and tedious process, so the city wants to know: how can we increase blight ticket compliance?

The first step in answering this question is understanding when and why a resident might fail to comply with a blight ticket. This is where predictive modeling comes in.

Goal: Predict whether a given blight ticket will be paid on time

# Approach

RandomForestRegression model was used in predicting the probability of compliance to be in class 0: non-compliant or 1: compliant. Four numerical predictors fine_amount, discount_amount, judgment_amount, and late_fee were considered. All non-US data and NULL compliance data were ignored in modeling. Model accuracy was evaluated with Area Under ROC (AUC), which was found to be 75.62%.
