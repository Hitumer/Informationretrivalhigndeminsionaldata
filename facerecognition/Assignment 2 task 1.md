Assignment 2

Task 1

1) Denote $\hat{\boldsymbol{s}}$ by $\hat {\boldsymbol{s}} = (s_1, s_2, \dots, s_p)^T$, with $s_1^2+\dots + s_p^2 = 1$.  

$\boldsymbol{s}^T \boldsymbol{\Sigma}\boldsymbol{\Sigma}^T \boldsymbol{s} = ||\boldsymbol{\Sigma}\boldsymbol{s}||^2 = \sigma_1^2s_1^2 + \dots +\sigma_p^2s_p^2 \leq max(\sigma_i^2)\Sigma{s_i^2} = \sigma_1^2$, 
with equality when $s_1 = 1, s_2 = \dots = s_p = 0$. 

So we get the expected $\hat {\boldsymbol{s}} = (1, 0, \dots, 0)^T$. 



2) Denote $\boldsymbol{U}$ by $\boldsymbol{U}= (\boldsymbol{u}_1, \dots, \boldsymbol{u}_p)$

Denote $\boldsymbol{a}$ by $\boldsymbol{a} = \alpha_1\boldsymbol{u}_1 + \dots + \alpha_p\boldsymbol{u}_p $
Because $\boldsymbol{U}^T\boldsymbol{U} = \boldsymbol{I}$, we have $ ||\boldsymbol{a}|| = \alpha_1||\boldsymbol{u}_1|| + \dots + \alpha_p||\boldsymbol{u}_p|| = 1, (\alpha_1 + \dots + \alpha_p = 1)$

We want to maximize $\boldsymbol{a}^T \boldsymbol{X}\boldsymbol{X}^T \boldsymbol{a} = \boldsymbol{a}^T\boldsymbol{U}\boldsymbol{\Sigma}\boldsymbol{V}^T\boldsymbol{V}\boldsymbol{\Sigma}^T\boldsymbol{U}^T\boldsymbol{a} = \boldsymbol{a}^T\boldsymbol{U}\boldsymbol{\Sigma}\boldsymbol{\Sigma}^T\boldsymbol{U}^T\boldsymbol{a}$. From the result of 1), we know that $\boldsymbol{U}^T\boldsymbol{a}= \hat {\boldsymbol{s}} = (1,0,\dots, 0)^T$, i.e. 

$\begin{pmatrix}
\boldsymbol{u}_1^T \\
\vdots \\\
\boldsymbol{u}_p^T\\\
\end{pmatrix} \cdot ( \alpha_1\boldsymbol{u}_1 + \dots + \alpha_p\boldsymbol{u}_p) =  (\alpha_1||\boldsymbol{u}_1||,  \dots , \alpha_p||\boldsymbol{u}_p||)^T = (1,0,\dots, 0)^T$

So $\alpha_1 = 1, \alpha_2 = \dots = \alpha_p =0 \implies \boldsymbol{a}=\boldsymbol{u}_1$. 

