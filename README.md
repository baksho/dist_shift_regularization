The topic of the project is **Covariate Shift Regularization with Kernel Methods**.

## Description
Covariate shift, a fundamental challenge in supervised learning, occurs when the distribution of input features differs between training and test datasets while the conditional distribution of the target given the input remains unchanged. This project explores the challenge of covariate shift through the lens of kernel methods, particularly in the linear regression settings. We analyze theoretical foundations, propose strategies for mitigating covariate shift using importance weighting with weights estimated by kernel density estimation and self-attention mechanisms. We conduct experiments using synthetic data to assess the effect of mean shift on model performance, comparing ordinary least squares and gradient descent estimators. We also explore the roles of different parameters like sample size, learning rate, masking fucntion etc. in mitigating the challenge posed by covariate shift.

## Project Outline
The main goal of this project is to understand the impact of covariate shift on learning algorithms and performance.

- We formally introduce the challenge of covriate shift in the framework of kernel methods.
- We explore different strategies to tackle the challenge introduced by covariate shift.
- We also summarize and present the state of the art, covering current methodologies and researches in this landscape.
- We implement two methods to handle covariat shift in our synthetically generated data using importance weighting: one method using Kernel Density Estimation to estimate the importance weights and another method with self-attention mechanism, where the weights are estimated along with regression parameter using gradient-descent-ascent algorithm instead of predicting it from the available data.
- We compare the method with its corresponding variants of no importance weighting.
- We also compare the algorithms with respect to complexity: choice of learning rate, sample sizes, masking function used in self-attention mechanism etc.

#### References
Below reference were extensive used during this project:
- Francis Bach. *Learning theory from first principles.* MIT press, 2024.
- Davit Gogolashvili, Matteo Zecchin, Motonobu Kanagawa, Marios Kountouris, and Maurizio Filippone. *When is importance weighting correction needed for covariate shift adaptation?* arXiv preprint arXiv:2303.04020, 2023.
- Cong Ma, Reese Pathak, and Martin J Wainwright. *Optimally tackling covariate shift in rkhs-based nonparametric regression.* arXiv preprint arXiv:2205.02986, 2022.
- Mehryar Mohri. *Foundations of machine learning.* MIT press, 2018.
- Hidetoshi Shimodaira. *Improving predictive inference under covariate shift by weighting the log-likelihood function.* Journal of Statistical Planning and Inference 90 (2000) 227-244, 2000.
- Masashi Sugiyama, Matthias Krauledat, and Klaus-Robert Müller. *Covariate Shift Adaptation by ImportanceWeighted Cross Validation.* Journal of Machine Learning Research 1 (2000) 1-48, 2000.

Other references used during this project can be found in the biblipgraphy section of the final report.
