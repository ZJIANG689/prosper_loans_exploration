# Prosper_Loan_Data_Exploration

## Dataset

The investigated dataset is from Prosper, the first marketplace lending platform of America. The dataset contains 113,937 loan records with 81 features on each loan record. The recorded features including the loan amount, borrower rate (interest rate), current loan status, borrower income, borrower credit history, borrower employment status, borrower asset information, borrower investment information, and borrower payment information. The main purpose of this project is to summarize the characteristics of variables that can affect the borrower debt pressure, influence the investor's investment decision, and to get some practice about the relationships among multiple variables using summary statistics and data visualizations.
Note: Because the ProsperRating records did not exist prior to July 2009, it shows as missing data in the earlier records. Prior to 2009, the CreditGrade was used as the evaluation system by Prosper. Since we have more ProsperRating over CrediGrade records, the rows with the CrediGrade records will be excluded from this analysis. The additional rows with the conditions below will also be exclude.
1. Missing borrower's income information
2. Borrower rate is higher than 0.35
3. Missing employment status information
4. Credit score lower than 400

## Summary of Findings

In this exploration, I found the Prosper Rating system applied in the Prosper platform reflects the borrower's risks, and it differentiates the borrowers by giving them different borrower rate based on their past financial records. Besides, the Prosper rating system also identifies the borrower's debt pressure, which is consistent with the pattern observed in the income ranges vs. debt to income ratio plot. What is more, the Prosper rating system also help the investors to avoid risk when investing their money. The data shows the investors in general prefer to invest the low risk, low borrower rate loans. For the high borrower rate loans, because of the increased risks, although the rate is attractive but the investors in general prefer to invest in small amount of the loans, mainly aggregates on the USD 4k loan, which is also the loan amount have the highest borrower counts and high borrower rate (0.32). This interesting finding indicates the investors in general are more willing to reduce the risks of their investment.

The other interesting findings include the explanation for the highest counts of the loan amount 4k. The boxplot of the loan amount vs. Prosper rating shows the borrowers with E and HR (indicate these borrowers are high risks and receive high borrower rates) have very narrow box at around loan amount 4k. Such result demonstrate that the E and HR borrowers have been regarded as 'high risks' borrowers in the Prosper rating system, therefore they are limited from borrowing larger loan amount. The result is another evidence of showing how the Prosper system protects the investor.

The borrower rate vs. house owner histogram shows owning house helped to lower the borrower rate. However, a further investigation shows owning house does not to get a better Prosper rating scale.

Other interesting discoveries include most borrowers from California, Texas,  New York, Florida, and Illinois. Most borrowers are employed as professionals. The top reason for borrowing the loan is debt consolidation. In this dataset, most of the borrowers have at least one Prosper loan already when they enter the system. Most of the borrowers prefer three years loan term.

## Key Insights for Presentation

For the presentation, I mainly focus on how accurate the Prosper rating system on differentiating the borrowers and its' effects on the investors' behaviors.

I started by using univariate analysis to get a general idea of the borrowers' background information to understand the possible reasons of why they borrow loans, followed by the bivariate analysis of the different variables associate with the Prosper rating system through clustered barchart, heatmap, boxplot, etc.

After I identified Prosper rating system does correlated with borrowers' debt pressure and influences the investors' investment decisions, I applied multivariate analysis to further investigate how the investors use the Prosper rating system to make their decisions.

## References:
1. https://en.wikipedia.org/wiki/Prosper_Marketplace
2. https://nbviewer.jupyter.org/github/bockjo/Udacity_portfolio/blob/master/EDA_Prosper%20loans%20data%20set.html
3. https://nonusingh.github.io/EDA/
4. https://rstudio-pubs-static.s3.amazonaws.com/284488_195ef48d299e46f5b009987c8b988b69.html
5. https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0
