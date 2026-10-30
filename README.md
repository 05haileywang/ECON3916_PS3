# ECON3916_PS3

The increase in average West revenue from 808 to 1,236 dollars is not a reflection of the true improvement in customer performance. It is due to the customer table being joined to the order table before the average was calculated. This results in customers with multiple orders appearing multiple times, which will give their revenue disproportionate weight in the average revenue calculation. The customer average of 808 dollars is the appropriate figure given the question we are trying to answer.

Missing data creates a large risk to the accurate reporting of data. A simple filter, like region != 'West' will not include customers with NULL regions, even though they are not actually West customers either. This missing data and incorrect filtering would exclude 434 customers from the analysis. Future analysis should always consider the steps on how to handle missing regions.

The program evaluation demonstrates the importance of choosing the correct controls when comparing data. The naive estimated program effect was $263.08, compared with a true simulated effect of $30. After we controlled for account size, the estimate fell to $30.84. By adding support tickets as a control, we introduced collider bias in our analysis and produced a biased negative estimate.

Before reporting results to upper leadership, I would double-check the raw data, refine the procedures based on the question we are trying to solve, identify how to handle NULL values, and select control variables based on causal relationships.
