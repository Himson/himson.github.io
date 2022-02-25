---
title: 无线感知CSI相位校准
date: 2022-02-25 09:33:45
tags: Wireless sensing
---
# 无线感知CSI相位校准：从理论到系统实践
我想到哪写到哪。毕竟只是个人博客。
## 理论
### 一，由傅里叶变换得到的常识
CSI, channel state information是对信道频响（Channel frequency response）的离散采样。它是带限的(band-limited)。由于采样定理，带宽决定了CSI的时间上对多径的分辨率。假设一个“完美”系统。只有一条无线传播路径，比如是Line-of-sight path。根据傅里叶变换，CSI的幅度是一个常数。相位则会随着子载波发生线性的相位翻转，翻转的斜率是由系统的sampling timing offset(SFO)决定的。而如果场景是多径，我们可以观察到CSI在幅度和相位上存在频率选择性。又由于CSI是CFR的离散采样，CSI的频点上的间隔决定了时间上的不模糊(unambigious)范围。

### 二，那些不完美的因素
实际系统是复杂的。有如下因素会带来CSI相位的误差
1. Carrier frequency offset
2. PLL frequency offset
3. Sampling frequency offset

待更
