# lead-lag Factor
  尝试对The Leading Premium这篇文章在A股市场的复现，最后效果不好。

## 文献因子解释
  原文是分行业做行业的LL因子，上20%相对于下20%的组合有显著的超额收益率。
  对于个股的operating income growth分别考虑滞后1-4期与领先1-4期与GDP增长率计算相关系数，加权得到

$$
 LL_{t}^{i}=\sum_{j=-J}^{J} \left | \rho_{t,j}^{i} \right | \cdot j  / (\sum_{j=-J}^J  \left | \rho_{t,j}^{i} \right |)
$$

## 因子处理
数据来源于国泰安，
