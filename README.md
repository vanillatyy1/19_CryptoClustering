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
To mitigate FutureWarnings and UserWarnings, I first attempted the following, and the code works the 1st time. But when I tried to run it again it does not work.

"""
    # import os
    # os.environ["OMP_NUM_THREADS"] = "1"

    # import warnings

    # Suppress the warning
        # There is a warning related to a known issue with KMeans in scikit-learn 
        # when using Windows with MKL (Intel's Math Kernel Library). 
        # It's a memory leak warning that occurs when there are fewer chunks than available threads.
        # An attempt was made to write code "import import os os.environ["OMP_NUM_THREADS"] = "1"", but
        # warning persists. An additional attempt to use "import warnings" and calls to filterwarnings() to supress the warning.
        # Resources: https://docs.python.org/3/library/warnings.html

        # warnings.filterwarnings("ignore", category=UserWarning, message="UserWarning: KMeans is known to have a memory leak on Windows with MKL, when there are less chunks than available threads. You can avoid it by setting the environment variable OMP_NUM_THREADS=1.*")
"""

But with the help of my tutor, I added the following code in the beginning and it successfully suppressed the warnings.

"""
    import warnings
    warnings.filterwarnings("ignore")
"""
