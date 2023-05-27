# 形式理论

## 厄米算符的本征函数
（可观测量的确定态）

### 希尔伯特空间

- 所有在特定区域平方可积函数的集合构成的矢量空间称希尔伯特空间。
波函数存在于希尔伯特空间。

### 可观测量与厄米算符

- 可观测量（力学量）由厄米算符表示
- 可观测量Q的确定值态是Q的本征函数
- 谱的简并：多个线性独立本征函数具有相同本征值
- 性质:厄米算符=共轭算符+转置算符

$$
\begin{align} &\Braket{\Psi|\hat Q \Psi}=\Braket{\hat Q\Psi|\Psi}

\end{align}
$$
- 宇称算符

	- 只有两个本征态，本征值是描述粒子在空间反演下对称性质的量子数

$$
\begin{align} &\hat P r\hat P=-r,\quad\hat P\hat H(r,p)\hat P=\hat H(-r,-p) ,\quad [\hat P,\hat H]=0
\\&满足V(-x)=V(x)的任意两个方程的解都可以组合成奇或偶宇称解
\\证明：&若\psi(x)与\psi(-x)线性相关,
\\&\psi(x)=C\psi(-x)=C^2\psi(x),C=\pm 1,分别具有奇偶宇称
\\&若\psi(x)与\psi(-x)线性无关，
\\&令\phi=\psi(x)+\psi(-x)偶宇称,\chi=\psi(x)-\psi(-x)奇宇称
\end{align}
$$

### 分立谱

- 【实数性】
厄米算符本征函数，本征值为实数。
- 【正交性】
厄米算符不同本征值的本征函数正交。
相同本征值的本征函数线性组合依然具有相同本征值。
在每个简并子空间，可以利用施密特正交化构建正交本征函数。

	- 球谐函数相互正交

- 【完备性】
希尔伯特空间中任意函数都可以用厄米算符本征函数的线性组合表示。
可观测量算符（厄米算符）的本征函数是完备的。

### 连续谱

- 狄拉克正交归一性

	- 

$$
\Braket{\psi|\psi}=\delta(p-p')
$$

- 动量算符和坐标算符

	- 

$$
\begin{align} 1.&动量算符
\\&动量算符本征态为平面波，本征值连续取值构成连续谱
\\&本征函数：f_p(x)=\frac{1}{\sqrt{2\pi\hbar}}e^{\frac{i}{\hbar}px},满足\Braket{f_{p'}|f_p}=\delta(p-p')
\\&完备性：f(x)=\int c(p)f_p(x)dp=\frac{1}{\sqrt{2\pi\hbar}}\int c(p)e^{\frac{i}{\hbar}px} dp
\\&展开系数:c(p')=\Braket{f_{p'}|f}=\int c(p)\Braket{f_{p'}|f_p}dp=\int c(p)\delta(p-p') dp
\\&动量空间波函数：c(p)=\Braket{f_p|\Psi}=\frac{1}{\sqrt{2\pi\hbar}}\int e^{-\frac{i}{\hbar}px}\Psi(x,t)dx
\\&与坐标空间波函数互为傅里叶变换
\\&动量分布概率：|\Phi(p,t)|^2dp
\\2.&坐标算符
\\&本征值为连续实数，本征函数为狄拉克函数
\\&坐标分布概率：|\Psi(y,t)|^2dy

\end{align}
$$

- 箱归一化

	- 

$$
\int \psi_p^*\psi_p d\tau=\frac{1}{L^3}\int_{-\frac{L}{2}}^{\frac{L}{2}} dx\int_{-\frac{L}{2}}^{\frac{L}{2}} dy \int_{-\frac{L}{2}}^{\frac{L}{2}} dz=1\Rightarrow \begin{cases}\psi_p=\frac{1}{L^{\frac{3}{2}}} e^{\frac{i}{\hbar}p\cdot r} \\\psi_p^*=\frac{1}{(2\pi\hbar)^{\frac{3}{2}}}e^{-\frac{i}{\hbar}p\cdot r}
\end{cases}
$$

- 动量的径向分量量子化

	- 

$$
\begin{align} &动能分解：T=\frac{p_r^2}{2m}+\frac{L^2}{2mr}
\\&\hat p_r=-i\hbar(\frac{\partial }{\partial r}+\frac{1}{r}),\quad [\hat r,\hat p_r]=i\hbar
\\&\hat p_r^2=-\hbar^2(\frac{\partial }{\partial r}+\frac{1}{r})^2=-\hbar^2\frac{1}{r^2}\frac{\partial }{\partial r} r^2\frac{\partial }{\partial r}





\end{align}
$$

## 表象和矩阵表示

### 坐标表象与动量表象

- 

$$
\begin{align} 1.&坐标表象(实空间)：x\delta(x-x_0)=x_0\delta(x-x_0),p=-i\hbar\frac{\partial }{\partial x},\psi_p(r)=(\frac{1}{\sqrt{2\pi\hbar}})^3e^{\frac{i}{\hbar}p\cdot r}
\\&动量表象(相空间)：p\delta(p-p_0)=p_0\delta(p-p_0),x_p=i\hbar\frac{\partial }{\partial p},c_r(p)=(\frac{1}{\sqrt{2\pi\hbar}})^3e^{-\frac{i}{\hbar}p\cdot r}
\\2.&考虑离散情况，取有物理意义的厄米算符构成对易完备组K，
\\&用共同本征矢量作为作为基矢K\ket{i}=k_i\ket{i}.i表示完备组中各算符本征值序号的集合.
\\&取定这样的一组基矢称为取一个表象（K表象）.
\\&
空间任意矢量都可以按基矢展开：
\ket{\psi}=\sum_i \ket{i}\Braket{i|\psi}=\sum_i a_i\ket{i},
\\&态矢\ket\psi在K表象中的波函数（矢量\psi在基矢\ket{i}上的分量）：a_i=\Braket{i|\psi} 

\end{align}
$$

### 态、算符和方阵的矩阵表示

- 

$$
\begin{align} 1.&态的矩阵表示：投影矢量（系数）的列矩阵\ket n，共轭矩阵：行矩阵\bra n,\boldsymbol\Psi
\\&\Psi(x,t)=\sum_n a_n(t)u_n(x)+\int a_q(t) u_q(x) dq,\quad\sum_n a_n^*a_n+\int a_q^* a_q dq=1
\\2.&算符的矩阵表示：厄米矩阵元\boldsymbol F_{mn}=\int u_n^*(x)\hat F(x,\frac{\hbar}{i}\frac{\partial }{\partial x}) u_m(x)dx=\Braket{n|\hat F|m}
\\&u_n为PQ两种态中的共同本征函数，算符在自身表象中为对角矩阵
\\3.&公式的矩阵表示：
\\&期望值公式：\bar F=\int\Psi^*\hat F\Psi dx=\sum_{mn}a_m^*\cdot F_{mn}\cdot a_n=\boldsymbol{\Psi^+ F\Psi}
\\&本征值方程：\hat F\Psi(x,t)=\lambda \Psi(x,t)\rightarrow\sum_n(\boldsymbol F_{mn}-\lambda\boldsymbol\delta_{mn})a_n(t)=0
\\&久期方程：\det|\boldsymbol F_{mn}-\lambda\boldsymbol\delta_{mn}|=\left |\begin{array} &F_{11}-\lambda &F_{12}&\cdots &F_{1n}\\F_{21}&F_{22}-\lambda&\cdots &F_{2n}\\\cdots&\cdots&\cdots &\cdots\\F_{n1}&F_{n2}&\cdots &F_{nn}-\lambda\end{array}\right |=0
\\&薛定谔方程：i\hbar \frac{d\sum a_m(t)}{dt}=\sum_n \boldsymbol H_{mn}a_n(t)
\\&\qquad \Rightarrow i\hbar\frac{d}{dt}
\left [\begin{array} &a_1(t)\\a_2(t)\\\dots\\a_m(t)\end{array}\right ]=
\left [\begin{array} &H_{11}&H_{12}&\cdots &H_{1n}\\H_{21}&H_{22}&\cdots &H_{2n}\\\cdots&\cdots&\cdots &\cdots\\H_{m1}&H_{m2}&\cdots &H_{mn}\end{array}\right ]\left [\begin{array} &a_1(t)\\a_2(t)\\\dots\\a_n(t)\end{array}\right ]
\end{align}
$$

### 变换的矩阵表示
求矩阵元

- 

$$
\begin{align} 1.&矩阵元的变换：算符\hat F的矩阵元\begin{cases}
已知A表象：F_{mn}=\int \psi_m^*\hat F\psi_n dx
\\未知B表象：F'_{ij}=\int \phi_i^*\hat F\phi_j dx\end{cases}
\\&将未知波函数\phi(x)按已知\psi(x)展开\begin{cases}
\phi_i=\sum_m \psi_m^* \cdot S_{mi}^*\\
\phi_j=\sum_n S_{nj}\cdot \psi_n
\end{cases}

\\&\rightarrow
\begin{cases}
\boldsymbol\Phi^+=\boldsymbol\Psi^+\boldsymbol S\\ \boldsymbol\Phi=\boldsymbol S^T \boldsymbol\Psi
\end{cases},\qquad \begin{cases}
S_{nk}=\int\psi^*_n\phi_j dx\\
S_{mi}^*=\int \phi_m^*\phi_i^* dx
\end{cases}
\\&S^+=S^{-1}，厄米矩阵等于逆矩阵，S即幺正矩阵,作幺正变换
\\2.&态矢量\Psi(x,t)=\sum u(x,t)的变换：即求\phi_i(x)的展开系数b_i(t)
\\&b_i(t)=\int \phi_i^* u(x,t)dx=\sum_m \int\Psi_m^* S_{mi}^* u(x,t)dx
\\&\qquad =\sum_m S_{mi}^* a_m=\sum_m (S^+)_{im} a_m=(S^+a)_i，即b=S^+a
\\3.&幺正变换：从表象A到B的表象变换。幺正矩阵不是厄米矩阵
\\&变换公式：F'=S^{-1}FS=F^+FS,\quad b=S^{-1}a=S^+ a

\\&幺正变换不改变算符本征值和矩阵F的迹，但改变本征矢

\end{align}
$$

### 狄拉克符号与表示

- 

$$
\begin{align} &不依赖于坐标系，量子态用希尔伯特空间矢量\ket {s(t)}替代波函数表示，可以用任意基表示。
\\&\ket {s(t)}\begin{cases}用坐标本征函数\ket {x}展开得到波函数\Psi(x,t)&\Psi(x,t)=\Braket{x|s(t)}\\
用动量本征函数\ket {p}展开得到动量空间波函数\Phi(x,t)&\Psi(x,t)=\Braket{p|s(t)}\\
用分立能量本征函数\ket {n}展开得到系数集合C_n(t)&C_n(t)=\Braket{n|s(t)}
\end{cases}
\\&以上是描述同一个态的三种途径

\end{align}
$$
- 

$$
\begin{align} 
&投影算符\hat P=\ket{\alpha}\bra{\alpha},\hat P\ket{\beta}=\ket{\alpha}\Braket{\alpha|\beta}，(\ket{\alpha}\bra{\beta})^*=\ket{\beta}\bra{\alpha}
\\&\hat P作用于任意态\ket{\psi}上，得到\ket{\psi}在基矢\ket{\phi_i}上投影的线性组合

\\&利用基矢展开有:\sum_n\ket{n}\Braket{{n}|\psi}=\ket \psi，展开系数：\Braket{n|\psi}=\int dx\Braket{n|x}\Braket{x|\psi}
\\&封闭性关系式：\begin{cases}
能量本征态：\sum_n\ket n\bra n=1\\
动量本征态：\int dp\ket p \bra p =1\\
位置本征态：\int dx\ket x \bra x=1
\end{cases}
\\&\ket{S(t)}=\begin{cases}
\sum_n\ket n\bra n\ket{S(t)}=\sum c_n(t)\ket n\\
\int dp\ket p \bra p\ket{S(t)} =\int\Phi(p,t)\ket p dp\\
\int dx\ket x \bra x\ket{S(t)}=\int \Psi(x,t)\ket x dx
\end{cases}
\\&各自的波函数，实际上是希尔波特空间矢量使用不同的基的展开系数

\end{align}
$$
- 

$$
\begin{align} 本征态：&位置空间\Psi(x,t)=\Braket{x|s(t)}到动量空间\Phi(x,t)=\Braket{p|s(t)}波函数变换：
\\&\Phi(p,t)=\Braket{p|s(t)}=\Braket{p|\bigg(\int dx\ket x\bra x\bigg)|s(t)}=\int\Braket{p|x}\Psi(x,t)dx
\\&\Braket{x|p}是用位置基表示的动量本征态，称为f_p(x),已经由狄拉克归一化得出
\\&则\Braket{p|x}=\Braket{x|p}^*=[f_p(x)]^*=\frac{1}{\sqrt{2\pi\hbar}}e^{-\frac{i}{\hbar}px}
\\算符：&\begin{cases}
动量表象中的位置算符：\Braket{p|\hat x|{s(t)}}\\
位置表象中的位置算符：\Braket{x|\hat x|s(x)}
\end{cases}
\\&\Braket{p|\hat x|{s(t)}}=\Braket{p|\hat x\bigg(\int dx\ket x\bra x\bigg)|{s(t)}}=\int\Braket{p|x|x}\Braket{x|s(t)}dx
\\&\qquad \int x\Braket{p|x}\Psi(x,t)dx=\int x\frac{e^{-\frac{i}{\hbar}px}}{\sqrt{2\pi\hbar}}\Psi(x,t)dx=i\hbar\frac{\partial }{\partial p}\int \frac{e^{-\frac{i}{\hbar}px}}{\sqrt{2\pi\hbar}}\Psi(x,t)dx



\end{align}
$$
- 

$$
\begin{align} &狄拉克表示：（左矢说明了所在表象）
\\&算符作用于态A得到态B：\Braket{\alpha |B}=\sum_n \Braket{\alpha| F|n}\Braket{n|A}
\\&坐标表象单位1：\int\ket x dx\bra x=1,\begin{cases}
\ket n=\int\ket x dx\Braket{x |n}\\
\bra \alpha=\int\Braket{ m| x'}dx' \bra{x' }
\end{cases}
\\&算符x表象矩阵元表达：\Braket{x'| \hat F|x}=\hat F(x',p')\delta(x-x')
\\&算符非x表象矩阵元表达：\Braket{\alpha| \hat F|n}=\int\Braket{\alpha|x}\hat F(x,p) dx\Braket{x|n}
\\&算符作用的简单表达\ket B=\hat F\ket A,\bra B=\bra A \hat F^+
\\&薛定谔方程：i\hbar\frac{\partial }{\partial t}\Braket{x|\Psi}=\Braket{x|H|\Psi}\rightarrow H\ket n=E_n\ket n

\end{align}
$$

### 有限个线性独立态体系

- 二态系统

	- 中微子振荡
	- 所有指定态用完备的归一化本征矢量组的线性组合表示

## 广义统计诠释
和相关定理

### 可观测量

- 力学量期待值是对含有相同体系的一个系综中不同体系重复测量平均值，而不是对同一个体系的重复测量的平均值。
- 

$$
\begin{align} &力学量A 的平均值:
\bar{A}=\frac{\sum_{i}|c_i|^2a_i}{\sum_{i}|c_i|^2}=\frac{\sum_{i}\Braket{\psi|a_i}\Braket{a_i|\psi}a_i}{1}=\sum_{i}\bra\psi A \ket {a_i}\Braket{a_i|\psi}=\bra \psi A  \ket\psi
\\&含变量A的函数期望值：\overline {f(A)}=\sum_i |c_i|^2 f(a_i)=\sum_i\Braket{\psi|f}\Braket{f|\psi}f(a_i)=\Braket{\psi|f(A)|\psi}

\end{align}
$$

### 波包运动与
埃伦费斯特定理
（力学量演化规律）

- 

$$
\begin{align} &\frac{d \braket F}{dt}=\frac{1}{i\hbar}\Braket{ [\hat F,\hat H]}+\Braket{\frac{\partial \hat F}{\partial t}}

\\&[\hat F,\hat H]=\hat F\hat H-\hat H\hat F。逐项求导，带入含时薛定谔方程可证。
 \\&若F不显含t,\frac{\partial F}{\partial t}=0,则\frac{d\bar{F}}{dt}=\frac{1}{i\hbar}\overline{[\hat F,\hat H]}
\\&若F与H对易,[\hat F,\hat H]=0：F为一个守恒量. 
\\&三维：\frac{d}{dt}\Braket{ r}=\frac{1}{m}\braket{p},\quad \frac{d}{dt}\braket {p}=\Braket{-\nabla V}
\end{align}
$$

### （赫尔曼-费因曼）
Hellmann-Feynman定理

- 

$$
\begin{align} &若\hat H\psi_n=E_n\psi_n,\lambda为中的任意参数，则有
\\&\frac{\partial E_n}{\partial \lambda}=\frac{\partial (\psi_n^* \hat H\psi_n d\tau)}{\partial \lambda}=\int\psi_n^*\frac{\partial \hat H}{\partial \lambda}\psi_n d\tau,即\Braket{\frac{\partial \hat H}{\partial \lambda}}_n=\frac{\partial E_n}{\partial \lambda}

\end{align}
$$

### 能级简并与
位力（Virial）定理
（动能与势能）

- 

$$
\begin{align} &埃伦费斯特定理中\hat F=\boldsymbol r\cdot \boldsymbol p\Rightarrow 定态下\frac{d}{dt}\Braket{\boldsymbol r\cdot \boldsymbol p}=0
\\&\Rightarrow  2\langle T\rangle=\langle \boldsymbol r\cdot\nabla V\rangle,\braket T=\Braket{\frac{\hat p^2}{2m}}
\end{align}
$$

## 对易关系和不确定原理

### 对易关系

- 

$$
\begin{align} &[\hat u,\hat v]=-[\hat v,\hat u],\quad[\hat u,c\hat I]=0,\quad[\hat u+\hat w,\hat v]=[\hat u,\hat v]+[\hat w,\hat v]
\\&[\hat u\hat w,\hat v]=[\hat u,\hat v]\hat w+\hat u[\hat w,\hat v],\quad[\hat u,\hat v\hat w]=[\hat u,\hat v]\hat w+\hat v[\hat w,\hat u]
\\&[u,[v,w]]+[v,[w,u]]+[w,[u,v]]=0
\\&连接对易关系与泊松括号：[\hat u,\hat v]=D\Set{u,v},D=i\hbar
\\&基本对易关系：[\hat x,\hat p_x]=i\hbar
\\&常用对易关系：[r_i,p_j]=-[p_i,r_j]=i\hbar\delta_{ij},\quad [r_i,r_j]=[p_i,p_j]=0
\end{align}
$$
- 等价关系：（可推广到多个算符）
两算符满足对易关系 
两算符对应力学量相互独立
两算符有一组组成完全系的共同本征函数ψn
- 完备共同本征态完全集完全确定体系的状态，这组相互对易的力学量个数即体系的自由度。
不考虑自旋的三维空间自由粒子（氢原子电子）自由度为3

### 广义不确定原理

- 

$$
\begin{align} &两算符不对易时，不能同时具有确定值:[\hat F,\hat G]=i\hat k
\\1.&设积分I(\xi)=\int|(\xi\Delta \hat F-i\Delta\hat G)\psi|^2 d\tau\ge 0,\xi为实参数
\\&均方偏差:\sigma^2=\Braket{(\Delta x)^2}=\Braket{x^2}-\braket x ^2
\\&利用厄米算符性质及二次方程代数性质：\overline{(\Delta\hat F)^2}\cdot\overline{(\Delta\hat G)^2}\ge\frac{k^2}{4}
\\2.&均方偏差:\sigma^2=\Braket{\big(\hat Q -\braket Q\big)^2}=\Braket{\Psi|(\hat Q-q)^2\Psi}=\Braket{(\hat Q-q)\Psi|(\hat Q-q)\Psi}
\\&\sigma_F^2\sigma_G^2=\Braket{f|f}\Braket{g|g}\ge|\Braket{f|g}|^2施瓦茨不等式、复数取模、厄米性质
\\&\sigma_F^2\sigma_G^2\ge\bigg(\frac{1}{2i}\Braket{[\hat F,\hat G]}\bigg)^2


\end{align}
$$

### 能量-时间不确定原理

- 根据埃伦费斯特定理，可导出能量时间不确定原理

$$
\begin{align} &\Delta E=\sigma_H,\Delta t=\frac{\sigma _Q}{|\frac{d\Braket{Q}}{dt}|}代入广义不确定原理即可
\\&\sigma _Q=|\frac{d\Braket{Q}}{dt}|\Delta t,\Delta t表示Q的期望值变化一个标准差所需时间
\\&定态极端情况，\Delta t\rightarrow \infty
\end{align}
$$

## 对称性和守恒律

### 平移算符

- 

$$
\begin{align} &
平移算符：\hat T(\boldsymbol a)\psi(\boldsymbol r)=\psi(\boldsymbol r-\boldsymbol a)
\\&在x处泰勒展开：\hat T(a)\psi(x)=\psi(x-a)=\sum_{n=0}^{\infty} \frac{1}{n!}(-a)^n\frac{d^n}{dx^n}\psi(x)=\sum_{n=0}^{\infty} \frac{1}{n!}\bigg(\frac{-ia}{\hbar}\hat p\bigg)^n\psi(x)
\\&平移算符用动量算符表示：\hat T(a)=\sum_{n=0}^{\infty} \frac{1}{n!}\bigg(\frac{-ia}{\hbar}\hat p\bigg)^n=e^{-\frac{ia}{\hbar}\hat p},是酉变换:\hat T(a)^{-1}=\hat T(-a)=\hat T(a)^+
\\&算符变换：\Braket{\psi'|\hat Q|\psi '}=\Braket{\psi|\hat Q'|\psi }=\Braket{\psi|\hat T^\dagger\hat Q\hat T|\psi }\Rightarrow \hat Q'(\hat x,\hat p)=\hat T^\dagger\hat Q(\hat x,\hat p)\hat T=\hat Q(\hat x+a,\hat p)
\\&系统具有平移对称性\Rightarrow [\hat H,\hat T]=0，离散的平移对称性是布洛赫定理前提。
\\&连续平移对称性说明动量守恒：[\hat H,\hat T(\delta)]=[\hat H,1-i\frac{\delta}{\hbar}\hat p]=0\Rightarrow [\hat H,\hat p]=0



\end{align}
$$

### 宇称算符

- 

$$
\begin{align} 宇称算符：&\hat \Pi\psi(\boldsymbol r)=\psi(-\boldsymbol r),\begin{cases}
\hat \Pi\psi(r,\theta,\phi)=\psi(r,\pi-\theta,\phi+\pi)\\
\hat\Pi\psi_{nlm}(r,\theta,\phi)=(-1)^l\psi_{nlm}(r,\theta,\phi)
\end{cases}
\\一维：&同理满足酉变换：\hat Q'(\hat x,\hat p)=\hat \Pi^\dagger\hat Q(\hat x,\hat p)\hat \Pi=\hat Q(-\hat x,-\hat p),且[\hat H,\hat \Pi]=0
\\&结论：对位置对称的一维势的定态本身就是奇函数或偶函数，且宇称守恒
\\&对一维归一化束缚态，不存在简并性，对称势的每个束缚态即宇称的本征态，散射除外
\\三维：&伪向量pseudovectors在奇偶校验下不会改变符号：\{\hat \Pi,\hat {\boldsymbol V}\}=0,例如角动量L
\\&伪标量pseudoscalar在奇偶校验下改变符号：\{\hat \Pi,\hat f\}=0
\\&三维空间V(r)=V(-r)的粒子哈密顿量都具有反演对称性（任意中心势均满足）



\end{align}
$$
- 

$$
\begin{align} &选择规则：根据对称情况判断矩阵元何时为0
\\&矩阵元：\Braket{b|\hat Q|a},期望值：a=b=\psi
\\&电偶极矩算子：\hat{\boldsymbol p_e}=q\hat{\boldsymbol r},\Pi^\dagger\hat{\boldsymbol p_e}\hat \Pi=-\hat{\boldsymbol p_e},选择规则决定了哪些原子跃迁允许，哪些禁止
\\&拉波特Laporte规则：偶极矩算符矩阵元在具有相同奇偶性的状态之间为0
\\&\quad\Braket{n'l'm'|\hat{\boldsymbol p_e}|nlm}=-\Braket{n'l'm'|(-1)^{l'}\hat{\boldsymbol p_e}(-1)^l|nlm}=(-1)^{l+l'+1}\Braket{n'l'm'|\hat{\boldsymbol p_e}|nlm}
\\&\quad 则l+l'为偶数时\Braket{n'l'm'|\hat{\boldsymbol p_e}|nlm}=\boldsymbol 0
\\&Laporye规则适用于奇偶校验下任何奇算符

\end{align}
$$

### 旋转算符

- 

$$
\begin{align} &关于z轴旋转算符：\hat R_z(\varphi)\psi(r,\theta,\phi)=\psi(r,\theta,\phi-\varphi)\Rightarrow \hat R_z(\varphi)=e^{-\frac{i\varphi}{\hbar}\hat L_z}
\\&使用算符无穷小形式：\hat R_z(\delta)\approx 1-\frac{i\delta}{\hbar}\hat L_z
\\&则\hat x'=\hat R^\dagger \hat x\hat R\approx \hat x+\frac{i\delta}{\hbar}[\hat L_z,\hat x]\approx \hat x-\delta \hat y，同理\hat y'=\hat y+\delta\hat x,\hat z'=\hat z
\\&矩阵方程：\left [ \begin{matrix}
\hat x'\\
\hat y' \\
\hat z'
\end{matrix} \right ]
=\left [ \begin{matrix}
1&-\delta&0\\
\delta&1&0 \\
0&0&1
\end{matrix} \right ]
\left [ \begin{matrix}
\hat x\\
\hat y \\
\hat z
\end{matrix} \right ]
\xrightarrow[\varphi\rightarrow \delta ]{\cos\varphi\rightarrow 1,\sin\varphi\rightarrow 0}
\left [ \begin{matrix}
\hat x'\\
\hat y' \\
\hat z'
\end{matrix} \right ]
=\left [ \begin{matrix}
\cos\varphi&-\sin\varphi&0\\
\sin\varphi&\cos\varphi&0 \\
0&0&1
\end{matrix} \right ]
\left [ \begin{matrix}
\hat x\\
\hat y \\
\hat z
\end{matrix} \right ]

\end{align}
$$
- 

$$
\begin{align} &绕坐标轴沿着单位向量n的三维旋转算符：\hat R_z(\varphi)=e^{-\frac{i\varphi}{\hbar}{\boldsymbol{n\cdot\hat L}}}
\\&线性动量是平移的产生子，角动量是旋转的产生子generator
\\&则\hat V_x'=\hat R^\dagger \hat x\hat R\approx \hat x+\frac{i\delta}{\hbar}[\hat L_z,\hat x]\approx \hat x-\delta \hat y，同理\hat y'=\hat y+\delta\hat x,\hat z'=\hat z
\\&矩阵方程：\left [ \begin{matrix}
\hat V_x'\\
\hat V_y' \\
\hat V_z'
\end{matrix} \right ]

=\left [ \begin{matrix}
\cos\varphi&-\sin\varphi&0\\
\sin\varphi&\cos\varphi&0 \\
0&0&1
\end{matrix} \right ]
\left [ \begin{matrix}
\hat V_x\\
\hat V_y \\
\hat V_z
\end{matrix} \right ]，[\hat L_i,\hat V_j]=i\hbar \varepsilon_{ijk}\hat V_k
\\&\dots\dots\\&对中心势场，角动量守恒是旋转不变性的结果

\end{align}
$$
- 
- 

$$
\begin{align} &Wigner-Eckart 魏格纳-艾卡特定理：陈述旋转选择规则
\\&标量算子\hat f：\Braket{n'l'm'|\hat f|nlm}=\delta_{ll'}\delta_{mm'}\Braket{n'l\|f\|nl},\|f\|称约化矩阵元
\\&向量算子\hat {\boldsymbol V}：
\begin{cases}
\Braket{n'l'm'|\hat V_+|nlm}=-\sqrt 2C_{m1m'}^{l1l'}\Braket{nl'\|V\|nl}\\
\Braket{n'l'm'|\hat V_-|nlm}=\sqrt 2C_{m\text{-1}m'}^{l1l'}\Braket{nl'\|V\|nl}\\
\Braket{n'l'm'|\hat V_z|nlm}=C_{m0m'}^{l1l'}\Braket{nl'\|V\|nl}
\end{cases}
\\&\quad C_{m_1m_1M}^{j_1j_2J}即CG系数
\\&\quad 当且仅当\begin{cases}
\Delta l=0,\pm1 \\ \Delta m=0,\pm1
\end{cases},向量算符的任意分量的矩阵元非零
\\&\dots

\end{align}
$$

### 对称性与简并

- 

$$
\begin{align} &若存在定态\ket{\psi_n}，则\ket{\psi_n'}=\hat Q\ket{\psi_n}是具有相同能量的定态
\\&多个非交换对称算符的存在保证了能谱的简并性
\\&\dots
\end{align}
$$

### 时间平移算符

- 

$$
\begin{align} &时间平移算符：\hat U(t)\Psi(x,0)=\Psi(x,t),\quad
\hat U(t)=e^{-\frac{i}{\hbar}\hat Ht}
\\&用于简化求解H与时间无关的含时薛定谔方程
\\&\Psi(x,t)=\hat U(t)\Psi(x,0)=\sum_n c_n\hat U(t)\psi_n(x)=\sum_n c_n e^{-\frac{i}{\hbar}E_n t} \psi_n(x)
\\&时间平移不变性：能量守恒
\end{align}
$$

### 薛定谔图像、海森堡图像

- 

$$
\begin{align} &海森堡绘景：\hat Q_{H}(t)=\hat U^\dagger(t)\hat Q\hat U(t)，i\hbar\frac{d}{dt}\hat Q_H(t)=[\hat Q_H(t),\hat H]
\\&将时间平移算符应用于算子与波函数，变换后算符即海森堡绘景算子
\\&海森堡绘景中，波函数在时间上是常数：\Psi_H(x)=\Psi(x,t)
\\&并且算符按海森堡算符变换公式随时间演化
\\
\\&薛定谔绘景：\hat H\Psi(x,t)=i\hbar\frac{\partial }{\partial t}\Psi(x,t)
\\&波函数随时间的演化遵循薛定谔方程，算符本身没有时间依赖性，
\\&期望值的时间依赖性来自于波函数:\Braket{\hat Q}=\Braket{\Psi(t)|\hat Q|\Psi(t)}
\\\\&二者完全等价：\Braket{\Psi(t)|\hat Q|\Psi(t)}=\Braket{\Psi(0)|\hat U^\dagger\hat Q\hat U|\Psi(0)}=\Braket{\Psi_H|\hat Q_H(t)|\Psi_H}

\end{align}
$$

