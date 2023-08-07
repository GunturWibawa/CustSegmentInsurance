# CustSegmentInsurance

Customer Segmentation in Sure Tomorrow Insurance Company

The project assigned to me during the eleventh sprint involves Linear Algebra.

Throughout this sprint, I explored fundamental concepts such as vectors, matrices, and linear regression.

# **Project Insight**

The insurance company "Sure Tomorrow" is manage to address specific challenges through the application of machine learning. I assigned to assess the viability of these efforts.

**Objective 1: Identify clients that correspond to a specific set of criteria to facilitate the company's marketing initiatives.**

To accomplish this, I utilized the k-Nearest Neighbors (kNN) algorithm. Upon examination, I observed that unscaled data yields relatively similar neighboring data up to index 5, whereas scaled data did up to index 3. Consequently, it can be concluded that although unscaled data in the kNN algorithm produces more analogous index, I would advocate the use of scaled data to minimize the potential arbitrary sequencing of neighboring data index due to identical distance values.

**Objective 2: Forecast the probability of a new client filing an insurance claim and ensure if the predictive model outperforms the baseline prediction model.**

I employed the F1 score as a metric to evaluate this model, as the company is keen to prevent elevated instances of:

- FP (False Positives): Clients who will not receive insurance benefits but are predicted to do so, thereby decreasing the company's profits.
- FN (False Negatives): Clients who are eligible for benefits but are incorrectly forecasted not to, leading to escalated company expenditures.

The analysis of the machine learning training revealed that the model's performance is enhanced when trained on scaled data. Intriguingly, scaling the data yielded a FN score of zero, signifying the model's ability to precisely predict the beneficiaries, thus safeguarding the company from losses incurred by misallocation of benefits.

**Objective 3: Safeguard clients' private information without undermining the models developed in the previous objectives.**

In this section, I executed data masking to preserve customer information by forming a random square matrix possessing the same quantity of columns and rows as the original matrix. The original matrix remains retrievable through the application of the inverse matrix of the masking matrix post-transformation.

In summary, the project resulted in the following insights:

1. Scaling numerical data enhances the ability to predict specific numerical values with greater precision, even beyond the decimal point. This proves highly valuable in identifying clusters of data.
2. The metric for evaluating a model should be selected wisely, reflecting the risks or negative consequences that the model building process aims to evade.
3. Data obfuscation methodologies can be effectively deployed to safeguard private and sensitive information without impairing the model's evaluation metrics.
