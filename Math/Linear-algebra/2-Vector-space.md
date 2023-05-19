# 向量空间

## 向量空间R^n

### 欧几里得n维空间R^n

- 定义

	- 向量满足封闭性质、加法性质、数乘性质的向量集合称为向量空间。比如欧几里得空间。

- 数量积与几何结构

	- 

$$
\begin{align} &所有实分量的n维向量的集合，称为欧式空间，R^n，
\\&R^n成员为(n×1)的实矩阵,即所有列向量的集合
\\&欧几里得长度（范数）：||x||=\sqrt{\sum_n x_i^2}=\sqrt{x^Tx}
\\&欧几里得距离：||x-y||
\\&柯西施瓦茨不等式：||A^TB||\le||A||||B||
\\&三角不等式：||A+B||\le||A||+||B||
\\&||||A||-||B||||\le||A-B||
\end{align}
$$
	- 

$$
\begin{align}  &R^n中的内积：<x,y>=x^Ty
\\&函数<u,v>=u^TAv是R^n的内积,当且仅当A_{n\times n}是一个对称正定矩阵

\end{align}
$$

- 矩阵乘法

	- 

$$
\begin{align} &左列=右行时，左行\times右列：(a_{i1},a_{i2},\cdots,a_{is})\left(
    \begin{array}{c}
        b_{1j} \\
        b_{2j} \\
        \cdots \\
        b_{sj}
    \end{array}
\right)=\sum\limits_{k=1}^sa_{ik}b_{kj}=c_{ij}
\\&左行\times右列：左行可为列向量组成的行，右列可为行向量组成的列（分块矩阵）
\\&这实际上是向量的点积
\end{align}
$$
	- 

$$
\begin{align} &左行=右列时，左列\times右行： \left(\begin{array}{c}
        a_{1} \\
        a_{2} \\
        \cdots \\
        a_{n}
    \end{array}
\right) (b_{1},b_{2},\cdots,b_{n})
   =\left(\begin{array}{c}
        a_{1}b_{1}&a_{1}b_{2} &\cdots&a_{1}b_{n}\\
        a_{2}b_{1} &a_{2}b_{2}&\cdots&a_{2}b_{n}\\
        \cdots &\cdots&\ddots&\vdots\\
        a_{n}b_{1}& a_{n}b_{2}&\cdots&a_{n}b_{n}
    \end{array}
\right) 
\\&左列\times右行：左列可为列向量组成的行，右行可为行向量组成的列（分块矩阵）
\\&这实际上是向量的外积/张量积。
\end{align}
$$
	- 

$$
\begin{align} &叉积的导出：向量分量与正交条件导出含n-1个方程n个未知数的方程组
\\&该方程组齐次且未知数个数大于方程个数，恒有非零解\\&定义：对三维向量，\boldsymbol {u\times v}=\left(\begin{array}{c}
        u_2v_3-u_3v_2 \\
        u_3v_1-u_1v_3 \\
        u_1v_2-u_2v_1 
    \end{array}
\right) =
\left(\begin{array}{c}
        \boldsymbol i &\boldsymbol  j&\boldsymbol k \\
        u_1&u_2&u_3 \\
        v_1&v_2&v_3
    \end{array}
\right) ,方向有右手定则
\\&代数性质：\boldsymbol u\times\boldsymbol v=-\boldsymbol v\times\boldsymbol u,\quad\boldsymbol u\cdot(\boldsymbol v\times\boldsymbol w)=(\boldsymbol u\times \boldsymbol v)\cdot \boldsymbol  w,\quad \boldsymbol u\times(\boldsymbol v\times\boldsymbol w)\ne (\boldsymbol u\times \boldsymbol v)\times \boldsymbol  w

\end{align}
$$

- 满足向量空间三条性质的向量空间子集称为Rn的子空间。
- 基和维数

	- 对属于n维向量空间的任意向量b，都能被n组向量组成的向量组唯一线性表示，则该向量组为该空间的基。
向量组的基线性无关。
	- 如果n个向量组成的矩阵为可逆矩阵，则这n个向量为该空间的一组基，而数字n就是该空间的维数.

构成向量空间的基向量个数即维数。
一个子空间所有的基包含相同个数的基向量。

### 线性相关性

- 定义

	- 线性组合

		- 

$$
\begin{align} &R^m中向量组\{\boldsymbol a_1,\boldsymbol a_2,\cdots,\boldsymbol a_m\}线性组合：k_1\boldsymbol\alpha_1+k_2\boldsymbol\alpha_2+\cdots+k_m\boldsymbol\alpha_m,k_i\in R
\\&向量组\{\boldsymbol a_1,\boldsymbol a_2,\cdots,\boldsymbol a_m\}所有线性组合构成的集合称为张成（span）
\\&R^m中任意向量的张成都是R^m的子空间

\end{align}
$$

	- 线性相关

		- 

$$
\begin{align} &相关方程：k_1\boldsymbol\alpha_1+k_2\boldsymbol\alpha_2+\cdots+k_m\boldsymbol\alpha_m=\boldsymbol 0，\boldsymbol A\boldsymbol k=\boldsymbol 0
\\&

线性相关：相关方程存在非平凡解，则称\boldsymbol a_1,\boldsymbol a_2,\cdots,\boldsymbol a_m线性相关。
\\&
\qquad 含有零向量或成比例向量的向量组必然线性相关。
\\&

线性无关：相关方程只有平凡解，则称\boldsymbol a_1,\boldsymbol a_2,\cdots,\boldsymbol a_m线性无关。
\\&

\qquad 一个非零向量必然线性无关。
\\\\&p个不同向量\boldsymbol a_1,\boldsymbol a_2,\cdots,\boldsymbol a_p是\boldsymbol R^m中的向量组，p>m，向量组必然线性相关

\end{align}
$$

- 判定定理

	- 

$$
\begin{align}     1.&\alpha_1,\alpha_2,\cdots,\alpha_n线性无关\quad\Leftrightarrow\quad向量组的任一向量都不能被其他向量线性表出。
\\&【线性相关至少存在一个约束】


     \\2.&向量组\alpha_1,\alpha_2,\cdots,\alpha_n线性无关，而\beta,\alpha_1,\alpha_2,\cdots,\alpha_n线性相关，
\\&则\beta可由\alpha_1,\alpha_2,\cdots,\alpha_n线性表示，且表示方法唯一。
\\&【b在n组向量张成的空间中，则可被其唯一线性表示，且这组向量为基】
\end{align}
$$
	- 

$$
\begin{align}    3.& 若向量组\alpha_1,\alpha_2,\cdots,\alpha_n可由小于n个向量的向量组表示，则n维向量组必然线性相关

\\&若线性无关向量组\alpha_1,\alpha_2,\cdots,\alpha_n可由另一组向量表示，则该组向量个数\ge n
     \\&【在有限维向量空间中，线性无关组长度\le张成向量组长度】【低维不能表示高维】
\end{align}
$$
	- 

$$
\begin{align} 
     4.&向量组\alpha_1,\alpha_2,\cdots,\alpha_m线性相关\quad\Leftrightarrow\quad 齐次线性方程Ax=0有无穷多解
\\&向量组\alpha_1,\alpha_2,\cdots,\alpha_m线性无关\quad\Leftrightarrow\quad 齐次线性方程Ax=0只有零解
\\&系数矩阵的列向量线性相关——齐次方程组有非零解。
    \\5.&向量\beta=\alpha_1,\alpha_2,\cdots,\alpha_n\quad\Leftrightarrow\quad Ax=\beta有解
\\&向量\beta\ne\alpha_1,\alpha_2,\cdots,\alpha_n\quad\Leftrightarrow\quad Ax=\beta无解

  \\&系数矩阵列向量线性无关，增广矩阵列向量线性相关——非齐次方程组有解
\end{align}
$$
	- 

$$
\begin{align}  6.& 向量组\alpha_1,\alpha_2,\cdots,\alpha_n部分线性相关，则全部线性相关。
   
\end{align}
$$
	- 

$$
\begin{align} 
   7.&原来线性相关的向量组，降维仍然线性相关。
\\&原来线性无关的向量组，扩充后仍线性无关。  
\\&引理：如果向量组\{\alpha_1,\alpha_2,\cdots,\alpha_m\},线性相关,\alpha_1\ne 0,j\in\{2,\dots,m\}
\\&\qquad 则去掉向量组的第j项，剩余组的张成仍然为原张成
\\&定理：在向量空间中，每个张成向量组都可以化简为一组基
\\&定理：在有限维向量空间，每个线性无关向量组都可以扩充为一组基。
\end{align}
$$

- 最大无关组

	- 子主题 1

$$
\begin{align}  & 极大线性无关组：在向量组\alpha_1,\alpha_2,\cdots,\alpha_n中，
\\&若存在部分a_i,a_j,\cdots,a_k满足：a_i,a_j,\cdots,a_k线性无关；
\\&向量组中任一向量a_s（i=1,2,\cdots,n）均可由a_i,a_j,\cdots,a_k线性表出，
\\&则称向量组a_i,a_j,\cdots,a_k为原向量组的极大线性无关组。
\\&
不包含无用约束方程的最简方程组的系数矩阵就是极大线性无关组。
\\&
向量组的极大线性无关组一般不唯一，
\\&只由一个零向量组成的向量组不存在极大线性无关组，
\\&一个线性无关向量组的极大线性无关组就是其本身。


\end{align}
$$

- 等价向量组

	- 两个向量组可以互相线性表出，则称其为等价向量组

- 向量组的秩

	- 向量组构成矩阵的秩等于行向量组的秩等于列向量组的秩。

### 子空间

- 生成子空间

	- 

$$
\begin{align}  & \boldsymbol S=\{\boldsymbol x_1,\dots,\boldsymbol x_n\}\in R^n,则由\boldsymbol x_1,\dots,\boldsymbol x_n所有线性组合构成的子空间W
\\&称为S生成的子空间，记作Sp(S)或Sp\{\boldsymbol x_1,\dots,\boldsymbol x_n\}
\\&Sp\{\boldsymbol x\}=\{a\boldsymbol x:a为任意实数\}
   
\end{align}
$$

- 基本子空间

	- 零空间

		- 

$$
\begin{align}  & 矩阵\boldsymbol A_{m\times n}的零空间(\boldsymbol A的核)N(A)=\{\boldsymbol  {x:Ax=0},\boldsymbol x\in\boldsymbol R^n\}
\\&零空间由所有使得\boldsymbol A\boldsymbol x为零向量的向量\boldsymbol x组成，
\\&实际上零空间就是齐次方程组的解空间，N(A)\in\boldsymbol R^n

\end{align}
$$

	- 列空间

		- 子主题 1

$$
\begin{align}  & 矩阵\boldsymbol A_{m\times n}的列空间
(\boldsymbol A的值域)R(A)=\{\boldsymbol  {y:Ax=y},\boldsymbol x\in\boldsymbol R^n\}
\\&列空间由所有使得线性方程组\boldsymbol A\boldsymbol x=\boldsymbol y相容的向量\boldsymbol y组成，
\\&与\boldsymbol A相乘看作是定义R^m\rightarrow R^n的函数，则R^m产生的所有向量的集合为值域

   \\&C(A)\in\boldsymbol R^n
\end{align}
$$

	- 行空间

		- 

$$
\begin{align}  & 矩阵\boldsymbol A_{m\times n}的行空间
R(A^T)\in\boldsymbol R^m,\dim R(A^T)=rank (A)=r

   
\end{align}
$$

	- 左零空间

		- 

$$
\begin{align}  & 矩阵\boldsymbol A_{m\times n}的左零空间
C(A^T)\in\boldsymbol R^m,\dim R(A^T)=m-rank (A)=m-r

   
\end{align}
$$

- 子空间性质

	- 行阶梯型矩阵，主元存在的列数=列空间维数。自由变量存在的列数=零空间维数
列空间维数dimC(A)=rank(A)，
零空间维数dimN(A)=n−rank(A)
A的行空间和列空间有相同维数。
	- 行等价矩阵有相同行空间
	- 零空间维数被称为A的零化度，在矩阵A的行梯阵形矩阵中不包含台阶的纵列数，A的值域维数被称为A的秩。
	- 秩-零化度定理:对于m×n矩阵A，
n=rank(A)+nullity(A)
m=dimC(A)+dimN(A^T)=m

### 正交向量与正交子空间

- 正交向量

	- 两正交向量的点积为0。另外，x,y可以为0向量，由于0向量与任意向量的点积均为零，所以0向量与任意向量正交。
	- 把行空间与零空间称为n维空间里的正交补，即零空间包含了所有与行空间正交的向量；
同理列空间与左零空间为m维空间里的正交补，即左零空间包含了所有与零空间正交的向量。
	- 行空间与零空间将R^n分割为两个正交的子空间，
列空间与左零空间将R^m分割为两个正交的子空间。

- 正交矩阵

	- 标准正交基

		- 

$$
a^T_ia_j=\delta_{ij}
$$

	- 施密特正交化过程

### 从R^m到R^n的线性变换

- 线性变换

	- 把向量映射成向量的函数

$$
\begin{align} &\boldsymbol V\in \boldsymbol R^n,\boldsymbol W^\in \boldsymbol R^m,设T:\boldsymbol V\rightarrow \boldsymbol W,若对于\boldsymbol V中所有\boldsymbol u\boldsymbol v和数a
\\&都有T(\boldsymbol u+\boldsymbol V)=T(\boldsymbol u)+T(\boldsymbol v),T(a\boldsymbol u)=aT(\boldsymbol u)
\\&则称函数T是一个线性变换
\end{align}
$$

- 变换矩阵

	- 

$$
\begin{align} &设线性变换T:\boldsymbol R^n\rightarrow \boldsymbol R^m,\boldsymbol e_1,\dots,\boldsymbol e_n为\boldsymbol R^n中的单位向量
\\&定义变换矩阵A_{m\times n}=\big(T(\boldsymbol e_1),T(\boldsymbol e_2)\dots,T(\boldsymbol e_n)\big)
\\&则对于\boldsymbol R^n中所有\boldsymbol x，都有T(\boldsymbol x)=\boldsymbol A\boldsymbol x
\\&T(\boldsymbol x)=x_1T(\boldsymbol e_1)+x_2T(\boldsymbol e_2)+\dots+x_nT(\boldsymbol e_n)
\end{align}
$$

- 正交变换

	- 正交投影

		- 

$$
\begin{align} &\boldsymbol W\in \boldsymbol R^n,\dim(\boldsymbol W)=p,S=\{\boldsymbol e_1,\dots,\boldsymbol e_p\}是\boldsymbol W的一个标准正交基,
\\&则\boldsymbol v在\boldsymbol W上的正交投影T:\boldsymbol R^n\rightarrow \boldsymbol W定义为
\\&
T(\boldsymbol v)=(\boldsymbol v^T\boldsymbol e_1)\boldsymbol e_1+(\boldsymbol v^T\boldsymbol e_2)\boldsymbol e_2+\dots+(\boldsymbol v^T\boldsymbol e_p)\boldsymbol e_p，且T为线性变换
\end{align}
$$

	- 正交变换

		- 

$$
正交变换：对R^2中所有向量v,有||T(v)||=||v||，|A|=1
$$

- 最小二乘法

	- 不相容线性方程组最小二乘解

		- 如果给定线性方程组Ax=b无解，则进一步希望求x*，使得残差向量r=Ax*-b尽可能小。x*即Ax=b的最小二乘解。

	- 数据的最小二乘拟合
	- 亏秩矩阵
	- 最小二乘理论
	- 不相容方程组最小二乘解

## 有限维向量空间

### 向量空间

- 向量概念的推广：替换R^n中的向量

	- 矩阵、多项式、连续函数、狗
	- 一般的向量空间应包含向量的集合V，数量的集合S，以及加法和数乘两种代数运算
	- 数量集合S为实数时，V被称为实向量空间

- 有限维向量空间

	- 

$$
\begin{align} &V中向量组\{\boldsymbol a_1,\boldsymbol a_2,\cdots,\boldsymbol a_m\}线性组合：k_1\boldsymbol\alpha_1+k_2\boldsymbol\alpha_2+\cdots+k_m\boldsymbol\alpha_m,
\\&其中k_i属于实数集 R，所有线性组合构成的集合称为张成，记为span(\boldsymbol a_1,\cdots,\boldsymbol a_m)
\\&即span(\boldsymbol a_1,\cdots,\boldsymbol a_m)=\{k_1\boldsymbol\alpha_1+k_2\boldsymbol\alpha_2+\cdots+k_m\boldsymbol\alpha_m:k_i\in R\}
\\&V中任意一组向量的张成都是V的子空间
\\&如果一个向量空间可以由他的一组向量张成，则称其为有限维的
\end{align}
$$

- 子空间

	- 若V和W是向量空间，且W是V的非空子集，则W为V的子空间。
	- W为V的子集，当且仅当
（1）V的零向量0属于W
（2）u和v属于W，且u+v也属于W
（3）u属于W，且au也属于W
时，W为V的子空间。

- 生成集合

	- 

$$
\begin{align}  & Q=\{\boldsymbol v_1,\dots,\boldsymbol v_m\}是向量空间V的一个向量组,
\\&如果V中每一个向量\boldsymbol v都是Q中向量的线性组合：\boldsymbol v=a_1\boldsymbol v_1+\dots+a_m\boldsymbol v_m,
\\&称Q为V的一个生成集合
,Sp(Q)是V的子空间
\\&W\in V，且Q\subseteq W,当且仅当W=Sq(Q)时，Q是W的生成集合
\end{align}
$$

- 向量空间基

	- 若生成集合Q线性无关，则Q为V的一个基。（基只包含有限个向量）

### 内积空间与几何结构

- 实向量空间V的内积是一个函数，对V中每对向量u、v都赋予一个实数<u,v>，且满足：
（1）<u,u>≥0，当且仅当u=0时<u,u>=0
（2）<u,v>=<v,u>
（3）<au,v>=a<u,v>
（4）<u,v+w>=<u,v>+<u,w>
- 带内积的向量空间为内积空间
- 正交基

	- 

$$
\begin{align}  1.&任意向量用正交基表示：
\\&设B=\{v_1,\dots,v_n\}是内积空间的一组正交基，
\\&若v是V中任意向量，则u=\frac{\langle v_1,u\rangle}{\langle v_1,v_1\rangle}v_1+\dots+\frac{\langle v_n,u\rangle}{\langle v_n,v_n\rangle}v_n
\\2.&格拉姆-施密特正交化：
\\&设V为内积空间，\{u_1,\dots,u_n\}是V的一组基，令v_1=u_1，
\\&且对2\le k\le n，定义v_k=u_k-\sum_{j=1}^{k-1}\frac{\langle v_k,v_j\rangle}{\langle v_j,v_j\rangle}v_j


\end{align}
$$

- 正交投影与应用

	- 最佳最小二乘逼近
	- 傅里叶级数
	- 勒让德多项式
	- 第一类切比雪夫多项式

### 线性变换

- 有限维向量空间到有限维向量空间的线性映射。

根本性质：T(u+w)=T(u)+T(w),T(au)=aT(u)
- 若T:U→V是线性变换，且U为有限维向量空间，则T在U上作用完全取决于T在U的基上作用
- 向量空间之间的线性映射

	- 1.（一一）单射：f(x)=f(y)意味着x=y，可定义反函数，但未必值域的每个元素都一一对应，可以存在空缺，但不能重合
2.（多一/映上）满射：只要R(f)=Y,可以存在重合，但不能空缺
3.(一一对应)双射，即对应关系既是单射又是满射，所有元素完全一一对应

- 基本性质

	- 

$$
\begin{align} &T:U\rightarrow V为线性变换，定义U和V中零向量为0_U和0_V，
\\&T的零空间（核）为U的子集，N(T)=\{u\in U:T(u)=0_V\}
\\&T的值域，为V的子集，R(T)=\{v\in V:存在u\in U,v=T(u)\}

 \\1.&T(0_U)=0_V
\\2.&N(T)是U的子空间
\\3.&R(T)是V的子空间
\\4.&当且仅当N(T)=\{0_U\},即nullity(T)=0时，T是一一对应的
\\&设U为p维，B=\{u_1,\dots,u_p\}是U的一组基
\\1.&R(T)=Sp\{u_1,\dots,u_p\}
\\2.&当且仅当\{T(u_1),\dots,T_(u_p)\}在V中线性无关时，T是一一对应的
\\3.&rank(T)+nullity(T)=\dim(U)=p
\\&以上留作证明

\end{align}
$$

- 线性变换的运算

	- S·T≠T·S
	- 可逆变换

		- 既是一一对应又是映上（满射）的变换是可逆线性变换
		- 

$$
\begin{align} &T:U\rightarrow V为可逆线性变换

 \\1.&T^{-1}为线性变换
\\2.&T^{-1}是可逆的，且(T^{-1})^{-1}=T
\\3.&T^{-1}\cdot T=I_U,T\cdot T^{-1}=I_V,I为恒等变换
\end{align}
$$

	- 同构的向量空间

		- 若T:U→V是可逆线性变换，则UV为同构的向量空间，T称为一个同构。
		- 实n维向量空间U和欧式空间R^n是同构的。
实n维向量空间U和 V是同构的。
		- 若T:U→V是线性变换，L(U,V)是所有线性变换集合，L也是向量空间，且dim(U)=n,dim(V)=m时，L(U,V)同构于向量空间R_mn

- 线性变换的矩阵表示

	- 

$$
\begin{align} 1.&定义线性变换矩阵：T:U\rightarrow V为线性变换，\dim(U)=n,\dim(V)=m,
\\&B=\{u_1,\dots,u_n\}和C=\{v_1,\dots,v_m\}分别为U和V的基，
\\&设T的相对于基B和C的矩阵Q_{m\times n}=(Q_1|\dots|Q_n),
\\&\begin{cases}
T(u_1)=q_{11}v_1+\dots+q_{m1}v_m
\\\dots
\\T(u_n)=q_{1n}v_1+\dots+q_{mn}v_m

\end{cases},\quad
Q_i=[T(u_i)]_C=\left[
    \begin{array}{c}
        q_{1i} \\
        \cdots \\
       q_{ni}
    \end{array}
\right],i=1,\dots,m
\\&系数矩阵，只写系数，不写基向量
\\2.&表示定理：从一般向量空间转变为坐标向量，则线性变换T的作用变为乘以他的矩阵表示

\\&若u是U中的向量且T(u)=v,则Q[A]_B=[p(x)]_C,且Q唯一

\end{align}
$$

### 基变换与对角化

- 可对角化变换

	- 

$$
\begin{align} 1.&定义线性变换矩阵：T:V\rightarrow V为线性变换，\dim(V)=n,
\\&则T相对于基B的矩阵为对角矩阵D=\left[
    \begin{array}{c}
        d_1&0&\dots&0 \\
        0&d_2&\cdots &0 \\
       \vdots&\vdots&&\vdots\\
0&0&\cdots&d_n
    \end{array}
\right],i=1,\dots,m
\\2.&若T为线性变换，矩阵表示为对角形，则T称可对角化的
\\3.&向量空间V中存在非零向量v，使得T(v)=\lambda v,
\\&则\lambda 称为线性变换 T:V\rightarrow V 的特征值，v是 T对应于\lambda的特征向量
\\4.&V为n维向量空间，当且仅当存在V的一组基由T的特征向量组成时，T可对角化
\end{align}
$$

- 过渡矩阵与基变换

	- 

$$
\begin{align} &设B=\{u_1,\dots,u_n\}和C为向量空间V的基，
\\&则P为非奇异矩阵,对V中每个向量v,有[v]_C=[I_V(v)]_C=P[v]_B
\\&(即B的每个分量用C的所有分量表示，写出系数矩阵)
\\&P称为过度矩阵，下标表示左行向量为该字母表示的基
\\&利用过渡矩阵表示不同基B和C矩阵表示的关系
\\\\&若Q_1、Q_2是线性变换T关于B、C的矩阵
\\&则 Q_2=P^{-1}Q_1P,P是从C到B的过渡矩阵
\end{align}
$$

### 子主题 5

