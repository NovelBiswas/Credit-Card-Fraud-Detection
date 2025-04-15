# Credit-Card-Fraud-Detection
-Develop a fraud detection system to identify fraudulent credit card transactions using Machine Learning. This project involves data preprocessing, exploratory data analysis, feature engineering, model training, and evaluation. 

# Compare Models Based on Precision-Recall Tradeoff
The Precision-Recall (PR) tradeoff is critical in fraud detection because:
-Precision tells you: Of all predicted frauds, how many were actual frauds?
-Recall tells you: Of all actual frauds, how many did we catch?
-In fraud detection, high recall is often preferred — missing a fraud (false negative) is worse than flagging a legit transaction (false positive).

# Choosing the Best Model
Look at:
-Area under the Precision-Recall Curve (AP score)
-Context needs: If catching all frauds is key → pick model with highest recall, even at some precision cost

# Explain False Positives & False Negatives
In the context of fraud detection:


Prediction / Actual	                  |Not Fraud (0)	                      |Fraud (1)
 
Not Fraud (0)	                        |✅ True Negative	                  |❌ False Negative

Fraud (1)	                            |❌ False Positive	                |✅ True Positive

# ❗ False Positives (FP)
Model predicted fraud, but it was not fraud

E.g., a legit purchase flagged wrongly

Impact: Customer frustration, card gets blocked, bad UX

Acceptable to an extent if you want high recall

# ❗ False Negatives (FN)
Model predicted not fraud, but it was fraud

This is worse!

Fraud goes undetected → financial loss

Must minimize this

🔁 Tradeoff
If you tighten your fraud detection threshold, you'll catch more frauds (↑ recall), but also flag more legit transactions (↓ precision).

If you loosen the threshold, you'll annoy fewer users, but might let fraud slip by.

