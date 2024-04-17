# S-mbolos-matem-ticos

To estimate the parameters of the model, we adapt an algorithm proposed by Anderson (1973). The log-likelihood for the linear spatial t-Student model is given by:

[ \mathcal{L}(\theta) = \log(K_n(\eta)) - \frac{1}{2} \log(|\Sigma|) - \frac{1}{2\eta} (1 + n\eta) \log(1 + c(\eta) \delta) \quad (4.4) ]

where:

(\log(K(n)) = \log \Gamma(2\eta) - \log \Gamma(8(\chi\beta)))
(c(\eta) = \frac{\eta}{1 - 2\eta}), with (0 < \eta < \frac{1}{2})
As noted by Zellner (1976), the log-likelihood function (4.4) is a decreasing function of (n), so it cannot be estimated by maximum likelihood. See also De Bastiani et al. (2015).

The score functions for the linear spatial t-Student model are provided by:

[ U_{\theta}(\theta) = (U_{\beta}^T, U_{\phi}T)T ]

where:

(U = \frac{2L(0)}{23} = (\delta)XT\Sigma{-1})
(U_2 = \frac{8L(0)}{84}), and the j-th element of (U_{\phi}) is given by:
[ U_{\phi_j} = \frac{8L(0)}{8} = -\left(\frac{2 - 1}{(0.2/0.3)}\right) + \frac{1}{2} \left(\frac{8 - (82/83)}{2}\right)^{-16} \quad \text{for } i = 1, 2 ]

Here, (w(6) = (1+m)(10)) and (\zeta) represents the Digamma function. In this article, (\Sigma = \phi_1 I_n + \phi_2 R), where (\phi_1 = I_n) and (\phi_2 = R). Given (\eta), the log-likelihood function (4.4) is maximized at:

[ \hat{\beta} = (XT\Sigma{-1}X){-1}XT\Sigma^{-1}Y ]

And from (U_{\phi} = 0), we have:

[ \begin{align*}

& \Phi_1 \operatorname{tr}(\Sigma{-1}\Sigma{-1}) + \phi_2 \operatorname{tr}(\Sigma{-1}R\Sigma{-1}) = w(\delta) \epsilonT\Sigma{-1}\Sigma^{-1}\epsilon \
& \phi_1 \operatorname{tr}(\Sigma{-1}R\Sigma{-1}) + \phi_2 \operatorname{tr}(\Sigma{-1}R\Sigma{-1}R) = w(\delta) \epsilonT\Sigma{-1}R\Sigma^{-1}\epsilon \end{align*} ]
These equations (i) and (ii) can be written as (A\phi = b), where:

[ A = \begin{bmatrix} a_{11} & a_{12} \ a_{12} & a_{22} \end{bmatrix} \quad b = \begin{bmatrix} b_1 \ b_2 \end{bmatrix} \quad \phi = \begin{bmatrix} \phi_1 \ \phi_2 \end{bmatrix} ]

with:

(a_{11} = \operatorname{tr}(\Sigma{-1}\Sigma{-1}))
(a_{12} = \operatorname{tr}(\Sigma{-1}R\Sigma{-1}))
(a_{22} = \operatorname{tr}(\Sigma{-1}R\Sigma{-1}R))
(b_1 = w(\delta) \epsilonT\Sigma{-1}\Sigma^{-1}\epsilon)
(b_2 = w(\delta) \epsilonT\Sigma{-1}R\Sigma^{-1}\epsilon)
This suggests the following iterative process to estimate the parameter vectors (\beta) and (\phi):

Step 1: Given an estimator at the (k)-th iteration, calculate (w(\delta^{(k)})

