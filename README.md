# Hello_World
This is the first MD I tried. 
Does markdown on GitHub work just like RMarkdown? 
Test

## 1 
For $n_1+n_2$ samples the likelihood is 
$$L(\textbf{x}, \mu_1, \mu_2, \Sigma) = \frac{1}{(2 \pi)^{\frac{n_1 + n_2}{2} p} | \Sigma |^{\frac{n_1 + n_2}{2}}}
e^{- \overset{n_1}{\underset{i = 1}{\Sigma}} (x_i - \mu)' \Sigma^{- 1} (x_i -
\mu) / 2 - \overset{n_2}{\underset{j = 1}{\Sigma}} (x_j - \mu)' \Sigma^{- 1}
(x_j - \mu)}$$
\[ log L = {tr} \left[ \Sigma^{- 1} \left( \overset{}{\underset{i =
   1}{\overset{n_1}{\Sigma}} (x_i - \bar{x}) (x_i - \bar{x})'} +
   \overset{}{\underset{i = 1}{\overset{n_2}{\Sigma}} (x_i - \bar{x}) (x_i -
   \bar{x})'} \right) + n (\bar{x} - \mu) (\bar{x} - \mu)' \right] \]
\[ = {tr} \left[ \Sigma^{- 1} \left( \overset{}{\underset{i =
   1}{\overset{n_1}{\Sigma}} (x_i - \bar{x}) (x_i - \bar{x})'} +
   \overset{}{\underset{i = 1}{\overset{n_2}{\Sigma}} (x_i - \bar{x}) (x_i -
   \bar{x})'} \right) \right] + n_1 (\bar{x} - \mu_1)' \Sigma^{- 1} (\bar{x} -
   \mu_1) + n_2 (\bar{x} - \mu_2)' \Sigma^{- 1} (\bar{x} -
   \mu_2) \]
   To minimize it, since $n (\bar{x} - \mu)' \Sigma^{- 1} (\bar{x} -
   \mu)$ is symmetric non-negative definitive matrix, we can conclude when $$ \hat{\mu_1} = \bar{x_1}, \hat{\mu_1} = \bar{x_1}$$ that it would be shrunken. Then, according to \textit{Res 4.10}, that
\[ \frac{e^{- {tr} (\Sigma^{- 1} \mathbf{B}) / 2}}{| \Sigma |^b}
   \leqslant \frac{(2 b)^{p b} e^{- b p}}{| \mathbf{B} |^b} \]
in and only if $\Sigma = \frac{\mathbf{B}}{2 b}$ should the equation hold.  Then we denote $b = \dfrac{n_1+n_2}{2}$ and $\textbf{B} = (n_1 - 1 )S_1^2 + (n_2-1 )S_2^2$.
Thus $$\hat{\mu_1} = \bar{x_1} $$, $$\hat{\mu_2} =\bar{x_2} $$, $$\hat{\Sigma}= \dfrac{n_1+n_2 -2}{n_1+n_2} {\textbf{S}}_{pooled}
$$. 
