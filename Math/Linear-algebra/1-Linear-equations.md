# 核心问题——
线性方程组

## 概念

### 线性方程组

- 

$$
\begin{align} 1.&\begin{cases}
n元齐次线性方程组\\
        a_{11}x_1+\cdots+a_{1n}x_n=0 \\
        \cdots \\
        a_{m1}x_1+\cdots+a_{mn}x_n=0
    \end{cases}
\qquad\begin{cases}
n元非齐次线性方程组\\
        a_{11}x_1+\cdots+a_{1n}x_n=b_1 \\
        \cdots \\
        a_{m1}x_1+\cdots+a_{mn}x_n=b_n
    \end{cases}
\\&m是方程个数，即方程组行数，n是方程未知数个数，即类似方程组的列数。
\\2.&n元线性方程组等价为矩阵方程形式Ax=b
,增广矩阵[A,b]_{m\times(n+1)}=\left[
    \begin{array}{c:c}
        \begin{matrix}
            a_{11} & \cdots & a_{1n}\\
            \cdots \\
            a_{m1} & \cdots & a_{mn}
        \end{matrix}&
        \begin{matrix}
            |&b_1\\
            |&\dots\\
            |&b_m
        \end{matrix}
    \end{array}
\right]
\\&使用向量内积，矩阵m行行向量点乘x向量，得到m个分量的列向量b
\\3.&n元线性方程组等价为列向量的线性组合x_1\left[
    \begin{array}{c}
        a_{11} \\
        \cdots \\
        b_{m1}
    \end{array}
\right]
+x_2
\left[
    \begin{array}{c}
        a_{12} \\
        \cdots \\
        b_{m2}
    \end{array}
\right]
+\dots+x_n\left[
    \begin{array}{c}
        a_{1n} \\
        \cdots \\
        b_{mn}
    \end{array}
\right]
=\left[
    \begin{array}{c}
        b_1 \\
        \cdots \\
        b_m
    \end{array}
\right],
\\&n列，即n个未知数的系数列向量，m行，即每个未知数有m个系数，解m个一元方程
\\4.&n元线性方程组等价为列向量与变量的内积形式：
\left[
    \begin{array}{c}
        A_1 &
        \cdots &
        A_n
    \end{array}
\right]
\left[
    \begin{array}{c}
        x_1 \\
        \cdots \\
       x_n
    \end{array}
\right]
=b_{1\times n},A_i表示n个列向量
\end{align}
$$

### 矩阵和子式

- 矩阵实际就是数表，提供了线性方程组的简化记号。
在矩阵中，任取k行和k列 ，位于这些行和列的交点上的k2个元素原来的次序所组成的k阶方阵的行列式，叫做A的一个k阶子式。

## 求解线性方程组一般步骤

### → 给定m×n方程组
→ 写出增广矩阵[A|b]
→ 简化为阶梯型矩阵[C|d]，m×(n+1)
→ 代入求解或判断解的类型

- 注意增广矩阵无法判断和求解

### 高斯消元法与初等变换

- 

$$
\begin{align} &设A是一个m\times n矩阵，初等变换具有如下性质：
\\&\begin{cases}
     对A进行一次初等行变换，相当于在A左乘对应m阶初等矩阵；\\对A进行一次列变换，相当于在A右乘对应n阶初等矩阵。\\
     方阵A可逆的充分必要条件是存在有限个初等矩阵P_i使得A=\prod\limits_{i=1}^nP_i。\\
     方阵A可逆的充要条件是A\overset{r}{\sim}E。（即A代表的线性方程组能通过初等计算得到最后的解）
\end{cases}
\end{align}
$$
- 

$$
\begin{align}  &初等矩阵的转置也是初等矩阵。
  \\&   对初等矩阵进行行或列变换，\vert E_{ij}\vert=-1，对其求逆：E_{ij}^{-1}=E_{ij}。
     \\&对初等矩阵i行乘k，\vert E_i(k)\vert=k，对其求逆：E_i(k)^{-1}=E_i\left(\dfrac{1}{k}\right)。
    \\& 对初等矩阵第j行乘k加到i行，\vert E_{ij}(k)\vert=1，对其求逆：E_{ij}(k)^{-1}=E_{ij}(-k)。
\end{align}
$$
- 解方程组，使用初等行变换解不会发生改变，使用初等列变换则会改变解。
对于任何矩阵都能通过初等列变换变为行阶梯形矩阵和行最简形矩阵，
再通过列变换可以变为{标准形}：左上角是一个单位矩阵，其他元全部是0。
- LU分解

	- 高斯消去法等价于分解为三角矩阵：A=LU，L为行阶梯型矩阵（上三角矩阵）U变为A的矩阵（下三角矩阵，多个初等矩阵乘积）

另一种方式：A=LDU，U‘=DU，D为对角矩阵

### 逆矩阵求解

- 

$$
\begin{align} &若\boldsymbol A\boldsymbol x=\boldsymbol b,则解为\boldsymbol x=\boldsymbol A^{-1}\boldsymbol b,即求矩阵A的逆


\end{align}
$$

### 相容线性方程组

- 相容方程组：至少有一个解
不相容：无解。即[C|d]中C部分存在零行且d对应行非零。
- 同解方程组：有相同的解集，初等变换方程组同解
           增广矩阵与行阶梯型矩阵同解。
- 解集的几何解释：空间解析几何中图形元素交点的个数

## 线性方程组的解

### 求解Ax=0

- m×n方程组解得可能性：
无穷多解（r＜n）、唯一平凡解（r=n）
- m×n方程组，m＜n，必然有无穷多个（非平凡）解
        m≥n，必然为唯一零解。
特解：齐次方程组必然相容，永远存在零解(平凡解)。
- 非奇异矩阵

$$
\begin{align} &若相关方程\boldsymbol A\boldsymbol x=\boldsymbol 0唯一解为零解\boldsymbol x=\boldsymbol 0，则矩阵A为非奇异矩阵。
\\&当且仅当列向量(A_1,A_2,\dots,A_n)为线性无关组
，A为非奇异矩阵


\end{align}
$$

### 求解Ax=b

- m×n方程组解得可能性：（与m无关）
无穷多解（r＜n）、无解（r=n+1）、唯一解（r=n）
- r为行阶梯型矩阵[C|d]中非零行的个数（必然有r≤m），有r≤n+1。
    r=n+1时，有一行形式为[0,0...,1]，方程组一定不相容。
    r＜n+1，即r≤n，方程组必相容（r(A)=r(A|b)）
        r=n，方程组有唯一解。（当且仅当矩阵A为非奇异矩阵，方程Ax=b有唯一解）
        r<n，无论是否m＜n，必然有无穷多个解。
                每个非零行非零首元看做一个因变量（约束）
                n个变量，r个因变量（约束），则n-r个自由变量，赋任意值。
- 克拉默法则

### 线性方程组通解的向量形式

- 确定的向量系数×自由变量构成的列矩阵，r为行阶梯型矩阵的非零行个数。
- 

$$
\boldsymbol x=\left[     \begin{array}{c}
        x_1 \\
        \cdots \\
        x_r\\\_\_\_\\
x_{r+1}\\\dots \\ \dots\\x_{n}
    \end{array}
\right]=
1\left[
    \begin{array}{c}
        \alpha_{1} \\
        \cdots \\
 
        \alpha_{r}\\\_\_\_
\\0\\0\\\dots \\0
    \end{array}
\right]
+x_{r+1}
\left[
    \begin{array}{c}
        \beta_{1} \\
        \cdots \\
        \beta_{r}\\\_\_\_\\
1\\0\\ \dots\\0
    \end{array}
\right]
+\dots+x_n\left[
    \begin{array}{c}
        \gamma_{1} \\
        \cdots \\
        \gamma_{r}\\\_\_\_\\
0\\\dots \\ \dots\\1
    \end{array}
\right]
$$

## 线性方程组应用

### 求解二次曲线和曲面

- 给出一般形式，代入点的坐标，求解线性方程组，必然有r<n，得到曲线曲面方程。

### 确定网络中流量

- 对一个网络，进入节点总流等于离开节点总流，每条通道表示一个流量Xi，建立线性方程组。

### 图和网络

## 矩阵理论

### 重要矩阵

- 

$$
\begin{align} &转置矩阵：A=(a_{ij}),A^T=(a_{ji})

\\&对称矩阵:方阵A=A^T，且元素以对角线为对称轴对应相等。
\\&
反对称矩阵:方阵-A=A^T，且\left\{\begin{array}{l}
    a_{ij}=-a_{ji},i\neq j \\
    a_{ii}=0
\end{array}\right.
\\&
正交矩阵:方阵A^TA=E\Leftrightarrow A^T=A^{-1}\Leftrightarrow A的行（列）向量是标准正交向量组
\\&幂等矩阵:方阵P^2=P
\\&转置共轭矩阵：A^*=(\bar A)^T。
\\&厄米矩阵:方阵A^*=A,只有实特征值
\\&正定矩阵:对R^n中所有x\ne 0，实对称矩阵A都有x^TAx>0.特征值均为正

\\&酉矩阵:方阵A^*A=I .酉矩阵的特征值|\lambda|=1
,正交矩阵为实数域酉矩阵
\end{align}
$$

### 逆矩阵

- 逆矩阵定义

	- 若方阵AB=BA=E,则A是可逆矩阵，且逆矩阵唯一。

$$
方阵A可逆\Leftrightarrow |A|\ne 0
$$
	- 将AA-1=E看做矩阵方程，若A为非奇异的，则x=A-1有唯一解。

- 矩阵的逆存在性
- 逆矩阵计算

	- 

$$
\begin{align} 1.&伴随矩阵法：A^{-1}=\dfrac{1}{\vert A\vert}A^*
\\&求出\vert A\vert，判断是否为0\Rightarrow 写出A^*\Rightarrow计算A^{-1}=\frac{1}{\vert A\vert}A^*
\\2.&定义法：\begin{cases}
寻找矩阵B，使得AB=E，A^{-1}=B\\
A=BC,BC可逆，A^{-1}=(BC)^{-1}=C^{-1}B^{-1}\\
\left[\begin{array}{cc}
    A & O \\
    O & B
\end{array}\right]^{-1}=\left[\begin{array}{cc}
    A^{-1} & O \\
    O & B^{-1}
\end{array}\right],\quad \left[\begin{array}{cc}
    
O & A \\
    B & O
\end{array}\right]=\left[\begin{array}{cc}
    O & B^{-1} \\
    A^{-1} & O
\end{array}\right]
\end{cases}

\\3.&初等变换法（高斯-若尔当）：\left[A\vdots B\right]\overset{r}{\sim}\left[E\vdots A^{-1}\right]，\left[\begin{array}{c}
    A \\
    B
\end{array}\right]\overset{c}{\sim}\left[\begin{array}{c}
    E \\
    A^{-1}
\end{array}\right]
\\&2\times 2矩阵A=\left [ \begin{matrix}
a& b \\
c& d \\
\end{matrix} \right ],\Delta=ad-bc\ne 0,则A^{-1}=\frac{1}{\Delta}\left [ \begin{matrix}
d& -b \\
-c& a \\
\end{matrix} \right ]
\end{align}
$$

### 矩阵计算规律

- 

$$
\begin{align} &\begin{cases}
|kA|=k^n|A|\\
(kA)^T=kA^T\\
(kA)^{-1}=\frac{1}{k}A^{-1}\\
(kA)^*=k^{n-1}A^*
\end{cases}
\quad
\begin{cases}
|A+B|\ne |A|+|B|\\
(A+B)^T=A^T+B^T\\
(A+B)^{-1}\ne A^{-1}+B^{-1}\\
(A+B)^*\ne A^*+B^*
\end{cases}
\quad
\begin{cases}
|AB|=|A||B|\\
(AB)^T=B^TA^T\\
(AB)^{-1}= B^{-1}A^{-1}\\
(AB)^*\ne B^*A^*
\end{cases}

\\&\begin{cases}

(A^{-1})^T=(A^T)^{-1}\\
(A^*)^{-1}= (A^{-1})^*\\
(A^T)^*= (A^*)^T
\end{cases}
\quad \begin{cases}

|A^T|=|A|,|A^{-1}|=|A|^{-1}\\
|A^*|=|A|^{n-1}\\
(A^*)^*= |A|^{n-2}A
\end{cases}

\quad \begin{cases}
伴随矩阵A^*A=AA^*=|A|E\\
单位矩阵EA=AE\\
逆矩阵AB=E=BA
\end{cases}
\end{align}
$$
- 

$$
\left|\begin{array}{cc}     A & O \\
    O & B
\end{array}\right|=
\left|\begin{array}{cc}
    A & * \\
    O & B
\end{array}\right|=
\left|\begin{array}{cc}
    A & O \\
    * & B
\end{array}\right|=\vert A\vert\cdot\vert B\vert
$$

### 矩阵的秩

- 矩阵的秩

	- 最高阶非零子式的阶数r（A）
秩的本质就是组成矩阵的线性无关的向量个数。
若秩等于矩阵行数就是满秩，否则就是降秩。

- 性质

	- 

$$
\begin{align} &r(kA)=r(A)。
\\&
r(AB)\leqslant\min\{r(A),r(B)\}。当且仅当AB满秩等号成立。
\\&
r(A+B)\leqslant r(A|B)\leqslant r(A)+r(B)。
\\&
r(A^*)=\left\{\begin{array}{l}
    n, r(A)=n \\
    1, r(A)=n-1 \\
    0, r(A)<n-1
\end{array}\right.
\end{align}
$$

- 等价矩阵

	- 若AB同型且秩相等，则其等价。

$$
\begin{align} &\begin{cases}
&若A经过有限次行变换得到B，则称AB行等价，记为A\overset{r}{\sim}B；\\&若A经过有限次列变换得到B，则称AB列等价，记为A\overset{c}{\sim}B；\\&若A经过有限次初等变换得到B，则称AB等价，记为A\sim B。
\end{cases}
\\&设AB都是m\times n矩阵，初等变换与矩阵乘积关系：\\&\begin{cases}
& A\overset{r}{\sim}B的充要条件是存在m阶可逆矩阵P，使得PA=B。
\\&A\overset{c}{\sim}B的充要条件是存在n阶可逆矩阵Q，使得AQ=B。
\\&A\sim B的充要条件是存在m阶可逆矩阵P和n阶可逆矩阵Q，使得PAQ=B。
\end{cases}

\end{align}
$$

### 矩阵理论应用

- 差值多项式与
范德蒙德矩阵

	- 子主题 1

$$
\begin{align} &t_0,\dots,t_n各不相同时，范德蒙德矩阵
\left[
    \begin{array}{cccc}
        1 & t_0 & t_0^2 & \dots&t_0^n \\
        1 & t_1 & t_1^2 & \dots&t_1^n \\
        \vdots & \vdots & \vdots &\ddots& \vdots \\
        1 & t_n & t_n^2 &\dots&t_n^n
    \end{array}
\right]为非奇异矩阵，转置也是
\\&给定n+1个不同的数t_0,\dots,t_n,任意n+1个值y_0,\dots,y_n
\\&有且只有一个次数≤n的多项式p(t)=a_0+a_1t+\dots+a_nt^n,使得p(t_i)=y_i
\end{align}
$$

- 初值问题的解
- 数值积分与数值微分

## 等价结论组

### 对于n×n方阵A（等价结论组）
·A有逆矩阵
·A为非奇异矩阵
·A与I行等价
·|A|≠0
·Ax=0只有零解x=0
·Ax=b有唯一解
·A的列向量线性无关
·A满秩，r（A）=n
·A的特征向量线性无关
·A有n个不同的特征值
·A可对角化

### 对于n×n方阵A（等价结论组）
·A没有逆矩阵
·A为奇异矩阵
·A与I行不等价
·|A|=0
·Ax=0有无穷多个解
·Ax=b有无穷多个解
·A的列向量线性相关
·A不满秩，r（A）<n
·A的特征向量线性相关
·A存在相同的特征值
·A不可对角化

