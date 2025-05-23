---
title: Lecture 37：常系数齐次线性微分方程
tags:
  - 微分方程
  - 数学
categories: 
date: 2024-02-01
---
---
## 38.1 二阶常系数齐次微分方程
##### **定义**： #二阶常系数齐次微分方程
> <font color="#ccc1d9">描述：</font> 
> 1. 结构： $$y^{\prime\prime}+q +py^{\prime}+qy=0$$
> 2. 特征方程：$$r^2+pr+q=0$$

**解释**
+ 常系数与变系数：
	+ 概念：
		+ 未知函数的系数，如果是常数的，就是常系数方程，否则就是变系数的（比如系数当中有 $p(x)$ 的）
	+ 常系数：
		+ 结构：
			+ $y^n+py^{\prime}+qy=0$
	+ 变系数：
		+ 结构：
			+ $y^n+p(x)y^{\prime}+q(x)y=0$
		+ 解释：
			+ 通解 $y=C_1y_1(x)+C_2y_2(x)$
			+ $y_1$ 和 $y_2$ 是线性无关的；
			+ $y_1/y_2$ 不等于常数；
+ 特征方程： 
	+ 概念：
		+ 特征方程的根和微分方程的解息息相关； 
	+ 若是三阶方程的单实根 $r_1$
		+ 通解： $y=C_1e^{r_1x}$
	+ 若是不等实根 $r_1\neq r_2$
		+ 通解： $y=C_1e^{r_1x}+C_2e^{r_2x}$
	+ 若是相等实根 $r_{1}=r_{2}=r$
		+ 通解：$y=e^{rx}(C_1+C_2x)$
	+ 若是共轭复根 $r_{1,2}=\alpha\pm i\beta$
		+ 通解：$y=e^{\alpha x}(C_1\cos\beta x+C_2\sin\beta x)$
	+ 注意：
		+ 以上通解都是针对二阶的情况；
+ 三阶：
	+ 方法：
		+ 根据根的类型，对每个根使用二阶时的求不同实根的方法，然后将它们相加；
	+ 举例：$r^{3}-2r^{2}+r-2=0$ 时
		+ 求特征方程：$r_1=2,r_{1,2}=\pm i$
		+ 解 = 单实根 + 共轭复根 = $y=C_{1}e^{2x}+ C_{2}\cos x+C_{3}\sin x$

**方法**
+ 第一步：写特征方程
+ 第二步：找出特征根
+ 第三步，根据根的方程，写出对应式子
	+ 若是不等实根 
		+ 通解： $y=C_1e^{r_1x}+C_2e^{r_2x}$
	+ 若是相等实根 
		+ 通解：$y=e^{rx}(C_1+C_2x)$
	+ 若是共轭复根 
		+ 通解：$y=e^{\alpha x}(C_1\cos\beta x+C_2\sin\beta x)$
