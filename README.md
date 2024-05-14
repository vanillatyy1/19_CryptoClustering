# 19_CryptoClustering

## 1) Executive Summary:
The CryptoClustering project aims to analyze cryptocurrency market data using clustering techniques to identify patterns and group similar cryptocurrencies together.

By applying machine learning algorithms, particularly KMeans clustering, the project provides insights into the behavior and categorization of various cryptocurrencies based on market performance metrics.

## 2) Project Objectives:
- Utilize KMeans clustering to group cryptocurrencies based on market performance metrics such as price change percentages over different time intervals
- Apply Principal Component Analysis (PCA) for dimensionality reduction and visualization of the cryptocurrency dataset
- Evaluate the effectiveness of clustering techniques in identifying meaningful patterns and relationships within the cryptocurrency market

## 3) Resource Requirements:
- Technologies: Jupyter Notebook, Python and relevant libraries Pandas, hvplot.pandas, Scikit-learn

## 4) Takeaways:
- Understand the process of clustering analysis and its application in identifying patterns within complex datasets
- Addressed FutureWarnings and UserWarnings, acquiring the ability to mitigate them

## 5) Notes to Central Grader:
Initially, attempts were made to address FutureWarnings and UserWarnings by setting the environment variable OMP_NUM_THREADS to "1". Although this approach worked initially, it did not provide a long-term solution.

After consulting with my tutor, we implemented the following code at the beginning of the script, which successfully suppressed the warnings:

```
    import warnings
    warnings.filterwarnings("ignore")
```
This solution effectively mitigated the warnings and ensured smooth execution of the code.

