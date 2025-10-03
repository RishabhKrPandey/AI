# Customer Segmentation with Clustering 


**Project Objective:** To identify distinct groups of customers within a mall's dataset. By segmenting customers based on multiple dimensions (income, age, spending habits), we can provide rich, actionable insights to the marketing team for highly targeted campaigns.

<img width="1259" height="317" alt="image" src="https://github.com/user-attachments/assets/dcf3c5db-8854-41cc-bf6b-0c2e2a8503fe" />

### Feature Distribution
<img width="1314" height="435" alt="image" src="https://github.com/user-attachments/assets/b7da4fb9-871a-4170-9fc3-41e9e2798cae" />

#### Insights :-
1. The younger segment of customers are mainly comprised of females
2. The annual income of males are slightly higher, Females have a very tight income band. There are a few outliers in males suggesting ultra rich males.;
3. Spendind score of females are much higher than males, indicating they are more engaged in shopping than males
4. Younger segment -> Females, Rich segment -> Males, More spending segment -> Females

### Bivariate Analysis 
<img width="955" height="715" alt="image" src="https://github.com/user-attachments/assets/866389b7-1abb-4685-aabb-b5029582d8c4" />

**CRITICAL INSIGHT from Pair Plot:**
- The **`Annual Income` vs. `Spending Score`** plot is the most revealing. It clearly shows distinct, blob-like groups, making it the perfect candidate for clustering.
- The **`Age` vs. `Spending Score`** plot shows some patterns but they are less defined. We see a concentration of high-spending customers in the younger age brackets.
- `Gender` does not appear to be a strong separating factor in any of these plots, as the distributions for males and females largely overlap.

## Segmentation Model 1 - Income & Spending Score

<img width="920" height="494" alt="image" src="https://github.com/user-attachments/assets/4156b54b-e346-47b2-b940-b0a570df5596" />
<img width="963" height="622" alt="image" src="https://github.com/user-attachments/assets/9d30aa0c-5281-4e23-a617-4254d0223cad" />

####  Income-Based Personas and Strategy
Using the quantitative profiles, we can define our segments:
- **Cluster 3 (Careful High-Earners):** High income (88k) but low spending (17). Cautious, value-driven buyers.
- **Cluster 0 (Standard):** Average income (55k) and spending (50). This is the largest, core customer group.
- **Cluster 4 (Budget Shoppers):** Low income (26k) and low spending (21). Highly price-sensitive.
- **Cluster 1 (Target - High Value):** High income (87k) and high spending (82). The mall's prime target.
- **Cluster 2 (Enthusiasts):** Low income (26k) but high spending (79). Likely young, trend-focused shoppers.


## Segment model 2 :- Age vs Spending score
<img width="933" height="507" alt="image" src="https://github.com/user-attachments/assets/04996bd7-ad7f-4ff9-bab8-9db96e911fbd" />
<img width="938" height="614" alt="image" src="https://github.com/user-attachments/assets/371f1dd6-c818-4e35-a2c5-78f4050aa2d7" />

####  Interpreting the Age-Based Segments
- **Young Average-Spenders:** Customers under 40 with low-to-moderate spending.
- **Young High-Spenders:** A clear group of customers under 40 with high spending scores.
- **Older Low-Spenders:** A small group of older customers with very low spending scores.
- **Older Average-Spenders:** Customers over 40 with moderate spending scores.



## Hierarchical Clustering( Dendrograms)
<img width="937" height="485" alt="image" src="https://github.com/user-attachments/assets/d4659d60-c49f-4b9d-8ba8-7b1bea0bb342" />


## Conclusion

In this project, we successfully applied unsupervised machine learning to perform customer segmentation.

**Key Steps Undertaken:**
1.  **Performed an in-depth EDA:** Used 2D and 3D plots to explore customer data from multiple angles.
2.  **Built two distinct segmentation models:** Created an income-based model and an age-based model, showing that segmentation is not a one-size-fits-all process.
3.  **Used the Elbow Method** to programmatically determine the optimal number of clusters for each scenario.
4.  **Used Hierarchical Clustering** as an alternative method and used its dendrogram to validate our choice of `k`.
5.  **Created quantitative, data-driven personas** for each segment, providing the marketing team with precise, actionable insights for targeted campaigns.

