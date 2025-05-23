## 1.1 可降阶方程概念
**高阶方程降阶核心**
+ 核心：
	+ 大部分是不可以降阶的，在 1.2 小节当中的大部分只是理论上有解，但没有通用方法求解；
	+ 可以用通用方法降阶、求解的两种类型：$y^{\prime\prime}=f(x,y^{\prime})$ 和 $y"=f(y,y^{\prime})$
	+ 判断所属的可降阶类型，进行对应的代换，然后使用**分离变量法**；
+ 注意：
	+ 求高阶微分  方程定解时，每出来一个常数 `C`，就定一个常数；

**常见可降阶形式**
+ 1. $y^{\prime\prime}=f(x)$；
	+ 举例：$y^{\prime\prime}=e^{x},\quad y^{\prime}=e^{x}+e_{1}\quad y=e^{x}+C_{1}x+C_{2}$
+ 2. $y^{\prime\prime}=f(x,y^{\prime})$
	+ 方法：
		+ 令： ${y^{\prime}=P,y^{\prime\prime}=\frac{dP}{dx}}$
		+ 得到： $\frac{dp}{dx}=f(x,p)$ 关于 p、x 的一阶方程，然后进行分离变量；
	+ 举例：
		+ $\text{微分方程 }xy^{\prime\prime}+3y^{\prime}=0\text{ 的通解为}$
		+ 没有直接出现 y，所以为第二种方法；
		+ 得到：$y^{\prime}=p,y^{\prime\prime}=\frac{dp}{dx},x\frac{dp}{dx}+3p=0$ 此方程为一阶可分离方程； 
+ 3. $y"=f(y,y^{\prime})$
	+ 方法：
		+ 设： $y^{\prime}=P$、$y^{\prime\prime}=\frac{dp}{dy}P$；
		+ 变成只有 y、p，没有 x 的一阶方程，然后使用分离变量法；

## 1.2 高阶线性微分方程
**总结**
+ 高阶线性微分方程； 
	+ 包括： 
		+ 高阶线性齐次微分方程； 
		+ 高阶线性非齐次微分方程；
	+ 特点：
		+ 理论上有解，但是都没有通用的求解方法；
+ 可以解的情况：
	+ 常系数齐次线性微分方程；

**解的结构**
+ 二阶线性齐次微分方程：
	+ $$y^{\prime\prime}+p(x)y^{\prime}+q(x)y=0$$
+ 二阶线性非齐次微分方程：
	+ $$y^{\prime\prime}+p(x)y^{\prime}+q(x)y=f(x)$$

##### **定理**： #二阶线性齐次微分方程的解
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font>如果以 $y_1(x)$ 和 $y_2(x)$ 是二阶线性齐次微分方程的两个线性无关的的特解，那么：$$y=C_{1}y_{1}(x)+C_{2}y_{2}(x)$$
> 是二阶线性齐次微分方程的通解；

**解释**
+ 独立微分方程的个数和阶数一致；

**判断线性无关**
+ 如果 $\frac{y_{1}(x)}{y_{2}(x)}$ 不等于 C，则线性无关；

##### **定理**： #二阶线性非齐次微分方程的解
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font>如果 $y^*$ 是二阶线性**非齐次**微分方程的一个特解，$y_1(x)$ 和 $y_2(x)$ 是二阶线性**齐次**微分方程的两个线性无关的特解，则：
> $$y=C_{1}y_{1}(x)+C_{2}y_{2}(x)+y^{*}(x)$$
> 是非齐次微分方程的通解；

**解释**
+ $$齐次通解+非齐次特解=非齐次通解$$

##### **定理**： #非齐次微分方程与齐次微分方程的解
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font>如果 $y^*_1(x)$ 和 $y^*_2(x)$ 是非齐次微分方程的两个特解，则 $y(x)=$ $y^*_1(x)$ + $y^*_2(x)$  是**齐次**微分方程的解；

##### **定理**： #非齐次微分方程的解关于非齐次项的叠加性
> <font color="#8db3e2"><font color="#c6d9f0">描述：</font></font>如果 $y^*_1(x)$ 和 $y^*_2(x)$ 分别是方程 $y^{\prime\prime}+p(x)y^{\prime}+q(x)y=f_{1}(x)\quad\quad y^{\prime\prime}+p(x)y^{\prime}+q(x)y=f_{2}(x)$ 的特解，则：
> $$\dot{y_1}(x)+\dot{y_2}(x)$$ 是方程 $y^{\prime\prime}+p(x)y^{\prime}+q(x)y=f_1(x)+f_2(x)$ 的一个特解；
