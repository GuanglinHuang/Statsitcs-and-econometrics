# [h]igher-[o]rder multi-cumulant [f]actor [a]nalysis

This R package implements several factor analysis approaches based on the covariance matrix and the higher-order multi-cumulants, including factor number selection, factor estimation and the applications in financial market.

Installing the developer version of the package is possible by
```
devtools::install_github("GuanglinHuang/hofa")
```

**Update log:**

Changes in version 0.9.1
 - unit tests for M2.mle, M2.pca, M2.gmm, M3.gmm, M3.als, M4.als, Portfolio.IC and 
 Portfolio.PC functions.
 - remove M4.gmm functions, leave it as a future work.
 - fix bugs in M2.gmm and M3.gmm functions.
 
 
Changes in version 0.9.0
 - speed up CUM function by C++.
 - more unit tests of functions.R.
 - unit tests for M2.select, M3.select and M4.select.
 - small revision in the description of examples.
 
Changes in version 0.8.9
 - add Portfolio.PC function, implement Lassance and Vrins (2020)'s PC portfolio.
 - speed up Bai and Li (2012)'s Maximum Likelihood Estimation by C++. The related functions: M2.gmm, M3.gmm, M4.gmm and M2.mle are revised.
 
Changes in version 0.8.8
 - add Portfolio.IC function, implement Lassance and Vrins (2020)'s IC portfolio.
 - fix bugs in functions.R.

Changes in version 0.8.7
 - add M4.gmm function, using fourth-order moment for Generalized Moment Method in Fan and Zhong(2018), still in processing.
 - fix bugs in M2.gmm, M2.mle and M2.pca functions.
 
Changes in version 0.8.6
 - small revision in M2.gmm and M3.gmm functions.
 
Changes in version 0.8.5
 - small revision in M2.gmm function.
 - add M3.gmm function, using third-order moment for Generalized Moment Method in Fan and Zhong(2018).
 
Changes in version 0.8.4
 - Add M2.gmm function to estimate the factors and factor loadings by Generalized Moment Method in Fan and Zhong(2018).
 - Update the descriptions of M2.pca, M2.mle, M3.als and M4.als functions.
 - fix a small bug in M2.pca function.
 
Changes in version 0.8.3
 - Remove hofa.als function.
 - Add M3.als function to estimate the factors and factor loadings based on the third-order cumulant alternating least square algorithm.
 - Add M4.als function to estimate the factors and factor loadings based on the fourth-order cumulant alternating least square algorithm.
 
Changes in version 0.8.2
 - Remove M2.est function.
 - Add M2.mle function to estimate the factors based on the covariance by using maximum likelihood methods in Bai and Li(2012,2013).
 - Add M2.pca function to estimate the factors by using principal component analysis (Bai,2003; Fan et al.,2016). 
 
Changes in version 0.8.1
 - Add M2.est function to estimate the factors based on the covariance or correlation matrix. Maximum Likelihood methods in Bai and Li(2012,2013) are available now. This function still works in progress.

Changes in version 0.8.0
 - Remove GER.sel function.
 - Add M2.select function to determine the number of factors based on the second-order moment matrix.
 - Implement Bai and Ng(2002)'s IC3, PC3 and BIC3 estimators in M2.select.
 - Implement Onatski(2010)'s ON estimator in M2.select.
 - Implement Ahn and Horenstein(2013)'s GR and ER estimators in M2.select.
 - Implement Fan et al.(2020)'s ACT estimator in M2.select.
 - Add M3.select and M4.select function to determine the number of factors based on the higher-order moment tensor.
 - Better user parameter setting in M3.select and M4.select functions.
