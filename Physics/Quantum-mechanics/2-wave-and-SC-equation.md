# 波函数与薛定谔方程

## 波函数

### 量子论基础

- 德布罗意公式及其意义
- 光子相关公式
- 黑体辐射
- 波尔-索末菲量子论
- 不确定原理

	- 

$$
\sigma_x\sigma_p\ge \frac{\hbar}2{}
$$

### 波恩波函数的统计诠释

- 波函数在空间某点强度与该点找到粒子几率成正比。描写粒子的波是概率波，波函数描写体系的量子状态

### 归一化与概率守恒原理

- 

$$
\frac d {dT}\int_{-\infty}^{\infty}|\Psi(x,t)|^2dx=0
$$

## 定态薛定谔方程
（量子静力学）

### 不含时：系统哈密顿量与时间无关
定态：不含时系统能量的本征态，粒子几率密度不随时间变化，体系能量有确定值
束缚态：粒子被束缚于势阱，能级离散
散射态：粒子能级连续

### 定态方程

- 

$$
\begin{align} 力学量：&p=-i\hbar\nabla=\frac{h}{i}\nabla，E=i\hbar \frac{\partial }{\partial t}，H=-\frac{\hbar^2}{2m}\nabla^2+U(r)
\\期待值：&\braket p=\int\Psi^*(\frac{\hbar}{i}\frac{\partial }{\partial x})\Psi dx,\quad \braket Q=\int\Psi^*Q(x,\frac{\hbar}{i}\frac{\partial }{\partial x})\Psi dx,
\\多粒子薛定谔方程：&i\hbar\frac{\partial \Psi}{\partial t}=-\sum_{i=1}^{N}\frac{\hbar^2}{2m_i}\nabla_i^2\Psi+U\Psi
\\定态方程：&-\frac{\hbar^2}{2m}\frac{d^2\psi}{d x^2}+V\psi=E\psi
\\第n个定态波函数：&\psi_n(\boldsymbol r,t)=\psi_n(r)e^{-\frac{i}{\hbar}E_n t},\int|\psi|^2=1
\\含时薛定谔方程一般解：&\Psi(\boldsymbol r,t)=\sum_n c_n\psi_n(\boldsymbol r),\int|\Psi|^2=1
\\&体系初始时刻状态完全决定以后任意时刻状态
\\初始波函数t=0：&\Psi(\boldsymbol r,0)=f(r)=\sum_n c_n\psi_n(\boldsymbol r)
\\傅里叶系数：&c_n=\int \psi_n^*(\boldsymbol r)f(\boldsymbol r)d\boldsymbol r

\end{align}
$$

### 定态方程解的性质

- 1.分离变量得到的解是定态的，具有确定的总能量。
2.分离变量解的概率值和期待值都不依赖时间。
3.一般解是分离变量解的线性组合，并且含时指数因子不能相互抵消。
- 定态方程两类解（无限远处势能与粒子能量判据）
可归一化的解：无限远处E<V(±∞)，仅允许束缚态
不可归一化的解：无限远处E>V(∞)或E>V(-∞)，仅允许散射态

1.对归一化的解，分离变量常数E一定是实数。
2.定态波函数总可以通过线性组合得到实数解
3.如果势函数为偶函数，则波函数总是可以取作奇函数或偶函数，即有确定宇称。
（实质上是定态波函数相对于对称势的势阱中心是奇偶交替的）
4.定态方程所有归一化的解都有E>V的最小值恒成立，否则不能够归一化
5.定态波函数随着能量增加，与x轴节点数逐次增1
6.定态波函数满足正交归一性和完备性（任意函数都可以用定态波函数线性组合表示）。

### 动量分布概率

- 

$$
\begin{align} &
在一般情况下, \Psi 可看作许多平面单色波叠加而成,即含有各种波长(动量)的分波,
\\&令\omega=|c(\boldsymbol p,t)|^2 表示粒子的动量分布的概率密度,即动量分布函数
\\& 任意波函数 按动量傅里叶展开: \Psi (\boldsymbol r,t)=\int_\Omega c(\boldsymbol p,t)\Psi_p(r)dV_p，p为连续变量
\\&\quad动量为p的平面波函数：\Psi_p(\boldsymbol r)=\frac{1}{(2\pi\hbar)^{\frac{3}{2}}} e^{\frac{i}{\hbar} \boldsymbol p\cdot\boldsymbol  r}，\frac{1}{(2\pi\hbar)^{\frac{3}{2}}}为归一化因子
\\&\quad展开系数(概率幅)：c(\boldsymbol p,t)=\int \Psi(r,t)\Psi_p(r) dV=\frac{1}{(2\pi\hbar)^{\frac{3}{2}}} \int \Psi(\boldsymbol r,t)e^{\frac{i}{\hbar} \boldsymbol p\cdot\boldsymbol  r}dV_r
\end{align}
$$

### 粒子数守恒与刘维尔方程

- 

$$
\begin{align} &\frac{\partial \omega}{\partial t}+\nabla\cdot \boldsymbol J=0
\\&\frac{\partial }{\partial t}\int \omega\cdot d\tau+\oint_S\boldsymbol J\cdot d\boldsymbol S=0
\\&\boldsymbol  J=-\frac{i\hbar}{2m}(\Psi^*\nabla\Psi-\Psi\nabla \Psi^*)
\\&刘维尔方程：\frac{\partial \hat \rho}{\partial t}=\frac{1}{i\hbar}[\hat H(t),\hat\rho]

\end{align}
$$

### 一维势场性质

- 振荡定理:对离散谱的波函数，属于第(n+1)个能级En的本征函数ψn(x)共有n次等于零（对x为有限值而言）.
- 如势阱突然扩大，波函数不能瞬间变化，但算符H已瞬间变化。未知波函数用已知完备波函数展开求所占概率
- 一维情况不存在简并束缚态

## 量子力学基本原理

### 1.微观体系被一个波函数Ψ完全描述【波函数公式】

### 2.力学量用厄米算符表示，且组成力学量的厄米算符有组成完全系的本征函数【算符公式】

### 3.体系波函数Ψ用算符F的本征函数φ展开，则在态Ψ中测量力学量F，得到结果一定为厄米算符本征值，其中λn的概率为|Cn|^2，在λ→λ+δλ范围内概率为|Cλ|^2dλ【测量公式/广义统计诠释】

- 对任意态测量力学量F得到结果λn，体系的量子态就会坍缩到对应的本征矢上，简并态则坍缩到对应的本征子空间。
- |cn|2是处于Ψ态的粒子在测量Q值后将处于fn态的概率

### 4.体系状态的波函数满足薛定谔方程（量子态随时间的演化遵循薛定谔方程）【微观体系动力学演化公式】

### 5.全同粒子组成的体系中，两全同粒子调换不改变体系状态【全同性原理】

