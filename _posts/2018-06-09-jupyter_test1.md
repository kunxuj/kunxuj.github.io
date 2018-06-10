
# Understanding of TRPO Algorithm
$$L^{CLIP}(\theta) = \hat{\mathbb{E}}_t [\min(r_t(\theta) \hat{A}_t, \text{clip}(r_t(\theta), 1 - \epsilon, 1+\epsilon) \hat{A}_t)]$$



$$\max_{\theta} \quad L_{old}(\theta)  \\
s.t. \quad \bar{D}_{KL}(\theta_{old}, \theta) \leq \delta$$



