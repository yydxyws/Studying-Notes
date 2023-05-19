# 抽象代数

## 基本概念

### 二元运算与同余关系

### 幺半群与群

### 子群与商群

### 环与域

### 同态与同构

### 模

### 同态基本定理

### 循环群

## 环

### 分式域

### 多项式环

### 对称多项式

### 唯一析因环

### 主理想整环与Euclid环

### 域上一元多项式

### 唯一析因环的整数环

### 素理想与极大理想

### 整数环与数域

- 代数运算性质
加法运算与乘法运算定义

	- 

$$
\begin{align} &基本公理
	\\&1.加法结合律
\\&	2.加法交换律
\\&	3.存在零元素：有整数0.0+a=a+0=a。
\\&	4.存在负元素：每个整数a，总有-a，使得a+(-a)=0
\\&	5.乘法结合律
\\&	6.乘法交换律
\\&	7.存在单位元素：有整数1，a1=1a=a。
\\&	8.加乘分配律
\end{align}
$$

- 环和域 

	- 若集合R中规定加法运算与乘法运算，适用以上基本公理，则集合R称为交换环。
	- 整数系是一个交换环，称为整数环，记为Z.另外有理数系、实数系、复数系均为交换环.

凡复数系子集合，对复数的乘法和加法成为交换环，则称为数环。
	- 

$$
\begin{align} &设\mathbb{F}是至少有两个元素的交换环，若对F中每个非零元素a，\\
&存在元素b∈\mathbb{F}，使得ab=ba=1，则b为a的逆元素，记作a⁻¹。\\
&该交换环称为域。\\
&例如，有理数系、实数系、复数系都是域，依次称为有理数域、实数域\\&和复数域\mathbb{Q,R,C}。若复数域\mathbb C子集合\mathbb F对复数加法与乘法成为一个\\&域，则称\mathbb {F}为数域。
\end{align}
$$

		- 有理数系、实数系和复数系均是域，称为有理数域、实数域、复数域。
		- 若复数域C子集合F对复数的加法和乘法成为一个域，则F称为数域

- 一元多项式环

	- 

$$
\begin{align} &设a_i\in\mathbb F ,a_n\ne0,则f(x)=a_n x^n+a_{n-1}x^{n-1}+…+a_1x+a_0
\\&称为数域\mathbb F上的一元多项式。f(x)的全体集合记为\mathbb F[x].a_n为f(x)的首项系数，
\\&a_n=1为首一多项式,非负整数n称为f(x)次数，记为\deg f(x).
\\&若多项式f(x)系数全为0，称之为零多项式，次数为-\infty,又称纯量多项式。
\end{align}
$$
	- 

$$
\begin{align} &多项式加法有：\deg(f(x)+g(x))\le\max\{\deg f(x),\deg g(x)\}
\\&多项式乘法有：\deg(f(x)g(x))=\deg f(x)+\deg g(x)
\\&存在纯量多项式e(x)=1,使得f(x)e(x)=e(x)f(x)=f(x)
\\&…根据定义，\mathbb{F}[x]是交换环，称为数域\mathbb F的一元多项式环。 
\end{align}
$$

### 整除性与最大公因式

- 带余除法

	- 

$$
\begin{align} & 带余除法：设多项式 f(x),g(x) ∈F[x].g(x)≠0．则存在唯一
\\&一对多项式 q(x),r(x)∈F[x],\deg r(x)<\deg g(x)
\\&使得f(x)=q(x)g(x)+r(x).q(x)和r(x)分别称为商式与余式
\end{align}
$$
	- 

$$
\begin{align} &特例-剩余定理：
\\&设f(x)\in\mathbb F(x),a\in\mathbb F,则存在唯一q(x)\in\mathbb F[x],使得f(x)=(x-a)q(x)+f(a)
\end{align}
$$
	- 

$$
\begin{align} &Euclid长除法：「f(x)=q(x)g(x)+r(x)」\\
&给定多项式f(x)与g(x),g(x)\ne0,求商式q(x)与余式r(x)。
\\&\quad当\deg f(x)<\deg g(x)，有q(x)=0,r(x)=f(x)
\\&\quad当\deg f(x)\ge \deg g(x),记f(x)-\frac{a_n}{b_m}x^{n-m}g(x)=f_1(x)
\\&\qquad如果\deg f_1(x)<\deg g(x),则f(x)=\frac{a_n}{b_m}x^{n-m}g(x)+f_1(x)
\\&\qquad如果\deg f_1(x)\ge \deg g(x),f_1(x)的首项系数c_t\ne0,t<\deg f(x)
\\&\qquad则记f_1(x)-\frac{c_t}{b_m}x^{t-m}g(x)=f_2(x).
\\&\qquad\quad若\deg f_2(x)<\deg g(x),则f(x)=(\frac{a_n}{b_m}x^{n-m}+\frac{c_t}{b_m}x^{t-m})g(x)+f_2(x)
\\&\qquad\quad若\deg f_2(x)\ge\deg g(x),则重复上述过程…
\\&\quad经过有限步后，必有\mathscr l,使得\deg f_\mathscr l(x)<\deg g(x)
\\&\quad有f(x)=(\frac{a_n}{b_m}x^{n-m}+\frac{c_t}{b_m}x^{t-m}+…)g(x)+f_\mathscr l(x)

\end{align}
$$

- 多项式的整除性

	- 

$$
\begin{align} &多项式的整除性-定义：
\\&设非零多项式g(x)\in\mathbb F[x]，若存在q(x)\in\mathbb F(x)，使得多项式f(x)=g(x)q(x)，
\\&则多项式g(x)称为f(x)的一个因式，多项式f(x)称为g(x)的一个倍式。
\\&此时称多项式g(x)整除多项式f(x)，记为g(x)|f(x),否则称g(x)\nmid f(x)
\end{align}
$$
	- 

$$
\begin{align} &性质
\\&1.若g(x)|f(x)，h(x)|g(x),则h(x)|f(x)
\\&2.若g(x)|f_1(x)，g(x)|f_2(x),则对任意h_1(x),h_2(x)\in\mathbb F (x),g(x)|\big(h_1(x)f_1(x)+h_2(x)f_2(x)\big)
\\&3.若g(x)|f(x)，f(x)|g(x)，则存在非零数\lambda\in\mathbb F,使得f(x)=\lambda g(x)
\\&推论（因式定理）：设f(x)\in\mathbb F(x),a\in\mathbb F，则当且仅当f(a)=0时,(x-a)|f(x)

\end{align}
$$

- 最大公因式

	- 

$$
\begin{align} &定义：设f_1(x),f_2(x)不全为零，若首一多项式d(x)是f_1(x)和f_2(x)的公因式，
\\&\qquad且f_1(x)与f_2(x)每个公因式都是d(x)一个因式，则称d(x)为最大公因式，
\\&\qquad记为d(x)=\bigg(f_1(x),f_2(x)\bigg)
\\&定理：任意两个不全为零的多项式f_1(x),f_2(x)的最大公因式d(x)存在且唯一
\\&定理：d(x)是f(x)与g(x)的最大公因式，则存在多项式u(x),v(x)\in\mathbb F[x]，
\\&\qquad使得f(x)u(x)+g(x)v(x)=d(x)
\\&推论：对f(x),g(x)，所有零次多项式都是他们的公因式。若f(x),g(x)除
\\&\qquad零次多项式外不含其他公因式，则f(x),g(x)互素。
\\&推论：多项式f(x),g(x)互素，当且仅当存在u(x),v(x)使得f(x)u(x)+g(x)v(x)=1
\\&性质：\bigg(f(x),g(x)\bigg)=1, \bigg(f(x),h(x)\bigg)=1,则\bigg(f(x),g(x)h(x)\bigg)=1
\\&性质：\bigg(g(x),h(x)\bigg),h(x)|f(x)g(x),则h(x)|f(x)
\\&性质：f(x)|h(x)，g(x)|h(x)，且\bigg(f(x),g(x)\bigg)=1,则f(x)g(x)|h(x)

\end{align}
$$
	- 辗转相除法

### 唯一析因定理

- 

$$
\begin{align} &1.引言：在整数环\mathbb Z中，素数指除\pm1和自身之外不含其他因子的整数。
\\&整数环\mathbb Z中每个非零整数都可以唯一分解为若干素数乘积，不计素因子正负号顺序。
\\&2.不可约定义：
\\&设f(x)是数域\mathbb F的n次多项式，n\ge1.如果存在次数小于n的多项式
\\&g(x),h(x)\in\mathbb F[x]，使得f(x)=g(x)h(x)，则多项式f(x)称为在\mathbb F上可约.
\\&若多项式f(x)不是在\mathbb F上可约，则f(x)称为在\mathbb F上不可约,但在\mathbb K上可能可约。
\\&3.在\mathbb F上不可约多项式p(x)简单性质：
\\&(1)若a是\mathbb F中非零的数，则ap(x)在\mathbb F上不可约
\\&(2)若多项式f(x)\in\mathbb F[x]，则p(x)|f(x)\bigg(f(x)能被p(x)整除,p(x)称为f(x)的
\\&\quad不可约因式\bigg),或者p(x)与f(x)互素
\\&(3)若f(x),g(x)\in\mathbb F[x],且p(x)|f(x)g(x),则p(x)|f(x)或p(x)|g(x)
\\&(4)*唯一析因定理*：设n次多项式f(x)\in\mathbb F[x]，
\\&\quad则存在数域\mathbb F上的不可约多项式p_i(x)\in\mathbb F[x]，使得f(x)=\prod_{i=1}^s p_i(x)，
\\&\quad如果另有不可约多项式q_i\in\mathbb F[x]，使得f(x)=\prod_{i=1}^t q_i(x)，则s=t，
\\&\quad并且可以适当调整因式次序，使得q_i(x)=a_ip_i(x)，其中a_i\in\mathbb F,i=1,2,…,s
\\&表述：若不计不可约因式的次序和零次因式，每个多项式都可以唯一分解成不可约因式乘积


\end{align}
$$

### 实系数与复系数多项式

- 

$$
\begin{align} &1.定理：数域\mathbb F上的n次多项式f(x)在\mathbb F上至多有n个不同的根，其中n>0
\\&2.代数基本定理：任意一个n次复系数多项式一定有复数根，其中n\ge1
\\&3.复系数多项式唯一析因定理：设f(x)是任意一个n次复系数多项式，n>0,则f(x)恰有n个复数
\\&\quad根c_1,c_2,…,c_n,且f(x)=a_0(x-c_1)(x-c_2)…(x-c_n)
\\&推论：复系数多项式p(x)在复数域\mathbb C不可约的充分必要条件是\deg p(x)=1
\\&4.实系数多项式的复数根共轭成对出现。
\\&5.实系数多项式f(x)在实数域上不可约，则f(x)的次数为1或2.	其充要条件是判别式p^2-4q<0
\\&6.n次实系数多项式f(x)可分解为一次因式和二次不可约因式的乘积，即
\\&\quad f(x)=a_0\times(x-c_1)^{k_1} (x-c_2)^{k_2} …(x-c_s)^{k_s}\times (x^2+p_1x+q_1)^{e_1} (x^2+p_2x+q_2)^{e_2}… (x^2+p_tx+q_t)^{e_t}
\\&\quad其中k_i,e_j 均正整数，1\le i\le s,1\le j\le t,\quad\sum k_i+2\sum e_t=n。
\\&\quad c_i和p_j,q_j均为实数，且p^2_j-4q_j<0.

\end{align}
$$
- 

$$
\begin{align} &整系数与有理系数多项式
\\&1.若整系数多项式的系数最大公因子为1，则称之为本原多项式。
\\&每个整系数多项式都可以表示成系数的最大公因子和本原多项式的乘积。
\\&高斯引理：任意两个本原多项式的乘积是本原多项式。
\\&2.设n次整系数多项式f(x)在\mathbb Z上不可约，则f(x)在\mathbb Q不可约。
\\&\quad f(x)相对于整数环\mathbb Z和有理数域\mathbb Q不可约性是相同的。
\\&唯一析因定理：不计因式次序和符号，n次整系数多项式f(x)可以
\\&\qquad唯一分解为一个整数和若干个本原不可约多项式乘积。
\\&3.Eisenstein判别准则
\\&设f(x)=a_0+a_1x+…+a_nx^n\in\mathbb Z[x]，如存在素数p，
\\&使得p|a_i(i=0,1,…,n-1)，但p\nmid a_n,且p^2\nmid a_0,则f(x)在\mathbb Z上不可约。

\end{align}
$$

### 多元多项式环

- 

$$
\begin{align} &定义：设\mathbb N 是所有非负整数的集合，记\mathbb N^n=\{(k_1,k_2,…,k_n)\mid k_1,k_2,…k_n\in\mathbb N\}
\\&\qquad a_{k_1…k_n}\in \mathbb F,则a_{k_1…k_n}x_1^{k_1}…x_n^{k_n}称为数域\mathbb F上的n元单项式，\sum_{i=1}^n k_i为次数，a_{k_1…k_n}为系数
\\&定义：设M是集合\mathbb N^n的有限子集合，则f(x_1,…,x_n)=\sum_{(k_1,…,k_n)\in M} a_{k_1…k_n}x_1^{k_1}…x_n^{k_n}
\\&\qquad称为数域\mathbb F上的n元多项式，其中a_{k_1…k_n}\in\mathbb F.所有单项式的最高次数称为多项式的次数，
\\&\qquad记为\deg f，a_{k_1…k_n}称为项a_{k_1…k_n} x_1^{k_1}…x_n^{k_n}的系数.
\\&所有数域\mathbb F上的n元多项式集合记为\mathbb F[x_1,…,x_n]
\\&依据字典排列法写出所有的展开项，从角标最小、次数最高开始依次向后写
\\&基本定理验证得，\mathbb F[x_1,…,x_n]为数域\mathbb F上的n元多项式环


\end{align}
$$

### 对称多项式

- 

$$
\begin{align} &1.定义：设f(\boldsymbol x)\in\mathbb F[\boldsymbol x]，若对自然数1,2,…,n任意排列i_1i_2…i_n，都有
\\&\qquad f(x_{i_1},x_{i_2},…,x_{i_n})=f(x_1,x_2,…,x_n)，则称f(x_1,x_2,…,x_n)为n元对称多项式
\\&例如：\sigma_1=\sum_{1\le i_1\le n}x_{i_1},\quad\sigma_2=\sum_{1\le i_1<i_2\le n}x_{i_1}x_{i_2}…
\\&\qquad…\sigma_k=\sum_{1\le i_1<…<i_k\le n}x_{i_1}x_{i_2}…x_{i_k},\quad …\quad\sigma_n=x_1x_2…x_n
\\&以上称为n元基本对称多项式。
\\&2.对称多项式基本定理：
\\& 设f(\boldsymbol x)\in\mathbb F[\boldsymbol x]，则存在唯一的多项式g(\boldsymbol x)\in\mathbb F[\boldsymbol x]，使得f(\boldsymbol x)=g(\boldsymbol \sigma),
\\&其中\sigma_1,\sigma_2,…,\sigma_n是数域\mathbb F的n元对称多项式
\\&常常将对称多项式表示为关于基本对称多项式\sigma_i的多项式。
\\&3.Vieta定理：
\\&设数域\mathbb F上的n次多项式f(x)=\sum_{i=0}^n a_ix^i的根为c_1,…,c_n，
\\&则对于k=0,…n，有a_k=(-1)^{n-k}\cdot\sigma_{n-k}(\boldsymbol c),其中a_n=1,\sigma_0(\boldsymbol c)=1.
\\&4.Newton恒等式：
\\&当k\ge n时，\sum_{i=0}^n (-1)^i\sigma_i  s_{k-i}=0(\sigma_0=1)
\\& 当k< n时，\sum_{i=0}^k(-1)^i\sigma_i  s_{k-i}=0(\sigma_0=1)

\end{align}
$$

## 群论

### 概论（引言）

- 研究自然现象中的对称性，研究产生和破缺的演化规律。每一种对称性都和某种特定的变换有关。系统的研究各种变换之间普遍联系规律的数学是群论。

	- 数学上，将两种情况间通过确定的规则对应起来的关系，称作从一种情况到另一种情况的变换
	- 物理学上，如果某一现象或系统在某一变换下不改变，则说该现象或系统具有该变换对应的对称性

### 群和群表示

### 希尔伯特空间和算符

### 有限群的表示理论

- 群的生成组
- 群在集合上的作用
- Sylow子群
- 有限单群
- 群的直积

### 连续群及其表示

- 李群和李代数

	- 李代数的结构与分类
	- 李群的表示

### 物理中的应用

- 粒子物理中的应用

	- 整体对称性
	- 强子的内禀对称性
	- 味SU（N）整体对称性
	- 等效相互作用分析
	- 定域规范不变性

- 量子力学中的群论
- 固体物理中的群论

### 可解群与幂零群

### Jordan- Holder定理

### 自由幺半群与自由群

### 点群

## 域

### 域的单扩张

### 有限扩张

### 分裂域与正规扩张

### 可分多项式与完备域

### 可分扩张与本原元素

### 代数学基本定理

## 模

### 自由模

### 模的直和

### 主理想整环上的有限生成模

### 主理想整环上的有限生成扭模

### 主理想整环上的有限生成模的应用

### 主理想整环上的矩阵

## Galois理论

### Galois基本理论

### 一个方程的群

### 分圆域与二项方程

### 有限域

### 方程的根式解

