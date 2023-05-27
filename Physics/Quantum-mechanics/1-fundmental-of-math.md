# 数学基础

## δ函数与傅立叶变换

### 筛选性质

$$
\begin{align} &f(x)\delta(x-a)=f(a)\delta(x-a)
\\&\int^{\infty}_{-\infty}f(x)\delta(x-a)dx=f(a)\int^{\infty}_{-\infty}\delta(x-a)dx=f(a)

\end{align}
$$

### 常数提取

$$
\delta(ax)=\frac{1}{|a|}\delta(x)
$$

### 阶梯函数

$$
\frac{d\theta}{dx}=\delta(x)
$$

### 狄拉克函数的
傅里叶变换

$$
\begin{align} &f(x)=\frac{l}{\pi}\int_{-\infty}^{\infty} c_{\frac{i\omega}{\pi}} e^{i\omega x}d \omega=\frac{1}{2\pi} \int_{-\infty}^{\infty} F(\omega)e^{i\omega x}d \omega，
\\&F(\omega)=\int_{-\infty}^\infty f(x)e^{-i\omega_0x}d x
    
   =\int_{-\infty}^\infty F(\omega)\delta(\omega-\omega_0) d \omega
\\&2\pi\delta(x)=\int_{-\infty}^{\infty} e^{ik x}d k=\frac{1}{2\pi} \int_{-\infty}^{\infty} \cos kx d x，
\end{align}
$$

### 傅里叶变换

- 傅里叶级数——傅立叶积分：
周期函数→非周期函数
有限周期→无限周期

$$
\begin{align} &Fourier级数：f(t)=\sum_{-\infty}^\infty  c_ne^{in\omega t}

，c_n=\frac{1}{T}\int_{-\frac{T}{2}}^{\frac{T}{2}} f(t)\cdot e^{-in\omega t} d t
\\&Fourier积分：f(t)=\frac{1}{2\pi}\int F(\omega) e^{i\omega t}d\omega，F(\omega)=\int f(t) e^{-i\omega t }dt
\\&Plancherel定理：f(t)=\frac{1}{\sqrt{2\pi}}\int F(\omega) e^{i\omega t}d\omega，F(\omega)=\frac{1}{\sqrt{2\pi}}\int f(t) e^{-i\omega t }dt
\end{align}
$$

## Γ积分与常用积分公式

### 定义

$$
\begin{align} &n!=\int_{0}^{\infty}x^ne^{-x}dx=\Gamma(n+1)
\\&\Gamma(n+1)=n\Gamma(n),例如\Gamma(3)=\Gamma(2+1)=2\Gamma(2)=2
\\\\&\Gamma(-\frac{3}{2})=\frac{4\sqrt{\pi}}{3}，\Gamma(\frac{1}{2})=\sqrt{\pi}，
\\&\Gamma(-\frac{1}{2})=-2\sqrt{\pi}，\Gamma(1)=\Gamma(2)=1
\end{align}
$$

### 特殊积分转化

$$
\begin{align} &\int_{-\infty}^{\infty} |x|^ne^{-x^2}dx=\int_{0}^{\infty} x^{n-1}e^{-x^2}dx^2=\int_{0}^{\infty} t^{\frac{n+1}{2}-1}\cdot e^{-t}dt=\Gamma(\frac{n+1}{2})
\\&\int_{0}^{\infty} x^{n-1}\cdot e^{-ax}\cdot \sin(bx)dx=\frac{\sin(n\arctan \frac{b}{a})}{(a^2+b^2)^{n/2}}\Gamma(n),n,a>0
\\&n=2时，\int_{0}^{\infty} xe^{-ax}\cdot\sin(bx)dx=\frac{2ab}{(a^2+b^2)^{2}}，
\\&\qquad\int_{0}^{\infty} xe^{-ax}\cdot\cos(bx)dx=\frac{a^2-b^2}{(a^2+b^2)^{2}}
\end{align}
$$

### 高斯积分

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

## 坐标系与矢量变换

### 哈密顿算符与拉普拉斯算符

### 球坐标系单位矢量变换

### 双重矢量积

- 

$$
\boldsymbol A\times(\boldsymbol B\times\boldsymbol C)=\boldsymbol B(\boldsymbol A\cdot \boldsymbol C)-\boldsymbol C(\boldsymbol A\cdot \boldsymbol B)
$$

## 三角函数与常用级数

### 三角函数常用公式

### 复变函数不同形式取模

$$
e^{|ix|}=1,e^{|a+ib|}=e^a,|c|^2=a^2+b^2
$$

### 含三角函数的特殊积分

$$
\begin{align} &\int_{0}^{\infty} e^{-ax}\cdot x^{n-1}\cdot\sin(bx)dx=\frac{\sin(n\arctan \frac{b}{a})}{(a^2+b^2)^{n/2}}\Gamma(n),n,a>0

\end{align}
$$

### 双曲函数常用公式

## 常微分方程的解

### 根据系数判断解的形式

$$
\begin{align} &\frac{d^2\psi}{dx^2}=-q\psi\Rightarrow y''=-qy，特征方程r^2+q=0,r=\pm\sqrt{-q}
\\1.&q<0,\Delta>0,-q=k^2>0,
\\&y=Ae^{r_1x}+Be^{r_2x}=Ae^{kx}+Be^{-kx}=C\cosh kx+D\sinh kx
\\2.&q=0,\Delta=0,y=A+B
\\3.&q>0,\Delta<0,q=k^2>0,r=\pm i\sqrt q=\pm ik
\\&y=e^{ax}(A\cos kx+B\sin kx)=A\cos kx+B\sin kx=Ce^{ikx}+De^{-ikx}

\end{align}
$$

### 微分方程解的性质

## 内积、矩阵、行列式与基矢变换

### 内积与施瓦茨不等式

### 转置、共轭、逆、幺正、正交矩阵

### 基矢变换

$$
\begin{align} &基矢从f到e变换，|e_i\rangle=\sum_{i=1}^n S_{ij}|f_i\rangle\begin{cases}
|e_1\rangle=S_{11}|f_1\rangle+\dots+S_{n1}|f_1\rangle\\
\dots\\
|e_n\rangle=S_{1n}|f_1\rangle+\dots+S_{nn}|f_n\rangle
\end{cases}
\\&上标表示基矢,a^f=Sa^e,a^e=S^{-1}a^f,
\\&T代表一个线性变换，a'^e=T^e a^e,
\\&则a'^f=Sa'^e=S(T^e a^e)=ST^e S^{-1} a^f,即T^f=ST^e S^{-1}
\end{align}
$$

### 本征矢和本征值 

$$
\begin{align} &本征方程矩阵形式：\boldsymbol T\boldsymbol a=\lambda \boldsymbol a\Rightarrow (\boldsymbol T-\lambda \boldsymbol I)\boldsymbol a=0,\boldsymbol a\ne 0
\\&则矩阵(\boldsymbol T-\lambda \boldsymbol I)一定是奇异不可逆的\Rightarrow |\boldsymbol T-\lambda \boldsymbol I|=0
\\&即\det (\boldsymbol T-\lambda \boldsymbol I)=\left | \begin{matrix}
T_{11}-\lambda &T_{12}&\dots&T_{1n}  \\
T_{21} &T_{22}-\lambda&\dots&T_{2n}  \\\dots &\dots&\dots&\dots \\T_{n1}&T_{n2}&\dots&T_{nn}-\lambda   
\end{matrix} \right |=0
\\&展开行列式得到关于\lambda的矩阵的特征方程C_n\lambda^n+\dots+C_1\lambda+C_0=0

\\&可以得到最多n个不同\lambda本征值，本征值集合为谱线。本征值相同则谱线简并

\end{align}
$$

### 对角化与厄米变换

## 概率论与数理统计

### 均方差与期望

### 级数求和

## 特殊数理函数

### 厄米多项式

### 勒让德多项式

### 连带勒让德多项式

### 球谐函数

### 合流超几何函数

### 贝塞尔函数

### 球贝塞尔函数

## 泛函分析与变分法

