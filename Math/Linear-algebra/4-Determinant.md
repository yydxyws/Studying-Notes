#  行列式

## 定义

### 几何定义

- n阶行列式是n个n维向量组成的，运算结果是n维向量组成的几何体超体积。

线性相关，体积为0.

### 逆序数与定义

- 

$$
\left|\begin{array}{cccc}      a_{11} & a_{12} & \cdots & a_{1n} \\
    a_{21} & a_{22} & \cdots & a_{2n} \\
    \vdots & \vdots & \ddots & \vdots \\
    a_{n1} & a_{n2} & \cdots & a_{nn}
\end{array}\right| 
=\sum\limits_{j_1j_2\cdots j_n} (-1)^{\tau(j_1j_2\cdots j_n) }a_{1j_1}a_{2j_2}\cdots a_{nj_n}
$$

### 展开定理与定义

- 行列式等于其任一行或列的各元素与对应的代数余子式乘积之和。

$$
\begin{align} &余子式：D=\left|\begin{array}{cccc} 
    a_{11} & a_{12} & \cdots & a_{1n} \\
    a_{21} & a_{22} & \cdots & a_{2n} \\
    \vdots & \vdots & \ddots & \vdots \\
    a_{n1} & a_{n2} & \cdots & a_{nn}
\end{array}\right|
\\&代数余子式：\color{red}A_{ij}=(-1)^{i+j}M_{ij}
\\&D=a_{i1}A_{i1}+\cdots+a_{in}A_{in}或D=a_{1j}A_{1j}+\cdots+a_{nj}A_{nj}
\end{align}
$$

## 性质

### 拉普拉斯定理：|AB|=|A||B|

### 行列互换等价

### 行全为零值为零

### 行公因子k提外面

### 某行元素拆分和

### 两行互换值反号

### 行成比例值为零

### 倍加值不变

## 行列式的计算

### 三阶行列式

- 对角线法则

### 特殊行列式

- 主对角线

	- 

$$
\left|\begin{array}{cccc}      a_{11} & a_{12} & \cdots & a_{1n} \\
     & \ddots & \cdots & a_{2n} \\
     & & \ddots & \vdots  \\
     & & & a_{nn}
\end{array}\right|=
\left|\begin{array}{cccc} 
    a_{11} & & & \\
    a_{21} & \ddots & & \\
    \vdots & \cdots & \ddots &  \\
    a_{n1} & a_{n2} & \cdots & a_{nn}
\end{array}\right|=
\left|\begin{array}{cccc} 
    a_{11} & & & \\
     & \ddots & & \\
     & & \ddots &  \\
     & & & a_{nn}
\end{array}\right|=\prod_{i=1}^n a_{ii}
$$

- 副对角线

	- 子主题 1

$$
\begin{align} \left|\begin{array}
     & & & a_{1n} \\
     & & \ddots & a_{2n} \\
     &  \ddots& \cdots & \vdots  \\
    a_{n1} & a_{n2} & \cdots & a_{nn}
\end{array}\right|=
\left|\begin{array}
    a_{11} & a_{12} & \cdots & a_{1n} \\
    a_{21} & \cdots &  & \\
    \vdots & \ddots & & \\
    a_{n1} & & &
\end{array}\right|=
\left|\begin{array}
     & & & a_{1n} \\
     & & \ddots & \\
     & \ddots & & \\
    a_{n1} & & &
\end{array}\right|=(-1)^{\frac{n(n-1)}{2}}a_{1n}\cdots a_{n1}
\end{align}
$$

- 拉普拉斯展开式

	- 子主题 1

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

- 范德蒙德

	- 子主题 1

$$
\left|\begin{array}{cccc}          1 & 1 & \cdots & 1 \\
        a_1 & a_2  & \cdots & a_n \\
        \cdots & \cdots & \vdots & \cdots \\
        a_1^{n-1} & a_2^{n-1} & \cdots & a_n^{n-1} \\
    \end{array}\right|=\prod\limits_{1\leqslant j<i\leqslant n}(a_i-a_j)
$$

### 递推法

### 余子式和代数余子式线性组合

## 行列式理论的应用

### 克莱姆法则

- 引理

	- 

$$
\begin{align} &引理：方程组Ax=b是相容的,A_{n\times n}=(A_1,\dots,A_n),b为列向量,x_i为解的第i个分量
\\&对每个i,1\le i\le n,n\times n的矩阵B_i=(A_1,\dots,A_{i-1},b,A_{i+1},\dots,A_n)

\\&都有x_i\det(A)=\det(B_i)
\\&证明：i=1时，x_1A_1+\dots+x_nA_n=b
\\&\quad 则x_i\det(A)=\det(x_iA_1,A_2,\dots,A_n)=\det(b-x_2A_2-\dots-x_nA_n,A_2,\dots,A_n)
\\&\qquad =\det(b,A_2,\dots,A_n)-\dots-x_n\det(A_n,A_2,\dots,A_n)=\det(b,A_2,\dots,A_n)
\end{align}
$$

- Crame法则

	- 子主题 1

$$
\begin{align} &非奇异矩阵A_{n\times n}=(A_1,\dots,A_n),b为R^n任意向量
\\&对每个i,1\le i\le n,n\times n的矩阵B_i=(A_1,\dots,A_{i-1},b,A_{i+1},\dots,A_n)

\\&则Ax=b解的第i个分量x_i=\frac{\det(B_i)}{\det(A)}
\end{align}
$$

### 伴随矩阵

- 

$$
\begin{align} &伴随矩阵：行列式\vert A\vert各个元素的代数余子式A_{ij}\boldsymbol{转置}构成的矩阵。
\\&A^*=\left[
    \begin{array}{cccc}
        A_{11} & A_{21} & \cdots & A_{n1} \\
        A_{12} & A_{22} & \cdots & A_{n2} \\
        \vdots & \vdots & \ddots & \vdots \\
        A_{1n} & A_{2n} & \cdots & A_{nn}
    \end{array}
\right],\quad A^*A=AA^*=|A|E


\end{align}
$$

### 朗斯基行列式

- 

$$
\begin{align} &假设f_0(x),\dots,f_n(x)是定义在区间[a,b]上的实值函数，\\&若存在一组不全为零的数使对[a.b]所有x,a_0f_0(x)+\dots+a_nf_n(x)=0,
\\&则\{f_0(x),\dots,f_n(x)\}是一组线性相关的函数。
\\&若使该式成立只能该组数全为零，则\{f_0(x),\dots,f_n(x)\}函数组线性无关，

\\&线性无关性检验：a_0,\dots,a_n满足相关方程，且f_i(x)足够可微，对方程求导：
\\&\left[
    \begin{array}{cccc}
        f_0(x) & f_1(x) & \cdots & f_n(x) \\
        f_0'(x) & f_1'(x) & \cdots & f_n'(x) \\
        \vdots & \vdots & \ddots & \vdots \\
        f_0^{(n)}(x) &f_1^{(n)}(x) & \cdots &f_n^{(n)}(x)
    \end{array}
\right]
\left[
    \begin{array}{cccc}
        a_0 \\a_1 \\
        \vdots  \\
        a_n
    \end{array}
\right]=
\left[
    \begin{array}{cccc}
        0\\
        0 \\
        \vdots \\
        0    \end{array}
\right],
\\&系数矩阵为W(x),\det[W(x)]为\{f_0(x),\dots,f_n(x)\}的朗斯基行列式
\\&若朗斯基行列式在[a,b]中任意一点值非零，W(x)为非奇异矩阵，函数线性无关
\\&!!但是对所有x，\det[W(x)]=0\ne  函数线性相关

\end{align}
$$

## 线性代数引论，Lee W.Johnson

