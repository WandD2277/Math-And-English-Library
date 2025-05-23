## 40.1 欧拉方程 
### 40.1.1 基本概念
##### **定义**： #欧拉方程
> <font color="#ccc1d9">描述：</font>
> 1. 形式：$$x^ny^{(n)}+a_1x^{n-1}y^{(n-1)}+\cdots+a_{n-1}xy^{\prime}+a_ny=f(x)$$

**解释**
+ 概念：
	+ 欧拉方程，同时也是个线性方程，但是是变系数的；
	+ 但它是一种特殊的变系数：一种非常**有规律**的线性变系数方程；
+ 思想：
	+ 把这种规律的变系数方程化成常系数方程；
+ 方法：
	+ 设 $x=e^t$，得到 $x^{k}y^{(k)}=D(D-1)\cdots(D-k+1)y$ 
	+ 其中 $D=\frac{d}{dt}$，$Dy=\frac{dy}{dt}$，$D^{2}=\frac{d^{2}}{dt^{2}}\quad\quad D^{2}y=\frac{d^{2}y}{dt^{2}}$

### 40.1.2 例题
**例题**：求欧拉方程 $x^{2}\frac{d^{2}y}{dx^{2}}+4x\frac{dy}{dx}+2y=0\quad(x>0)$ 的通解；
+ 分析
+ 解析
	+ $x=e^{t}\quad D(p-1)y+4Dy+2y=0$
	+ 得到：$(y^{2}-1)y+4y+2y=0$
	+ 得：$\frac{d^{2}y}{dt^{2}}+3\frac{dy}{dt}+2y=0$ 
+ 题型：#
