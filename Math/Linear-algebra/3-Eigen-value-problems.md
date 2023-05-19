# 特征值问题

## 特征值与特征向量

### 概述

- 

$$
\begin{align} &Ax=\lambda x,x为非零向量，变形：(A-\lambda I)x=0,x\ne 0
\\&问题：1.求所有的数\lambda,使得A-\lambda I为奇异矩阵
\\&2.给定一个使A-\lambda I奇异的数\lambda，求满足方程的所有非零向量x
\\&特征值和特征向量可以为复数
\\\\&对矩阵A_{2\times 2}=\left [ \begin{matrix}
a& b \\
c& d \\
\end{matrix} \right ],A-\lambda I=\left [ \begin{matrix}
a-\lambda& b \\
c& d-\lambda \\
\end{matrix} \right ]
\\&|A-\lambda I|=\left | \begin{matrix}
a-\lambda& b \\
c& d-\lambda \\
\end{matrix} \right|=(a-\lambda)(d-\lambda)-bc=0
\\&当且仅当\lambda^2-(a+d)\lambda+(ad-bc)=0，时满足奇异性


\end{align}
$$

### 特征多项式与特征空间

- 

$$
\begin{align} &定理：A_{n\times n}-\lambda I奇异\Leftrightarrow 特征方程\det(A-\lambda I)=0
\\&A的全部特征值为行列式展开的多项式（特征多项式）的所有零点
\\&定理：若\lambda是A_{n\times n}的一个特征值,x是A的任意特征向量
\\&（1）\lambda^k是A^k的一个特征值
\\&（2）若A为非奇异的，则\frac{1}{\lambda }是A^{-1}的一个特征值
\\&（3）\alpha任意数， \lambda+\alpha是 A+\alpha I的一个特征值
\\&（4）x也是A^k、A^{-1}、A+\alpha I的特征向量
\\&（5）A和A^T有相同特征值
\\&（6）当且仅当\lambda=0是A的特征值时，A为奇异的

\\&（7）三角矩阵的特征值为对角线上的元素
\\&凯莱哈密顿定理：若p(\lambda)是A的特征多项式，则p(A)是零矩阵


\end{align}
$$
- 

$$
\begin{align} 定义：&若\lambda是A_{n\times n}的特征值,则对应特征向量x是A-\lambda I的中的非零向量
\\&A-\lambda I的零空间由所有使得(A-\lambda I)x=0的向量组成，称为E_\lambda，
\\&E_\lambda即特征空间，E_\lambda维数（基向量个数）为\lambda的几何重数
\\推论：&1\le \lambda的几何重数\le\lambda的代数重数,特征多项式相同不等于特征空间相同
\\定义：&若\lambda是A_{n\times n}的特征值, \lambda的几何重数小于\lambda的代数重数，则A为亏损矩阵
\\定理：&特征值不同，则特征向量线性无关。n个不同特征值有n个线性无关向量
\\定理：&对实矩阵A，\lambda对应x,则必有\bar \lambda对应\bar x
\\定理：&对实对称矩阵A，所有特征值都是实数
\end{align}
$$

### 有相同特征值的矩阵类
——相似矩阵

- 相似性

	- 

$$
\begin{align} 定义：&若存在非奇异矩阵S_{n\times n}，使得B=S^{-1}AS,则A和B相似。

\\定理：&相似矩阵有相同特征多项式,从而特征值相同,代数重数相同(比相同多项式更本质)：
\\&\det(S^{-1}AS-\lambda I)=\det[S^{-1}(A-\lambda I)S]=\det(S^{-1})\det(A-\lambda I)\det(S)
\\&相似矩阵特征向量一般不同，为Sx

\end{align}
$$

- 对角化

	- 

$$
\begin{align} 定义：&A相似于对角矩阵D，则D^k=S^{-1}A^kS,计算矩阵A^k=SD^kS^{-1}

\\定理：&当且仅当A有n个线性无关的特征向量(n个不同特征值)时，矩阵A_{n\times n}是可对角化的
\\对角化&设S的列向量为A的特征向量,S=(u_1,\dots,u_n),Au_k=\lambda_ku_k
\\&S^{-1}S=(S^{-1}u_1,\dots,S^{-1}u_n)=(e_1,\dots,e_n)=I
\\&AS=(Au_1,\dots,Au_n)=(\lambda _1u_1,\dots,\lambda_nu_n)
\\&S^{-1}AS=(\lambda _1S^{-1}u_1,\dots,\lambda_nS^{-1}u_n)=(\lambda _1e_1,\dots,\lambda_ne_n)=\lambda I=D
\\定义：&正交矩阵:方阵Q可逆,且Q^TQ=E\Leftrightarrow Q^T=Q^{-1}\Leftrightarrow Q的行（列）向量是标准正交向量组
\\&对正交矩阵Q，x\in R^n,有||Qx||=||x||,\det(Q)=\pm 1
\\&实对称矩阵可被正交矩阵对角化，能被正交矩阵对角化的是实对称矩阵
\\&实对称矩阵A的特征向量是R^n的一个标准正交基，
\\&对称矩阵A对应不同特征值（属于不同特征空间）的特征向量相互正交
\\定理：&对实对称矩阵，存在正交矩阵Q使得Q^TAQ=T,T为上三角矩阵,相似于A（特殊舒尔定理）
\\定义：&（酉相似）对n阶方阵AB，存在酉矩阵U使得U^{-1}AU=U^HAU=B
\\定理：&（舒尔定理）任何方阵A都酉相似于一个三角矩阵T.A的舒尔分解：A=QTQ^T


\end{align}
$$

- 谱分解

	- 

$$
\begin{align} &A为对称矩阵，特征值\lambda_1\dots,\lambda_n，设特征向量u_1\dots,u_n单位正交，
\\&矩阵A可以表示为A=\lambda_1u_1u_1^T+\dots+\lambda_nu_nu_n^T，此即A的谱分解,
\\&每个n阶矩阵u_iu_i^T都是秩为1的矩阵,特征值不要求各异

\end{align}
$$

- 若尔当型

## 二次型

### 二次型

- 定义

	- 

$$
\begin{align} 
1.&f(x_1,x_2,\cdots,x_n)=\sum\limits_{i=1}^n\sum\limits_{j=1}^nb_{ij}x_ix_j为n元二次型，简称二次型(型为齐次多项式)
\\2.&由a_{ij}=a_{ji}=\frac{b_{ij}+b_{ji}}{2}(1\le i,j\le n)定义的对称矩阵A唯一使f(x)=x^TAx
\\3.&二次型矩阵就是一个对称矩阵，A^T=A，一定可以相似对角化。
\\4.&若二次型中只含有平方项，所有交叉项的系数为0，
\\&形如d_1x_1^2+d_2x_2^2+\cdots+d_nx_n^2的二次型就是标准形。

\\5.&若标准形中系数d_i仅为1，0，-1，
\\&即形如x_1^2+\cdots+x_p^2-x_{p+1}^2-\cdots-x_{p+q}^2的二次型称为规范形。

\\6.&二次型的标准形与规范形就是相似理论中的
\\&可逆矩阵相似对角化与实对称矩阵相似对角化的方法。

\end{align}
$$

- 分类

	- 

$$
\begin{align} &若对于R^n中所有x\ne 0，均有q(x)=x^TAx>0，\lambda_i>0
\\&则称f为\textbf{正定二次型}，对应矩阵A为\textbf{正定矩阵}。
\\&
若令一个正定二次型等于某个正数，则对于空间就是一个封闭曲面。
\\&\quad q(x),\lambda_i\ge 0\Rightarrow 半正定的，
\\&\quad q(x)\le 0,\lambda_i\le0\Rightarrow 半负 定的
\\&\quad q(x)< 0,\lambda_i<0\Rightarrow 负定的，
\\&\quad q(x)和\lambda_i有正有负\Rightarrow不定的
\\&用于描述多变量二次方程解集
\end{align}
$$

### 标准形与规范形

- 合同变换

	- 

$$
\begin{align} 1.&合同变换
\\&若f(x)=x^TAx，令x=Cy，则f(x)=(Cy)^TA(Cy)=y^T(C^TAC)y=y^TBy=g(y)，
\\&此时二次型f(x)=x^TAx通过线性变换x=Cy得到一个新二次型g(y)=y^TBy。
\\&将二次型用x表示换成用y表示:x^TAx=y^TBy,f(x)与g(y)的系数矩阵A与B满足B=C^TAC
\\2.&设AB为n阶实对称矩阵，若存在可逆矩阵C，使得C^TAC=B，
\\&则称AB\textbf{合同}，记为A\simeq B，此时f(x)与g(x)为合同二次型。
\\3.&
若二次型f(x)=x^TAx合同于标准形d_1x_1^2+d_2x_2^x+\cdots+d_nx_n^2
\\&或合同于规范形x_1^2+\cdots+x_p^2-x_{p+1}^2-\cdots-x_{p+q}^2，
\\&则称d_1x_1^2+d_2x_2^x+\cdots+d_nx_n^2为f(x)的\textbf{合同标准形}或\textbf{合同规范形}。

\end{align}
$$

- 配方法

	- 任何二次型均可通过配方法（做可逆线性变换）化为标准形与规范形
——可逆矩阵对角化

- 正交变换法

	- 任何二次型均可通过正交变换法化为标准形（规范形不一定能表示出)
——正交矩阵对角化

- 惯性定理

	- 无论选取什么样的可逆线性变换，将二次型化为标准形或规范形，其正项个数p正惯性指数，负项个数q负惯性指数都是不变的
	- 若二次型的矩阵秩为r，则r=p+q，可逆线性变换不改变正负惯性指数。
	- 两个二次型或实对称矩阵合同的充要条件是有相同的正负惯性指数，或有相同的秩及正负惯性指数。

### 正定二次型

- 正定性性质

	- 

$$
\begin{align} &等价条件组
\\& -对于任意x\neq0，有x^TAx>0。（定义）
 \\& -   f的正惯性指数p=n，即所有系数全为正。
 \\&  -  存在可逆矩阵D，使得A=D^TD。
 \\&  -  A\simeq E
  \\& -  A的特征值\Lambda_i>0（i=1,2,\cdots,n）
  \\&  - A的全部顺序主子式均大于0。

\end{align}
$$
	- 子主题 2

$$
\begin{align} 设A=(a_{ij})_{n\times n}，则\vert A_k\vert=\left|\begin{array}{cccc}
    a_{11} & a_{12} & \cdots & a_{1k} \\
    a_{21} & a_{22} & \cdots & a_{2k} \\
    \vdots & \vdots & \ddots & \vdots \\
    a_{k1} & a_{k2} & \cdots & a_{kk}
\end{array}\right|
\\称为n阶矩阵A的\textbf{k阶顺序（左上角）主子式}。

\end{align}
$$
	- 子主题 3

$$
\begin{align} &n元二次型f=x^TAx正定的必要条件是：
\\&- a_{ii}>0（i=1,2,\cdots,n）。
  \\&-\vert A\vert>0。
\end{align}
$$

- 正定性判定

	- 

$$
\begin{align} &具体型:
\\&-判定主子式是否全部大于0
 \\&  -  求特征值是否全部大于0。
 \\&  -  配方法判定正惯性指数是否全为n。
  \\&  - 定义法，证明\forall x\neq0，x^TAx>0，即f>0。
 \\&-找到可逆矩阵D，使得A=D^TD。
\\&抽象型：
\\&对于抽象型正定问题，首先要表明A是对称的，即A^T=A；
\\&基本的方法就是判定特征值\lambda是否全部为正。




\end{align}
$$

- 正定矩阵

	- 矩阵分解
	- 几何意义

### 二次曲线与二次曲面

- 子主题 1

$$
\begin{align} &一般二元二次方程x^2+bxy+cy^2+dx+ey+f=0
\\&\Rightarrow  \boldsymbol x^TA\boldsymbol x+a^T\boldsymbol x+f=0,\boldsymbol x=\left [ \begin{matrix}
x \\
y \\
\end{matrix} \right ]
,A=\left [ \begin{matrix}
a& \frac{b}{2} \\
\frac{b}{2} & c\\
\end{matrix} \right ],a=\left [\begin{matrix}
d \\
e \\
\end{matrix} \right ]
\\&利用x=Qy消去交叉项，定义不同曲线
\\&三元二次方程同理定义不同曲面

\end{align}
$$
- 主轴定理

## 特征值理论应用

### 差分方程

- A的幂
- u（k+1）=Au（k）

### 微分方程

- 求解一阶
- 指数矩阵

### 马尔科夫矩阵

### 海森伯格矩阵

- 克雷洛夫方法
- 豪斯霍尔德变换

	- QR分解

- 广义特征向量
- 矩阵多项式

