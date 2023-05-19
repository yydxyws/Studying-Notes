# 热统前置基础

## 理论物理前置

### 广义参量与Lagrange方程

### Hamilton正则方程与相空间

### 电磁场

### 电磁场中带电粒子的L和H

### 场的波动性

## 有用的数学

### 阶乘积分

- 

$$
\begin{align} &n!=\int_{0}^{\infty}x^ne^{-x}dx=\Gamma(n+1)
\\&\Gamma(n+1)=n\Gamma(n),例如\Gamma(3)=\Gamma(2+1)=2\Gamma(2)=2
\\\\&\Gamma(-\frac{3}{2})=\frac{4\sqrt{\pi}}{3}，\Gamma(\frac{1}{2})=\sqrt{\pi}，
\\&\Gamma(-\frac{1}{2})=-2\sqrt{\pi}，\Gamma(1)=\Gamma(2)=1
\end{align}
$$

### 高斯积分

- 

$$
\begin{align} &高斯函数为形式为e^{-\alpha x^2}的偶函数
\\&\int_{-\infty}^{\infty}e^{-\alpha x^2}dx=\sqrt{\frac{\pi}{\alpha}}，
\int_{0}^{\infty}e^{-\alpha x^2}dx=\frac{1}{2}\sqrt{\frac{\pi}{\alpha}}
\\&方程两边对\alpha微分，\int_{-\infty}^{\infty}x^2e^{-\alpha x^2}dx=\frac{1}{2}\sqrt{\frac{\pi}{\alpha^3}}
\\&方程两边对\alpha微分,\int_{-\infty}^{\infty}x^4e^{-\alpha x^2}dx=\frac{3}{4}\sqrt{\frac{\pi}{\alpha^5}}
\\&一般公式：\int_{-\infty}^{\infty}x^{2n}e^{-\alpha x^2}dx=\frac{(2n)!}{n!2^{2n}}\sqrt{\frac{\pi}{\alpha^{2n+1}}}
\\&对x^{2n+1}e^{-\alpha x^2}在0\sim \infty积分：\int_{0}^{\infty}xe^{-\alpha x}dx=\frac{1}{2\alpha}
\\&一般公式：\int_{0}^{\infty}x^{2n+1}e^{-\alpha x^2}dx=\frac{n!}{2\alpha^{n+1}}
\end{align}
$$

### 斯特林公式

- 

$$
\begin{align} &n!\sim \sqrt{2\pi n}\big(\frac{n}{e}\big)^n

\\&\ln n!\approx n\ln n -n+\frac{1}{2}\ln(2\pi n)
\\&\ln n!\approx n\ln n -n，n\gg 1
\end{align}
$$

### 黎曼函数

- 

$$
\begin{align} &黎曼函数：\zeta(s)=\sum_{n=1}^{\infty}\frac{1}{n^s},s=1发散，s>1收敛
\\&\zeta(2)=\frac{\pi^2}{6},\zeta(4)=\frac{\pi^4}{90},\zeta(6)=\frac{\pi^6}{945}
\\&玻色积分：I_B(n)=\int_{0}^{\infty} dx\frac{x^n}{e^x-1}=\zeta(n+1)\Gamma(n+1)
\\&\qquad\bigg(=\int_{0}^{\infty} dx\frac{x^ne^{-x}}{1-e^{-x}}=\int_{0}^{\infty}dxx^n\sum_{k=0}^{\infty} e^{-(k+1)x}=\sum_{k=0}^{\infty} \frac{1}{(k+1)^{n+1}} \int_{0}^{\infty} dy y^ne^{-y}\bigg)
\\&\int_0^\infty \frac{x^3 dx}{e^x-1}=\zeta(4)\Gamma(4)=\frac{\pi^4}{15}
\\&特殊积分：I=\int_{0}^{\infty} dx\frac{x^{n-1}}{e^{ax}-1}=\frac{1}{a^n} \int_{0}^{\infty} dy\frac{y^{n-1}}{e^{y}-1}=\frac{1}{a_n}\zeta(n)\Gamma(n)
\\&\frac{dI}{da}=-\int_{0}^{\infty} dx\frac{x^{n}e^{ax}}{(e^{ax}-1)^2}=-\frac{n}{a^{n+1}} \int_{0}^{\infty} dy\frac{y^{n-1}}{e^{y}-1}
\\&令a=1,有\int_{0}^{\infty} dx\frac{x^{n}e^{x}}{(e^{x}-1)^2}=n\zeta(n)\Gamma(n)

\end{align}
$$

### 多对数函数

- 

$$
\begin{align} &多对数函数（容基埃函数）:常用于求解玻色/费米分布的积分
\\&Li_n(z)=\sum_{k=1}^{\infty}\frac{z^k}{k^n},z位于复平面开单位圆盘中，即|z|<1,
\\&注意：\frac{1}{z^{-1}e^x-1}=\frac{ze^{-x}}{1-ze^{-x}}=\sum_{m=0}^{\infty}(ze^{-x})^{m+1}
\\&则\int_{0}^{\infty} \frac{x^{n-1}dx}{z^{-1}e^x-1}=\sum_{m=0}^{\infty}\int_{0}^{\infty}
x^{n-1}(ze^{-x})^{m+1}dx
=\sum_{m=0}^{\infty}\frac{z^{m+1}}{(m+1)^n}\int_{0}^{\infty}
y^{n-1}e^{-y}dy
\\&\quad=\Gamma(n)\sum_{m=0}^{\infty}\frac{z^{m+1}}{(m+1)^n}=\Gamma(n)\sum_{k=1}^{\infty}\frac{z^k}{k^n}=\Gamma(n)Li_n(z)
\\&同理得到\int_{0}^{\infty} \frac{x^{n-1}dx}{z^{-1}e^x\pm 1}=\mp\Gamma(n)Li_n(\mp z)
\\&|z|\ll 1时，Li_n(z)\approx z,
\\&z=1时，Li_n(1)=\sum_{k=1}^{\infty}\frac{1}{k^n}=\zeta(n)
\end{align}
$$

## 数理方程

### 建立方程的方法

- 统计法

	- 马尔萨斯人口模型
	- logistics模型

- 微元法

	- 波动方程
	- 电报方程
	- 热传导方程

- 规律法

	- 物理学规律

### 二阶偏微分方程

- 定解问题

	- 一维波动方程

$$
U_{tt}=a^2\nabla^2U+f(x,t)
$$
	- 三维热传导方程

$$
U_t=a^2\nabla^2U+f(x,y,z,t)
$$
	- 拉普拉斯方程

$$
\nabla^2U=f
$$

- 定解条件

	- 初始条件
	- 边界条件
	- 衔接条件

### 线性偏微分方程通解

- 标准形式
- 线性偏微分方程解的叠加性
- 常系数线性齐次/非齐次偏微分方程通解
- 特殊变系数线性齐次偏微分方程
- 波动方程行波法

	- 行波达朗贝尔公式
	- 端点的反射
	- 跃变点的反射
	- 波的色散和耗散

- 热传导方程的定型讨论
- 拉普拉斯方程的定型讨论

### 分离变量法

- 分离变量介绍

	- 两端固定弦的自由振动
	- 矩形区域的稳定问题
	- 多于两个自变量的定解问题
	- 两端固定弦的强迫振动

- 非齐次边界条件的齐次化
- 齐次的泛定方程

	- 傅里叶级数法
	- 傅里叶积分法

- 非齐次的泛定方程

	- 冲量定理法
	- 格林函数法
	- 傅里叶级数法
	- 傅里叶积分法
	- 泊松方程

- 内积空间与函数空间
- 自伴算符的本征值问题
- Sturm Liouville型方程本征值问题

### 二阶常微分方程级数解法和本征值问题

- 特殊函数常微分方程

	- 拉普拉斯方程
	- 波动方程
	- 输运方程
	- 亥姆霍兹方程
	- 矢量的波动方程

- 常点邻域上的级数解法
- 正则奇点邻域上的级数解法
- 施图姆-刘维尔本征值问题

