# lead-lag Factor
  尝试对The Leading Premium这篇文章在A股市场的复现，最后效果不好。

## 文献因子解释
  原文是分行业做行业的LL因子，行业的产出增长与t期之后的GDP增长相关系数越大，t越大，LL因子越大，上20%相对于下20%的组合有显著的超额收益率。
  对于个股的operating income growth分别考虑滞后1-4期与领先1-4期与GDP增长率计算相关系数，加权得到。

$$
 LL_{t}^{i}=\sum_{j=-J}^{J} \left | \rho_{t,j}^{i} \right | \cdot j  / (\sum_{j=-J}^J  \left | \rho_{t,j}^{i} \right |)
$$

## 因子处理
数据来源于国泰安，对于t期的因子，考虑之前8个季度经营性现金流量净额增长率与中国GDP增长率（未除去通胀）的根据相关系数加权的领先期数，在12个季度的跨度下，对于个股在横截面层面分别考虑分组计算spread和回归的方法，t检验均不显著。

参考文献：Croce M M, Marchuk T, Schlag C. The leading premium[J]. The Review of Financial Studies, 2023, 36(8): 2997-3033.
