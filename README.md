# employee-attrition-analysis

**Introduction**

The purpose of this report is to evaluate the underlying relationships and patterns between and within each of the observed variables in the given dataset. Clustering is used to group the data to better understand the relationships and patterns across groups. Multiple predictive models are used to discover which group of employees is more likely to resign from their jobs, and what factors contribute to it. We choose accuracy and AUC as the evaluation metrics.

**Dataset Description**

Created by IBM data scientists, the dataset contains 1471 employees’ information including demographic, job-specific, and personal factors. It has 35 variables that include both numerical and categorical data. 


The graph shows the importance of variables by random forest model.
<img src="graph/random forest - importance.png" alt="importance" width="700"/>


If use k means to cluster employees to different groups, we choose the number of centers by the total within sum of squares plot, according to the graph, two groups is appropriate. 

<img src="graph/the total within sum of squares plot.png" alt="importance" width="700"/>

-	group 1: employees with less work experience and income
-	group 2: employees with more work experience and higher income








**Conclusion**

For the dataset, logistic regression works best among models without clustering. It has the highest accuracy and AUC. However, we need to consider that the data is imbalanced, it is likely that there are no enough positive samples and models fail to learn from the training set. 

Factors that decrease the likelihood of employees’ attrition are

•	Environment Satisfaction   

•	Job Involvement   

•	Job Satisfaction   

•	Years In Current Role    

•	Relationship Satisfaction 

•	Training Times Last Year   
   
   
Factors that increase the likelihood of employees’ attrition are
 
•	Business Travel Frequently

•	Work over time 

•	Distance From Home  

•	Marital Status Single  

•	Years Since Last Promotion        

