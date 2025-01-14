**PORTFOLIO OPTIMIZATION**

Portfolio optimization aims to allocate assets in a portfolio to achieve a balance between risk and return. A common technique for this is minimizing portfolio variance while maximizing expected utility, grounded in modern portfolio theory introduced by Harry Markowitz.

The code for this activity is based on two main data descriptors: Variance and expectation. This activity is designed for course: MA2012 	Statistics Fundamentals.

### Variance Minimization and Utility Maximization
1. **Minimizing Variability (Risk)**: Variability is quantified using the portfolio's variance, calculated as:

   $$\sigma_p^2 = \mathbf{w}^\top \Sigma \mathbf{w}$$
   
   where $\mathbf{w}$ is the weight vector of asset allocations, and $\Sigma$ is the covariance matrix of asset returns. Minimizing $\sigma_p^2$ leads to reduced portfolio risk.

3. **Maximizing Expected Utility**: Utility functions quantify investor satisfaction. A common approach is to maximize the expected utility of portfolio returns:
   
   $$U(\mathbf{w}) = \mathbb{E}[R_p] - \frac{\lambda}{2} \sigma_p^2$$
   
   Here, $\mathbb{E}[R_p]$ is the expected return, $\lambda > 0$ is the risk-aversion coefficient, and $\sigma_p^2$ is the portfolio variance. Investors with higher risk aversion $(\lambda\)$ prioritize lower risk over higher returns.

### Relation to Markowitz Theory
Markowitz's theory proposes that portfolios should be optimized based on the trade-off between expected return and risk. This leads to the **efficient frontier**, a set of portfolios with the highest return for a given level of risk. The theory underpins the optimization process:
1. **Input Estimation**: Estimate expected returns $\mathbb{E}[R]$ and covariance $\Sigma$ of asset returns.
2. **Objective**: Solve for $\mathbf{w}$ to maximize utility while minimizing variance.
3. **Constraints**: Ensure practical allocations, such as $\sum w_i = 1$ (portfolio weights sum to 1) and $w_i \geq 0$ (no short-selling if restricted).
