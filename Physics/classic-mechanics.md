# **分析力学**

## 拉格朗日动力学

### 分析力学基础

- 各种坐标系下动力学方程

	- 

- 约束问题

	- 主动力与约束力、保守力与非保守力
	- 自由度与广义坐标，张成位形空间

		- 极坐标中广义力对应力矩

- 为了抛掉一切约束力

	- 虚位移：只需约束许可，无运动方程和时间制约
虚功：任意力沿虚位移做功，实际是变分符号δr
理想约束：约束使得约束反力总虚功为零
虚功原理：平衡时主动力虚功也为零
位形空间平衡条件：广义力为零
	- 广义坐标变换：

$$
\delta r^{(a)}=\sum_j\frac{\partial r^{(a)}}{\partial q_j}\delta q_j
$$
	- 平衡稳定性：二阶导数判定
	- 例题

		- 

- 达朗贝尔原理

	- 将加速度力变为惯性力，转为静力学问题
	- 动力学普遍方程：

$$
\delta W=\sum_a\bigg(F_{主}^{(a)}-m^{(a)} \ddot r^{(a)}\bigg)\cdot \delta r^{(a)}=0
$$

### 拉格朗日方程

- 广义坐标形式的动力学普遍方程

	- 

$$
\frac{d}{dt}\bigg(\frac{\partial L}{\partial \dot q_j}\bigg)-\frac{\partial L}{\partial q_j}=Q_{非保守力}
$$
	- 体系只有保守力作用

$$
\frac{d}{dt}\bigg(\frac{\partial L}{\partial \dot q_j}\bigg)=\frac{\partial L}{\partial q_j}
$$
	- 牛顿力学中的拉格朗日量：L=T-V
	- 两个拉格朗日关系式：利用坐标变换得到

$$
\frac{\partial \dot r_i}{\partial \dot q_k}=\frac{\partial r_i}{\partial q_k},\quad \frac{\partial \dot r_i}{\partial  q_k}=\frac{d}{dt}\bigg(\frac{\partial r_i}{\partial q_k}\bigg)
$$

- 坐标系中的运动方程

	- 

$$
\begin{align} &在极坐标系，平面上自由粒子合外力在r,\phi方向
\\&\frac{d}{dt}\bigg(\frac{\partial L}{\partial \dot r}\bigg)-\frac{\partial L}{\partial r}=Q_r=F_r
\\&\frac{d}{dt}\bigg(\frac{\partial L}{\partial \dot \phi}\bigg)-\frac{\partial L}{\partial \phi}=Q_\phi=rF_\phi
\\&L=T=\frac{1}{2}m(\dot r^2+r^2\dot\phi^2)
\\&F_r=m(\ddot r-r\dot \phi^2),\quad F_\phi=m(r\ddot\phi+2\dot r\dot\phi)
\\&在球坐标系，广义力分别为Q_r=F_r,Q_\theta=rF_\theta,Q_\phi=r\sin \theta F_\phi
\end{align}
$$

- 例题

	- 

### 应用

- 解决耗散情形，加入耗散函数G
- RLC电路，广义坐标为电荷量q

## 最小作用量原理

### 泛函分析与变分法
（质点如何选择最优路径）

- 

$$
\begin{align} &变分：\Delta S=S[y(x)+\delta y]-S[y(x)]=\delta S+o(\delta y)
\\&微分：\Delta y=y(x+\Delta x)-y(x)=dy+o(\Delta x)
\\&变分原理：若泛函S(y)在函数y=y(x)上达到极值，
\\&\qquad\qquad则在函数y=y(x)上变分\delta S为0

\\&导函数的变分等于变分的导函数：\delta y'=(\delta y)'
\\&泛函数S的变分：
\\&\qquad\delta S=\int_a^b \delta f(y,y')dx=\int_a^b \bigg(\frac{\partial f}{\partial y}\delta y +\frac{\partial f}{\partial y'}\delta y' \bigg)dx

\\&又第二项\int_a^b\frac{\partial f}{\partial y'}\delta y' dx=\int_a^b\frac{\partial f}{\partial y'}d(\delta y) 

=\frac{\partial f}{\partial y'}\delta y \bigg|_a^b-\int_a^b\frac{d}{dx}\frac{\partial f}{\partial y'}\delta ydx
\\&\Rightarrow \quad \delta S=\frac{\partial f}{\partial y'}\delta y \bigg|_a^b

+\int_a^b\bigg(\frac{\partial f}{\partial y}-\frac{d}{dx}\frac{\partial f}{\partial y'}\bigg)\delta ydx
\\&S取极值意味着对任意\delta y，都有\delta S=0，又\delta y(a)=\delta y(b)=0
\\& \Rightarrow \quad \frac{\partial f}{\partial y}-\frac{d}{dx}\frac{\partial f}{\partial y'}=0(欧拉方程)
\end{align}
$$
- 函数：数集X→数集Y
泛函：函数集Y(x)→作用量S
微分：曲线上数微小变动左右游移，dx
变分：整条曲线形状改变，δy
求泛函的极值，实际是求函数y(x)的具体形式
变分、微分、积分可交换

### 不依赖于牛顿力学重建拉式方程
（质点路径如何加权表示）

- 费马原理：光总是选择耗时最短路径（光程最短）（光程是平稳值）

$$
L=\int_C n d l\quad\Rightarrow\quad dL=0
$$

	- 自然规律应当能写成令泛函S取极值（使作用量变分为零）的形式。

$$
\begin{align} &S=\int_C f d t\quad\Rightarrow\quad \delta S=0
\\&其中f满足欧拉方程：\frac{\partial f}{\partial q}-\frac{d}{dt}\bigg(\frac{\partial f}{\partial \dot q}\bigg)=0
\\&其中f=f(q_j,\dot q_j,t)，完整决定体系运动
\end{align}
$$

		- 物理体系的作用量取法 + 欧拉拉格朗日方程
       →具体运动方程 + 物理规律……
微分视角与积分视角

- 定义惯性系：保证物理规律在时空中均匀
限制f性质满足：
时间平移不变性（时刻）：不显含时间t
空间平移不变性（地点）：不显含空间坐标q
空间旋转不变性（方向）：依赖速度大小而非方向

$$
f只可能的形式：f=f(\dot q^2)
$$

	- 质点和质点系伽利略变换：

$$
\begin{align} &***对于单个质点的f：
\\&S系：\dot q(=v)，f=f(v^2)，S'系：v'=v+\varepsilon，f'=f(v'^{2})
\\&
泰勒展开：f'=f\bigg((v+\varepsilon)^2\bigg)=f\bigg(v^2+2v\cdot \varepsilon+\varepsilon^2\bigg)=f(v^2)+\frac{\partial f}{\partial(v^2)}2v\cdot \varepsilon

\\&要求f代入欧拉方程结果相同：f'=cf，f'=f+\frac{d}{dt}f_0(q,t)
\\&要求\frac{\partial f}{\partial(v^2)}2v\cdot \varepsilon与速度成线性关系，能够表达为时间全导数形式
\\&定义\frac{\partial f}{\partial(v^2)}=\frac{m}{2}，m定义为自由质点质量，f=\frac{1}{2}mv^2
\\\\&***对于质点系的f：
\\&如果各质点相互作用为保守力，f只会和质点坐标有关：
\\&f(q,\dot q)=\sum_a\bigg(\frac{1}{2}m^{(a)}\big(v^{(a)}\big)^2\bigg)-V\bigg(q^{(1)},q^{(2)},\dots\bigg)
\\&若受外力作用，V可能显含t
\end{align}
$$

- f=T-V,即体系拉格朗日量。
泛函+自然最简法则+物理规律对称性→E-L方程

$$
\boldsymbol{\frac{\partial L}{\partial q}-\frac{d}{dt}\bigg(\frac{\partial L}{\partial \dot q}\bigg)=0}
$$

	- 力学体系的作用量即拉格朗日量对时间积分：

$$
S=\int_{t_1}^{t_2} L(\boldsymbol q,\boldsymbol {\dot q},t) dt
$$

		- 作用量沿轨道对时间的全导数：

$$
dS=Ldt\Rightarrow\quad\frac{dS}{dt}=L
$$

### 最小作用量原理
（第一性原理地位）

- 本意：一切物理过程都可以转化为某种作用量S的极值问题，在完成同一件事的多种路径中，真正路径与其对应的作用量泛函是否恰好取到极值有关。

	- 亚里士多德：任何系统都有自己的第一性原理，这是一个根基性的命题假设，不能被缺省也不能被违反。

- 哈密顿原理
（一种表述）

	- 

$$
\begin{align} &\boldsymbol{
\delta S=\delta\bigg(\int_{t_1}^{t_2}L(q,\dot q,t)dt\bigg)=0}
\\&\delta S=\int_{t_1}^{t_2}\bigg(\frac{\partial L}{\partial q}\delta q+\frac{\partial L}{\partial \dot q}\delta \dot q\bigg)dt
\\&\quad=\int_{t_1}^{t_2}\bigg(\frac{\partial L}{\partial q}-\frac{d}{dt}\frac{\partial L}{\partial \dot q}\bigg)\delta qdt=0

\end{align}
$$
	- 保守的、完整的力学体系在相同时间内，从某一初位形转移到另一位形的一切可能运动中，真实运动必然是使得作用量具有平稳值的运动。
	- 变分为零说明是平稳值：极大、极小、常量。
一般情况下，真实运动的路径就是作用量最小的路径。

### 诺特定理

- 对于每一种连续对称性，都会有一个守恒量与之对应。
- 根据对称性选择坐标系，能得到某些循环坐标和对应的广义动量守恒。

	- 拉格朗日量不显含广义坐标，则对该坐标求导为零，即循环坐标。代入拉格朗日方程，得广义动量守恒

- 只要一项物理规律是基于最小作用量原理而建立的，那么若是作用量有一种对称性则体系就有一种守恒量，反之若体系有一种守恒量则作用量就有一种对称性。
- 具有镜面反演对称性的称作极矢量，不具备的称为赝矢量/轴矢量，其本身描述平面内事物，只是约定记作矢量。

### 对称性与守恒量关系

- 对称性破缺

	- 宇称不守恒，CP守恒/破却，CPT守恒，生物分子手性，对称性自发破缺……

- 空间平移对称性——动量守恒

	- 要求L不能显含空间位置。
循环坐标（L不显含）对应的广义动量守恒。

$$
\begin{align} &\sum_a\frac{\partial L}{\partial q^{(a)}}=0\quad\Rightarrow \quad \frac{d}{dt}\bigg(\sum_a\frac{\partial L}{\partial \dot q^{(a)}}\bigg)=0
\\&广义动量：p_j=\frac{\partial L}{\partial \dot q}
\end{align}
$$

- 空间旋转对称性——角动量守恒

	- 

$$
\begin{align} &用\mathbb L表示拉氏量
\\&在直角坐标系中微小转动：\delta r=\delta \phi\times r,\delta v=\delta \phi\times v
\\&拉氏量变化：\delta \mathbb L=\sum_{(a)}\int_{t_1}^{t_2}\bigg(\frac{\partial \mathbb L}{\partial r}\delta r+\frac{\partial \mathbb L}{\partial v}\delta v\bigg)dt
\\&\qquad =\sum_{(a)}\int_{t_1}^{t_2}\bigg(\frac{\partial \mathbb L}{\partial r}(\delta \phi\times r)+\frac{\partial \mathbb L}{\partial v}(\delta \phi\times v)\bigg)dt
\\&\qquad=\delta \phi\cdot\sum_{(a)}\bigg[r\times\frac{\partial \mathbb L}{\partial r}+v\times \frac{\partial \mathbb L}{\partial v}\bigg]（矢量积公式）
\\&\qquad=\delta \phi\cdot\sum_{(a)}\bigg[r\times\frac{d}{dt}\bigg(\frac{\partial \mathbb L}{\partial v}\bigg)+\frac{d}{dt}\bigg(r\bigg)\times \frac{\partial \mathbb L}{\partial v}\bigg]

\\&\qquad=\delta \phi\cdot\frac{d}{dt}\sum_{(a)}\bigg(r\times\frac{\partial \mathbb L}{\partial v}\bigg)=\delta \phi\cdot\frac{d}{dt}\sum_{(a)}\bigg(r^{(a)}\times p^{(a)}\bigg)
\\&\Rightarrow \frac{d L}{dt}=0 \quad(体系总角动量守恒)
\end{align}
$$

- 时间平移对称性——能量守恒

	- 

$$
\begin{align} &不显含t的L关联t变换：\frac{d L}{d t}=\sum_j\bigg(\frac{\partial L}{\partial q_j}\frac{d q_j}{d t}+\frac{\partial L}{\partial \dot q_j}\frac{d \dot q_j}{d t}\bigg)
\\&\qquad=\sum_j\bigg[\dot q_j\frac{d }{d t}\bigg(\frac{\partial L}{\partial q_j}\bigg)+\frac{d }{d t}(\dot q_j)\frac{\partial L}{\partial \dot q_j}\bigg]=\frac{d }{d t}\bigg(\sum_j p_j\dot q_j\bigg)
\\&\Rightarrow \quad \frac{d }{d t}\bigg(\sum_j p_j\dot q_j-L\bigg)=0\quad \Rightarrow\quad \frac{dE}{dt}=0\quad(广义能量)
\\&经典力学体系下，E=\sum_j p_j\dot q_j-L=2T-(T-V)=T+V
\end{align}
$$

## 哈密顿动力学

### 建立哈密顿正则方程

- 追求数学对称性

	- 跳出经典力学，链接量子力学

$$
\begin{align} &保守完整系统：\frac{d}{dt}\bigg(\frac{\partial L}{\partial \dot q_j}\bigg)=\frac{\partial L}{\partial  q_j}
\\&方程并非是完美对称，q_j与\dot q_j张成抽象空间时两者乘积量纲不定
\\&利用广义动量替换速度确定量纲：p_jq_j\rightarrow[L]^2[T]^{-1}[M](能量\times时间)
\end{align}
$$
	- 勒让德变换

		- 

$$
\begin{align} 1.&单变量函数y=f(x),对任一点(x_0,y_0)利用斜率表示该点值:f(x)=f'(x)\cdot x+c(x)
\\&\qquad斜率：u=g(x)=\frac{df}{dx}=f'(x)\quad\Rightarrow x=[f'^{-1}](u)=g^{-1}(u)=x(u)
\\&\qquad截距：c(x)=y(x)-y'(x)\cdot x\quad\Rightarrow c\bigg(g^{-1}(u)\bigg)=y\bigg(g^{-1}(u)\bigg)-u\cdot\bigg(g^{-1}(u)\bigg)
\\&定义\widetilde f(u)为单变量函数f(x)的勒让德变换：\\&\qquad\widetilde f(u)=-c\bigg(x(u)\bigg)=u\cdot x(u)-f\bigg(x(u)\bigg)=u\cdot x-f(x)
\\&所有切线描绘的曲线边缘即函数f(x),将点与线信息关联
\\&微分几何语言描述就是切丛到余切丛的同构映射。
\\2.&二元函数f(x,y)的全微分：df=\frac{\partial f}{\partial x}dx+\frac{\partial f}{\partial y}dy=udx+vdy
\\&若从独立变量(x,y)到(u,v)，有x=x(u,v),y=y(u,v)
\\&\qquad\frac{\partial f}{\partial u}=\frac{\partial f}{\partial x}\frac{\partial x}{\partial u}+\frac{\partial f}{\partial y}\frac{\partial y}{\partial u}=u\frac{\partial x}{\partial u}+v\frac{\partial y}{\partial u}=\frac{\partial (ux)}{\partial u}-x+v\frac{\partial y}{\partial u}

\\&\qquad\frac{\partial f}{\partial v}=\frac{\partial f}{\partial x}\frac{\partial x}{\partial v}+\frac{\partial f}{\partial y}\frac{\partial y}{\partial v}=u\frac{\partial x}{\partial v}+v\frac{\partial y}{\partial v}=u\frac{\partial x}{\partial v}+\frac{\partial (vy)}{\partial v}-y
\\&\Rightarrow x=\frac{\partial (ux+vy-f)}{\partial u},\quad y=\frac{\partial (ux+vy-f)}{\partial v}
\\&\Rightarrow\widetilde f(u,v)是f(x,y)的Legendre变换:
\\&\qquad\widetilde f(u,v)=ux+vy-f(x,y)，其表示了切平面族
\\&对偶性质：\widetilde f(u,v)+f(x,y)=ux+vy=xf_x+yf_y
\\3.&多元函数的勒让德变换：
\\&\qquad \widetilde f(u_1,\dots,u_n)=\sum_{i=1}^n u_ix_i-f(x_1,\dots,x_n),\quad u_i=\frac{\partial f}{\partial x_i}
\\4.&部分变量勒让德变换：忽略不变的，累加变化的一对变量。
\\&例如F(Q,R)=f(Q,P)\pm PR
\end{align}
$$

	- 

$$
\begin{align} --&拉格朗日量到哈密顿量的转换
\\&L=L(\boldsymbol q,\boldsymbol {\dot q},t),\quad 
 \frac{\partial L}{\partial \dot q_i}=p_i,\quad \frac{\partial L}{\partial q_i}=\frac{d}{dt}\bigg(\frac{\partial L}{\partial \dot q_i}\bigg)=\frac{d}{dt}p_i=\dot p_i

\\& dL=\sum_i \frac{\partial L}{\partial q_i} dq_i+\sum_i\frac{\partial L}{\partial \dot q_i}d \dot q_i+\frac{\partial L}{\partial t}dt
=\sum_i \dot p_idq_i+\sum_i d( p_i \dot q_i)-\sum_i \dot q_i d p_i+\frac{\partial L}{\partial t}dt
\\&\Rightarrow利用勒让德变换取独立变量p_i,q_i：
\\&\Rightarrow dH=d\bigg(\sum_i  p_i \dot q_i-L(\boldsymbol q,\boldsymbol{\dot q},t)\bigg)=\sum_i \dot q_i d p_i-\sum_i \dot p_idq_i-\frac{\partial L}{\partial t}dt
\\&定义哈密顿量为\boldsymbol{H(\boldsymbol q,\boldsymbol{p},t)=\sum_i  p_i \dot q_i-L(\boldsymbol q,\boldsymbol{\dot q},t)},此即拉格朗日量的Legendre变换
\\&\Rightarrow dH=\sum_i\frac{\partial H}{\partial q_i}dq_i+\sum_i\frac{\partial H}{\partial p_i}dp_i+\frac{\partial H}{\partial t}dt，对比立即得到哈密顿正则方程！
\end{align}
$$

- 

$$
\begin{align} &哈密顿正则方程：（s个自由度，2S个一阶微分方程）
\\&\boldsymbol{\frac{\partial H}{\partial q_i}=-\dot p_i}，\qquad\boldsymbol{\frac{\partial H}{\partial p_i}=\quad\dot q_i},\qquad\bigg(\boldsymbol{\frac{\partial H}{\partial t}=-\frac{\partial L}{\partial t}}\bigg)
\\&(p_i,q_i)称为一对相互共轭的正则变量，二者地位相等,可互换
\end{align}
$$

	- 经典力学内等价于

		- H=T+V
		- 牛顿方程
		- 动力学普遍原理方程
		- 拉格朗日方程：（S个自由度，S个二阶微分方程）

	- H不显含q，对应的广义动量守恒。
H不显含t，体系能量守恒。

### 相空间中的哈密顿力学
(正则形式)

- s个广义坐标和s个广义动量组成2s维的相空间，其广泛应用于动力系统（按照一定规则随时间演化的系统）。

体系每个状态能够由相空间某个点代表，称为相点，其轨迹称为相轨，绘制相轨得到相（轨）图。

相体积元dΓ=Π dpi·dqi。

	- 
	- 

- 刘维尔定理

	- 相空间内某区域存在大量相点的分布，即系统运动状态的分布。

***保守体系中的相体积Γ不随时间演化而变化，始终守恒。

$$
\begin{align} &设相点密度为\rho=\rho(\boldsymbol q,\boldsymbol p,t),对整个相空间积分有\int \rho d\Gamma=N
\\&刘维尔定理：\frac{d\rho}{dt}=\frac{\partial \rho}{\partial t}+\sum_i \bigg(\frac{\partial \rho}{\partial q_i}\dot q_i+\frac{\partial \rho}{\partial p_i}\dot p_i\bigg)=0
\end{align}
$$

- 相空间的几何研究方法为微分几何，其形状称为流形，相空间是位形空间上的余切丛。
=牛顿力学——欧式空间——欧式几何——二阶微分方程——经典力学
=拉格朗日力学——位形空间——黎曼几何——s个二阶微分方程——广义相对论
=哈密顿力学——相空间——辛几何——2s个一阶微分方程——量子力学

### 泊松括号

- 力学量求导与微分

$$
\begin{align} &相空间任意力学量f=f(\boldsymbol q,\boldsymbol p,t),有
\\&\frac{df}{dt}=\frac{\partial f}{\partial t}+\sum_i \bigg(\frac{\partial f}{\partial q_i}\dot q_i+\frac{\partial f}{\partial p_i}\dot p_i\bigg)=\frac{\partial f}{\partial t}+\sum_i \bigg(\frac{\partial f}{\partial q_i}\frac{\partial H}{\partial p_i}-\frac{\partial f}{\partial p_i}\frac{\partial H}{\partial q_i}\bigg)
\\&泊松括号定义为：[f,H]=\sum_i \bigg(\frac{\partial f}{\partial q_i}\frac{\partial H}{\partial p_i}-\frac{\partial f}{\partial p_i}\frac{\partial H}{\partial q_i}\bigg)
\\&f对时间全导数改写为：\frac{df}{dt}=\frac{\partial f}{\partial t}+[f,H]

\end{align}
$$
- 泊松括号

$$
\begin{align} &任意两函数f、g泊松括号：
[f,g]=\sum_i \bigg(\frac{\partial f}{\partial q_i}\frac{\partial g}{\partial p_i}-\frac{\partial f}{\partial p_i}\frac{\partial g}{\partial q_i}\bigg)
\\&性质：[f,C]=0,\quad[f,g]=-[g,f],\quad [f,f]=0,
\\&\qquad [f,gh]=g[f,h]+[f,g]h，\quad [f,\sum_i C_ig_i]=\sum_i C_i [f,g_i], 
\\&\qquad 线性运算分配律：\frac{\partial }{\partial t}[f,g]=\bigg[\frac{\partial f}{\partial t},g\bigg]+\bigg[f,\frac{\partial g}{\partial t}\bigg]
\\&\qquad 雅可比恒等式：[f,[g,h]]+[g,[h,f]]+[h,[f,g]]=0
\\&特殊性质：[q_i,f]=\frac{\partial f}{\partial p_i},\quad [p_i,f]=-\frac{\partial f}{\partial q_i}
\\&\qquad[q_i,q_j]=0,\quad [p_i,p_j]=0,\quad [q_i,p_j]=\delta_{ij}
\\&哈密顿方程可改写为\dot p_i=[p_i,H],\quad \dot q_i=[q_i,H]
\\&两变量泊松括号为0，称为对易变量；结果为1，称为共轭正则变量

\end{align}
$$
- 泊松定理

$$
\begin{align} &根据1中知，\frac{df}{dt}=0时，[f,H]=-\frac{\partial f}{\partial t},同理，[g,H]=-\frac{\partial g}{\partial t}
\\&[f,[g,H]]+[g,[H,f]]+[H,[f,g]]=-[f,\frac{\partial g}{\partial t}]+[g,\frac{\partial f}{\partial t}]-[[f,g],H]=0
\\&\Rightarrow [[f,g],H]=-\frac{\partial [f,g]}{\partial t}，即[f,g]也是守恒量,此即泊松定理，
\\&已知两个守恒量，可利用泊松括号得到第三个守恒量
\\&一个不显含t的力学量f是守恒量\Longleftrightarrow [f,H]=0
\end{align}
$$

### 正则变换

- 目的：选择合适的坐标系，凑出尽可能多的循环坐标，使得解方程更轻松。即把一系列qi换成新的Qi，称为点变换。
- 哈密顿力学坐标q与动量p地位相等，所以可以同时将原本广义动量pi换成一系列新的广义动量Pi，实现了广义变换。

$$
\begin{align} &广义变换：P_i=P_i(\boldsymbol p,\boldsymbol q,t),\quad Q_i=Q_i(\boldsymbol p,\boldsymbol q,t),\quad [Q_i,P_i]=1

\\&P,Q同样满足哈密顿正则方程：
\\&\dot P_i=-\frac{\partial H'}{\partial Q_i},\quad \dot Q_i=\frac{\partial H'}{\partial P_i},\quad H'=H'(\boldsymbol P,\boldsymbol Q,t)
\\&P,Q为一对共轭的正则变量，满足以上要求称为正则变换

\end{align}
$$
- 

$$
\begin{align} &\delta S=\delta\bigg[\int_{t_1}^{t_2}L(\boldsymbol q,\boldsymbol {\dot q},t)dt\bigg]
=\delta\bigg[\int_{t_1}^{t_2}\bigg(\sum_i p_i\dot q_i-H(\boldsymbol p,\boldsymbol q,t)\bigg)dt\bigg]=0
\\&S=\delta\bigg[\int_{t_1}^{t_2}L'(\boldsymbol Q,\boldsymbol {\dot Q},t)dt\bigg]
=\delta\bigg[\int_{t_1}^{t_2}\bigg(\sum_i P_i\dot Q_i-H'(\boldsymbol P,\boldsymbol Q,t)\bigg)dt\bigg]=0
\\&即变换后的拉格朗日量依然满足最小作用量原理
\\&拉氏量积分后与t无关，则变分只对q,\dot q起作用，可平替为函数F对t全导数
\\&即：\bigg(\sum_i p_i\dot q_i-H\bigg)-\bigg(\sum_i P_i\dot Q_i-H'\bigg)=\frac{dF}{dt}
\\&\Rightarrow dF=\sum_i p_i d q_i-\sum_i P_i d Q_i+(H'-H)dt
\\&\Rightarrow dF(\boldsymbol q,\boldsymbol Q,t)=\sum_i\frac{\partial F}{\partial q_i}d q_i-\sum_i\frac{\partial F}{\partial Q_i}d Q_i+\frac{\partial F}{\partial t}dt
\\&利用正则变换的生成函数（母函数）F，有正则变换关系式：
\\&\boldsymbol {p_i=\frac{\partial F}{\partial q_i},\quad Q_i=-\frac{\partial F}{\partial Q_i},\quad H'=H+\frac{\partial F}{\partial t} }

\end{align}
$$
- 由于pq,PQ地位相等，则参数为“一旧一新一时间”四种类型，勒让德变换会有正负号变化
正则变换不改变泊松括号值：变换前后定义的[f,g]不变，可检验正则变换

### 哈密顿-雅可比方程

- 哈密顿-雅可比方程

	- 确定生成函数

		- 特殊生成函数使得新生成的哈密顿量H‘为0（最简），不显含任何坐标，即所有正则变量为常数（时间导数为0，守恒量）

			- 一阶偏微分方程的通积分与全积分
			- 利用分离变量法求解

	- 确定合适的正则变换

		- 让哈密顿量变得尽可能简单，能够凑出更多的循环坐标

	- 

$$
\begin{align} &根据正则变换关系式：H'=H+\frac{\partial F}{\partial t}=0，又\frac{\partial F}{\partial q_i}=p_i

\\&有(H-J)哈密顿-雅可比方程：H\bigg(\boldsymbol q,\frac{\partial F}{\partial \boldsymbol q},t\bigg)+\frac{\partial F(\boldsymbol q,\boldsymbol P,t)}{\partial t}=0

\end{align}
$$

- 作用量函数S

	- 

$$
\begin{align} &哈密顿主函数F，即作用量函数S(q,t)：H\bigg(\boldsymbol q,\frac{\partial S}{\partial \boldsymbol q},t\bigg)+\frac{\partial S}{\partial t}=0
\\&s个自由度有s+1个积分常数，函数S在方程中为偏导数，加减常数不影响结果，
\\&则方程全积分形式为:S=S(\boldsymbol q,t,\boldsymbol c)+C\quad(c为广义动量P)
\\&哈密顿主函数S随时间变化率为拉格朗日量L：\frac{dS}{dt}=\sum_i p_i\dot q_i-H=L
\end{align}
$$
	- 

$$
\begin{align} &S(\boldsymbol q,t)实际是积分上下限不定情况下的作用量，看做积分限中坐标的函数：
\\&\delta S=\delta \int_{t_1}^{t}Ldt

=\sum_i\frac{\partial L}{\partial \dot q}\delta q \bigg|_{t_1}^{t_2}

+\sum_i\int_{t_1}^{t_2}\bigg(\frac{\partial L}{\partial q}-\frac{d}{dt}\frac{\partial L}{\partial \dot q}\bigg)\delta qdt
\\&由于\delta q(t_1)=0，\delta q(t_2)=\delta q，\frac{\partial L}{\partial \dot q_i}=p_i

\\&\Rightarrow \delta S=\sum_i p_i\delta q_i \quad \Rightarrow \frac{\partial S}{\partial q_i}=p_i  \Rightarrow \quad\frac{dS}{dt}=\frac{\partial S}{\partial t}+\sum_i \frac{\partial S}{\partial q_i} \dot q_i=\frac{\partial S}{\partial t}+\sum_i p_i\dot q_i
\\&\Rightarrow 又\frac{dS}{dt}=L，得 \quad \frac{\partial S}{\partial t}=L-\sum_i p_i\dot q_i=-H 
\\&\Rightarrow dS=\sum_i p_i d q_i-Hdt=\bigg(\sum_i p_i d q_i-Hdt\bigg)^{(2)}-\bigg(\sum_i p_i d q_i-Hdt\bigg)^{(1)}
\\&\Rightarrow S=\int\bigg(\sum_i p_i d q_i-Hdt\bigg)
\end{align}
$$
	- 这说明任何情形下末态都不是初态的任意函数，不能用初态表示。
作用量能够写成全微分形式，运动才是可能的。
存在最小作用量原理与拉格朗日函数任何具体形式无关。

- 莫培督原理

	- 简约作用量

		- 

$$
\begin{align} &仅限定运动轨道，不涉及时间，建立更简单形式——简约作用量
\\&L不显含时间，则H不显含时间，系统能量守恒，H(p,q)=E=C
\\&末态时间变分：\delta S=-H\delta t\Rightarrow\quad \delta S+E\delta t=0
\\&最小作用量积分形式：S=\int\sum_i p_idq_i-E(t-t_0)=S_0-E(t-t_0)
\\&此处S_0=\int\sum_i p_idq_i=\int \boldsymbol{p\cdot dq}为简约作用量，满足\delta S_0=0

\end{align}
$$
		- 

$$
\begin{align} &简约作用量重要性质：
\\&考察一个所处环境随时间缓慢变化（体系特征时间内特征量变化极小）的粒子,
\\&其特征时间内相积分正比于简约作用量，即特征时间内相积分随时间近似守恒，
\\&近似守恒量J_i称为浸渐不变量或绝热不变量。
\\&（如非均匀小起伏场中周期运动粒子，周期内相积分J_i=\frac{1}{2\pi}\oint p_idq_i）

\end{align}
$$

	- 莫培督原理

		- 

$$
\begin{align} &莫培督原理：所有满足能量守恒且任意时刻过终点的轨道，简约作用量有极小值。
\\&雅可比原理：对简单质点，\delta S_0=\delta \bigg(\int\sqrt{2m(E-V)}ds\bigg)=0


\end{align}
$$

## 有心力场

### 有心力场运动轨道方程

- 寻找守恒量

	- 

$$
\begin{align} 
&质点仅受有心力作用，拉格朗日量：L=T-V=\frac{1}{2}m(\dot r^2+r^2\dot \phi^2)-V(r)
\\&L不显含\phi，\phi是循环坐标，与之对应的广义动量p_\phi=\frac{\partial L}{\partial \dot\phi}=mr^2\dot\phi守恒
\\&同理有能量守恒：E=T+V=\frac{1}{2}m(\dot r^2+r^2\dot \phi^2)+V(r)

\end{align}
$$

- 求解运动轨道

	- 

$$
\begin{align} 
&求解r:根据总动量守恒和总能量守恒（常数），消去导数项\dot r
\\&\dot r=\frac{dr}{dt}=\sqrt{\frac{2}{m}[E-V(r)]-\bigg(\frac{p_\phi}{mr}\bigg)^2}
\\&消去微分dt：根据p_\phi=mr^2\dot \phi,\frac{d\phi}{dt}=\frac{p_\phi}{mr^2}
\\&有运动轨道方程\phi(r)=\int\frac{p_\phi}{\sqrt{2m[E-V(r)]-(p_\phi r^{-1})^2}}\frac{dr}{r^2}+C
\\&令u=\frac{1}{r}，有\frac{du}{d\phi}=\frac{du}{dr}\frac{dr}{d\phi}=-\frac{1}{r^2}\frac{dr}{d\phi}
\\&改写轨迹微分方程得到：p_\phi\frac{du}{d\phi}=-\sqrt{2m[E-V(u)]-(p_\phi u)^2}
\\&p_\phi\frac{d^2u}{d\phi^2}=
\frac{m\frac{dV}{d\phi}+p_\phi^2u\frac{du}{d\phi}}{\sqrt{2m[E-V(u)]-(p_\phi u)^2}}=\frac{m\frac{dV}{d\phi}+p_\phi^2u\frac{du}{d\phi}}{-p_\phi\frac{du}{d\phi}}=-\frac{m}{p_\phi}\frac{dV}{du}-p_\phi u
\\&\frac{dV}{du}=\frac{dV}{dr}\frac{dr}{du}=\frac{F}{u^2} \longrightarrow 比耐公式：F=-\frac{p_\phi^2u^2}{m}(\frac{d^2u}{d\phi^2}+u)
\end{align}
$$

- 从开普勒三定律推导万有引力定律

	- [【Stardust · 理论物理初阶】 篇十 · 万有引力与天体运动：为天空立法](https://zhuanlan.zhihu.com/p/473342648)

	- 均匀球形天体之间总可以当做质点研究
	- 整个圆锥曲线大家族都是平方反比引力作用下运动轨迹的解
	- 行星轨道的形状完全由能量和角动量决定

- 初步应用

	- 潮汐与引潮力
	- 潮汐锁定现象
	- 洛希极限与行星环
	- 哈勃定律

### 质点系运动普遍规律

- 质点系的运动定理

	- 质心的定义
	- 动量定理，质心运动定理，动量守恒定律
	- 角动量定理（对定点和对质心），角动量守恒定律
	- 动能定理，
柯尼希定理：质点系动能=质心动能+各质点相对质心动能
机械能守恒定律

- 二体问题

	- 二体问题拉格朗日量

		- 

$$
\begin{align} &r_c=\frac{m_1r_1+m_2r_2}{m_1+m_2}，r=r_1-r_2，m=m_1+m_2，\mu=\frac{m_1m_2}{m_1+m_2}
\\&L=\frac{1}{2}m_1r_1^2+\frac{1}{2}m_2r_2^2-V(|r_1-r_2|)=\frac{1}{2}m\dot r_c^2+\frac{1}{2}\mu\dot r^2-V(r)

\end{align}
$$

	- 开普勒运动中的守恒量

		- 有心力场角动量守恒
保守力场能量守恒
平方反比力场LRL矢量守恒
		- LRL矢量方向始终由力心指向椭圆轨道的近日点，若R为守恒量，近日点方向不变，椭圆轨道闭合。

$$
\begin{align} 
&\frac{d}{dt}(\boldsymbol v\times \boldsymbol p_\phi-GMm\boldsymbol e_r)=\boldsymbol 0
\\&\boldsymbol R=\boldsymbol v\times \boldsymbol p_\phi-GMm\boldsymbol e_r(拉普拉斯-龙格-楞次矢量)
\end{align}
$$
		- 平方反比力场比起其他形式力场具有更高的动力学对称性，和轨道的简并性有关。
		- 假如是其他形式的力场（稍微偏离平方反比力场一点点），导致LRL矢量不再守恒，有微小的变动，那意味着：近日点存在漂移，行星的轨道也就不再是闭合的椭圆，每绕一圈都会往某个方向旋转一点。这种现象称为行星轨道的进动。

- 三体问题与摄动理论

	- 混沌理论与混沌系统
	- 限制性三体问题与摄动理论

### 碰撞与散射

- 经典碰撞与微分碰撞截面
- 散射与微分散射截面
- 卢瑟福散射公式

## 振动和波

### 简谐振动

- 

$$
\begin{align} 
&\ddot x+\omega x=0 
\\&x(t)=Acos(\omega t+\delta)
\\&\dot x(t)=-\omega A\sin(\omega t+\delta)
\\&\ddot x(t)=-\omega^2 A\cos(\omega t+\delta)
\\&\omega=\sqrt{\frac{\partial^2 V}{\partial q^2}\frac{1}{m}},\quad f=\frac{\omega}{2\pi}
\end{align}
$$

	- “对t求导”等价于“乘一个iω的因子”，微积分变成了简单的乘法，这使得计算变得非常方便。

$$
\begin{align} 
&x(t)=Ae^{i(\omega t+\delta)}=Ce^{i\omega t},\quad C=Ae^{i\delta}
\\&\dot x(t)=i\omega x,\quad \ddot x(t)=-\omega x^2
\end{align}
$$
	- 简谐振动的通解。

$$
\begin{align} 
&C=Ae^{i\delta}=a-bi
\\& x(t)=a\cos (\omega t)+b\sin (\omega t )
\end{align}
$$

- 复数的理解

	- 乘除法的几何意义也就变得很明显：做一次乘除，相当于复数的模长做一次放缩，同时辐角进行一次旋转.
正如我们之前将矩阵简洁明了地理解成“换坐标系”一样，现在面对复数，我们照样也能将它直接理解为“旋转”！
三角函数实质上可以表示成某个复数的实部或者虚部。
要注意：物理学研究尽管在中间步骤里可以借助复数，但最终的结果只能是实数（因为自然界总是用实数表示的）。

- 简谐振动的合成

	- 同方向、同频率简谐振动的合成

		- 振动相长与振动相消

	- 同方向、不同频率简谐振动的合成

		- 调制与拍频

	- 方向相互垂直的简谐振动的合成

		- 李萨如图形与锁模

### 非简谐振动

- 傅里叶展开与傅里叶级数

	- 狄利克雷收敛定理
	- 三角函数形式傅里叶展开

		- 

$$
\begin{align} &f(x)=\frac{A_0}{2}+\sum_{n=1}^\infty A_ncos(n\omega t)+\sum_{n=1}^\infty B_nsin(n\omega t)
\\&A_n=\frac{2}{T}\int_{0}^{T}f(x)cos(n\omega t)dt,n=0,1,2\dots
\\&B_ n=\frac{2}{T}\int_{0}^{T}f(x)sin(n\omega t)dt,n=1,2\dots


\end{align}
$$

	- 复指数形式傅里叶展开

		- 

$$
\begin{align} 
&f(t)=\sum_{-\infty}^{\infty} C_n e^{in\omega t},\quad -\infty<n<\infty
\\&C_n=\frac{1}{T}\int_o^T f(t) \big(e^{in\omega t}\big)^*dt
\end{align}
$$

- 频谱分析

	- 任何复杂的振动或者信号，只要具有周期性，都可以分解成一系列的简谐振动（正弦波）的叠加。
	- 最低的那个频率（等于原周期信号本身的频率）记作ω1=ω，称作基频（一般情况下基频的辐值也是最大的）；而更高的一系列频率（2ω、3ω……）则称作谐频，也称作泛频。
	- 波形图自变量是时间，描述的是信号强度随时间的变化；幅度频谱自变量是频率，描述的是不同频率成分的信号强度！有时我们把前者称为“在时域上描述”、后者称为“在频域上描述”。——傅里叶分析的意义便在于：将时域转化到频域

		- 幅度频谱：取复数形式傅里叶系数的模长为振幅，其幅角为频率

- 傅里叶变换：
非周期函数的频谱分析

	- 非周期性实函数进行傅里叶变换后，形成一个连续的、以ω为自变量的函数。这个过程就可以理解为：将时域上的函数f(t)转换到频域上的函数f^(ω)。这种转换过程称作傅里叶变换。
所以傅里叶变换的本质是函数到函数的转换，傅里叶变换仅仅是傅里叶级数在非周期函数上的推广。

		- 

$$
\begin{align} 
&\hat f(\omega)=\int_{-\infty}^{\infty} f(t)e^{-i\omega t}dt
\\&f(t)=\frac{1}{2\pi}\int_{-\infty}^{\infty}\hat f(\omega) e^{i\omega t}d\omega
\end{align}
$$
		- 一个信号的物理存在就是它能进行傅里叶变换的充分条件

	- δ函数
	- 拉普拉斯变换

		- 拉普拉斯变换与傅里叶变换最明显的一点差别在于iω变成了s，这个s不一定要是纯虚数，可以是任意的复数，因此拉普拉斯变换转换到的“s域”又称为复频域；其次，拉普拉斯变换中的积分是从0积分到无穷，而不是负无穷积分到正无穷，这意味着拉普拉斯变换更适用于一些“初值问题”——即从t=0时刻开始的问题。
		- 拉普拉斯变换将时域上的微分和积分直接转化成对s的乘法与除法，将微分方程转化为了代数方程，将大学的微积分转化为了小学的算术，这使得它可以用于控制理论中的系统响应分析（求取传递函数）。当然，拉普拉斯方程更通俗的应用在于让我们还可以借助它为我们求解那些让人讨厌的微分方程。具体的步骤是：通过拉普拉斯变换将微分方程转化为代数方程，三下五除二得到结果后，再利用拉普拉斯逆变换变回去就可以了。

### 自由振动
(小振动近似)
(可忽略二阶以上展开)

- 自由度=1的小振动

	- 

$$
\begin{align} &L=T-V=\frac{1}{2}m\dot q^2-V(q)，平衡位置取q=0
\\&\frac{\partial V}{\partial q}\bigg|_{q=0}=0，\frac{\partial ^2V}{\partial q^2}\bigg|_{q=0}=k>0，尝试泰勒展开
\\&V(q)=V(0)+\bigg(\frac{\partial V}{\partial q}\bigg|_{q=0}\bigg)q+\frac{1}{2}\bigg(\frac{\partial ^2V}{\partial q^2}\bigg|_{q=0}\bigg)q^2+o(q^2)
\\&\rightarrow L=T-V=\frac{1}{2}m\dot q^2-\frac{1}{2}kq^2，\omega=\omega_0=\sqrt{\frac{k}{m}}
\end{align}
$$

- 自由度=2的小振动

	- 

$$
\begin{align} &L=T-V=\frac{1}{2}m\dot x_1^2+\frac{1}{2}m\dot x_2^2-\bigg(\frac{1}{2}kx_1^2+\frac{1}{2}kx_2^2+\frac{1}{2}\kappa(x_1-x_2)^2\bigg)
\\&\quad=\frac{1}{2}m\dot x_1^2+\frac{1}{2}m\dot x_2^2-\frac{1}{2}(k+\kappa)x_1^2-\frac{1}{2}(k+\kappa)x_2^2+\kappa x_1x_2
\\&代入拉格朗日方程\frac{1}{dt}\bigg(\frac{\partial L}{\partial \dot q}\bigg)=\frac{\partial L}{\partial q}
\Rightarrow
\begin{cases}
m\ddot x_1+(k+\kappa)x_1=\kappa x_2
\\m\ddot x_2+(k+\kappa)x_2=\kappa x_1
\end{cases}
\end{align}
$$
	- 

$$
\begin{align} &令\omega_0=\sqrt{\frac{k+\kappa}{m}}，\eta=\frac{\kappa}{m}，有
\begin{cases}
\ddot x_1+\omega_0^2 x_1=\eta x_2
\\\ddot x_2+\omega_0^2 x_2=\eta x_1
\end{cases}

\\&猜测结论必然仍为简谐振动，且频率相同，
代入有
\\&\begin{cases}
x_1=C_1e^{i\omega t}
\\x_2=C_2e^{i\omega t}
\end{cases}
\Rightarrow
\begin{cases}
(\omega_0^2-\omega^2)C_1-\eta C_2=0
\\(\omega_0^2-\omega^2)C_2-\eta C_1=0
\end{cases}

\\&\left [ \begin{matrix}
 \omega_0^2-\omega^2 & -\eta \\
-\eta& \omega_0^2-\omega^2 \\
\end{matrix} \right ] \left [ \begin{matrix}
C_1 \\
C_2\\
\end{matrix} \right ] =\left [ \begin{matrix}
0\\
0 \\
\end{matrix} \right ] 
\Rightarrow \left | \begin{matrix}
 \omega_0^2-\omega^2 & -\eta \\
-\eta& \omega_0^2-\omega^2 \\
\end{matrix} \right |=0
\\&\Rightarrow\omega_0^2-\omega^2
\Rightarrow
\begin{cases}
\omega_1=\sqrt{\omega_0^2-\eta}=\sqrt{\frac{k}{m}}\\
\omega_2=\sqrt{\omega_0^2+\eta}=\sqrt{\frac{k+2\kappa}{m}}
\end{cases}
\end{align}
$$
	- 

$$
\begin{align} &两组频率使得最终坐标振动方程有两组解，对称及反对称
\\&\omega_1=\sqrt{\omega_0^2-\eta},C_1=C_2,\left [ \begin{matrix}
x_1\\
x_2 \\
\end{matrix} \right ] =\frac{1}{\sqrt{2}}\left [ \begin{matrix}
1\\
1\\
\end{matrix} \right ] \cdot Ae^{i\omega_1 t}

\\&\omega_2=\sqrt{\omega_0^2+\eta},C_1=-C_2,\left [ \begin{matrix}
x_1\\
x_2 \\
\end{matrix} \right ] =\frac{1}{\sqrt{2}}\left [ \begin{matrix}
1\\
-1\\
\end{matrix} \right ] \cdot Be^{i\omega_2 t}
\\&实际振动是两种集体振动形式的叠加，AB表示各自分量的系数
\\&\left [ \begin{matrix}
x_1\\
x_2 \\
\end{matrix} \right ] 
=A\bigg(\frac{1}{\sqrt{2}}\left [ \begin{matrix}
1\\
1\\
\end{matrix} \right ] \cdot e^{i\omega_1 t}\bigg)
+
B\bigg(\frac{1}{\sqrt{2}}\left [ \begin{matrix}
1\\
-1\\
\end{matrix} \right ] \cdot e^{i\omega_2 t}\bigg)
\end{align}
$$

- 简正模

	- 将每一种可能的振动模式称为一支简正模，他们几乎完全独立存在，允许叠加，互不干扰。
自由度=2的小振动里，坐标x1，x2相互耦合。从笛卡尔进入广义坐标，通过换坐标系将所有坐标分离，彼此独立，得到简正频率与简正坐标。
	- 

$$
\begin{align} &根据\left [ \begin{matrix}
x_1\\  x_2 \\
\end{matrix} \right ] 
=A\bigg(\frac{1}{\sqrt{2}}
\left [ \begin{matrix}
1\\   1\\
\end{matrix} \right ] 
\cdot e^{i\omega_1 t}\bigg)
+
B\bigg(\frac{1}{\sqrt{2}}
\left [ \begin{matrix}
1\\   -1\\
\end{matrix} \right ] 
\cdot e^{i\omega_2 t}\bigg)

\\&使用简正坐标Q_1和Q_2，有
\left [ \begin{matrix}
x_1\\  x_2 \\
\end{matrix} \right ] 
=Q_1\bigg(\frac{1}{\sqrt{2}}
\left [ \begin{matrix}
1\\   1\\
\end{matrix} \right ] \bigg)
+
Q_2\bigg(\frac{1}{\sqrt{2}}
\left [ \begin{matrix}
1\\   -1\\
\end{matrix} \right ] \bigg)
\\&\begin{cases}
Q_1=\frac{1}{\sqrt{2}}(x_1+x_2)=Ae^{i\omega_1 t}\\
Q_2=\frac{1}{\sqrt{2}}(x_1-x_2)=Be^{i\omega_2 t}
\end{cases}，L=\frac{1}{2}m\dot Q_1^2-\frac{1}{2}k Q_1^2+\frac{1}{2}m\dot Q_2^2-\frac{1}{2}(k+2\kappa) Q_2^2
\\&复振幅A和B，频率仍为\omega_1和\omega_2，两个完全独立的一维简谐振动
\\&一般频率最低的模式总是对称的，反对称频率较高

\end{align}
$$
	- 对称矩阵的本征值与本征矢

		- 

$$
\begin{align} &\left [ \begin{matrix}
 \omega_0^2-\omega^2 & -\eta \\
-\eta& \omega_0^2-\omega^2 \\
\end{matrix} \right ] \left [ \begin{matrix}
C_1 \\C_2\\
\end{matrix} \right ] =\left [ \begin{matrix}
0\\0 \\
\end{matrix} \right ] 
\Rightarrow
\left [ \begin{matrix}
 \omega_0^2 & -\eta \\
-\eta& \omega_0^2 \\
\end{matrix} \right ] \left [ \begin{matrix}
C_1 \\C_2\\
\end{matrix} \right ] =\omega^2\left [ \begin{matrix}
C_1\\C_2 \\
\end{matrix} \right ] 
\\&令\left [ \begin{matrix}
 \omega_0^2 & -\eta \\
-\eta& \omega_0^2 \\
\end{matrix} \right ] =\boldsymbol S,\left [ \begin{matrix}
C_1 \\C_2\\
\end{matrix} \right ] =\boldsymbol c, \omega^2=\lambda,得到\boldsymbol {Sc}=\lambda\boldsymbol c
\\&\lambda 为\boldsymbol S的特征值（本征值），\boldsymbol S总是一个实对称矩阵
\\&\boldsymbol c为\boldsymbol S的特征向量（本征矢），任意两个本征矢满足正交归一化条件

\end{align}
$$

			- 

	- 实对称矩阵性质

		- 性质一：
      s阶的实对称矩阵会有s个独立的本征矢，一般做归一化处理，且对应的本征值均为实数。

性质二：
      对于实对称矩阵，如果两个本征矢对应着不同的本征值，那么这两个本征矢一定相互正交，空间图像为本征椭球。此外，对角化前后，矩阵本征值不变。

性质三：
      对于实对称矩阵，如果两个本征矢对应着相同的本征值，那么这两个本征矢的任意线性组合也是原矩阵的本征矢，且还是对应和原来相同的本征值。

- 多个自由度的小振动

	- 多自由度耦合的小振动模型：
        常见于分子物理中的分子光谱、固体物理中晶格里的原子振动、电磁学中的耦合振荡等等。
        任何会振动的物体，都具有一组简正模以及相对应的简正频率（固有频率）。这些简正模相互独立，当外界条件符合激发起其中一种简正模的条件时，则这种简正模会被激发起来，形成统一的集体振荡，而另外的简正模则不会被激发。如果外界条件同时激发起了多支简正模，最终依然会形成集体振荡，振荡是多支简正模的线性叠加。

$$
\begin{align} &多个自由度\{q_1,q_2,\dots,q_s\},系统平衡条件：\frac{\partial V}{\partial q_i}\bigg|_{q_i=0}=0
\\&泰勒展开二阶项表示势能：V=\frac{1}{2}\sum_{i,j}\bigg(\frac{\partial^2 V}{\partial q_iq_j}\bigg|_{\boldsymbol q=0}\bigg)q_iq_j=\frac{1}{2}\sum_{i,j}K_{ij}q_iq_j
\\&系数K_{ij}可以写为s阶实对称矩阵\boldsymbol K
\\&系统拉格朗日量：L=T-V=\frac{1}{2}\sum_{i}m_i\dot q_i^2
-\frac{1}{2}\sum_{i,j}K_{ij}q_iq_j
\\&拉格朗日方程得到s个运动方程:m_i\ddot q_i+\sum_j K_{ij}q_j=0
\\&设想每个自由度做简谐振动，共同频率\omega，q_i=C_i e^{i\omega t}，
\\&定义v_i=\sqrt{m_i}C_i，K_{ij}'=\frac{K_{ij}}{\sqrt{m_im_j}} ，M_{(a)}=\bigg|\boldsymbol v_{(a)}\bigg|^2，K_{(a)}=M_{(a)}\omega^2_{(a)}

\\&-\omega^2v_i+\sum_{j}K_{ij}'v_j=0，本征值方程形式：\boldsymbol {K'v}=\omega ^2\boldsymbol v
\\&求解s个本征值得到s个简正频率，则每支简正模对应Q_{(a)}=A_{(a)}e^{i\omega_{(a)}t}
\\&简正坐标下L=\frac{1}{2}\sum_{(a)}M_{(a)}\bigg(\dot Q_{(a)}\bigg)^2
-\frac{1}{2}\sum_{(a)}K_{(a)}\bigg( Q_{(a)}\bigg)^2


\end{align}
$$

### 阻尼振动和受迫振动

- f=-bv形式阻尼

	- 

$$
\begin{align} &引入耗散函数G=\frac{1}{2}b\dot x^2,f=-\frac{\partial G}{\partial \dot x}，得到阻尼振动系统运动方程：m\ddot x+b\dot x+kx=0
\\&猜测x=Ce^{i\omega t}并带入得：-m\omega^2+ib\omega+k=0，\omega=i\bigg(\frac{b}{2m}\bigg)\pm\sqrt{-\bigg(\frac{b}{2m}\bigg)^2+\frac{k}{m}}
\\&令\beta=\frac{b}{2m}，\omega_0^2=\frac{k}{m}，振动方程：x(t)=Ce^{i\omega t}=Ce^{-\beta t}e^{\pm i\sqrt{\omega_0^2-\beta^2 }t}
\\&上式说明阻尼作用下，振幅随时间衰减。
\\1.&阻力较小(欠阻尼)\beta^2<\omega_0^2：令\omega_r=\sqrt{\omega_0^2-\beta^2}，x(t)=(Ce^{-\beta t})e^{\pm i\omega_r t}
\\2.&阻力较大(过阻尼)\beta^2>\omega_0^2：令i\omega_i=\sqrt{\omega_0^2-\beta^2}，x(t)=Ce^{-(\beta\pm \omega_i) t}
\\3.&(临界阻尼)\beta^2=\omega_0^2：x(t)=Ce^{-\beta t}，最短时间停止振动

\end{align}
$$

- 受迫振动

	- 

$$
\begin{align} &一般为周期驱动力F(t)=Fe^{i\Omega t},运动方程：m\ddot x+b\dot x+kx=F
\\&猜测x=Ce^{i\omega t},连同F(t)=Fe^{i\Omega t}带入得：(-m\omega^2+ib\omega+k)Ce^{i\omega t}=Fe^{i\Omega t}
\\&齐次方程通解：x_通(t)=C_通e^{-(\beta \pm i\omega_r) t}
\\&非齐次方程特解(\omega=\Omega):复振幅C_特=\frac{F}{-m\Omega^2+ib\Omega+k}=\frac{F}{m}\frac{1}{(\omega_0^2-\Omega_0^2)+2i\beta\Omega}
\\&\qquad |C_特|=\frac{F}{m}\frac{1}{\sqrt{(\omega_0^2-\Omega_0^2)^2+4\beta^2\Omega^2}},\tan\delta=-\frac{2\beta\Omega}{\omega_0^2-\Omega^2}
\\&x(t)=C_通e^{-(\beta \pm i\omega_r) t}+
\frac{F}{m}\frac{1}{\sqrt{(\omega_0^2-\Omega_0^2)^2+4\beta^2\Omega^2}}e^{i(\Omega t+\delta)}
\\&暂态解一段时间后消解，留下稳态解和驱动力频率一致
\\&\omega_0^2-\Omega_0^2时，振幅达到极大，发生共振，这时\beta=0,实际由于阻尼，共振频率略有偏移

\end{align}
$$

- 线性系统

	- 线性可叠加性
线性微分方程
小振动近似

### 振动的空间传播——波动

- 基本概念

	- 球面波，平面波，波阵面（波面），波射线（波线），简谐波
	- 简谐波表达式

		- 

$$
\begin{align} &波源振动方程(u为偏移量)：u(x=0,t)=A\cos(\omega t+\delta)
\\&波的振动状态以波速v传播，x点状态和往前推t时间波源状态重合
\\&u(x=v\Delta t,t)=A\cos[\omega (t-\Delta t)+\delta]=A\cos[\omega(t-\frac{x}{v})+\delta]
\\&(角)波数k=\frac{\omega }{v}表示单位距离相位的变化,(角)频率是单位时间相位变化
\\&三维情况:u(\boldsymbol r,t)=A\cos(\omega t-\boldsymbol {k\cdot r}+\delta)=Ce^{i(\omega t-\boldsymbol {k\cdot r})}
\\&波长\frac{2\pi}{k},波数\frac{k}{2\pi},复振幅C=Ae^{i\delta}

\end{align}
$$

	- 波动方程

		- 

$$
\begin{align} &为寻找标准形式波动方程，以弹簧波为出发点，为离散问题，将微分写为差分

\\&\frac{u_{n+1}-2u_n+u_{n-1}}{(\Delta x)^2}相当于连续问题中对空间的二阶偏导,\Delta x=a
\\&将离散的弹簧波运动递推方程改写为连续形式:\frac{\partial^2 u}{\partial t^2}=(\omega_0^2 a^2)\frac{\partial^2 u}{\partial a^2}=v^2\frac{\partial^2 u}{\partial x^2}，
\\&推广三维情形：\frac{\partial^2 u}{\partial t^2}=v^2\bigg(\frac{\partial^2 u}{\partial x^2}+\frac{\partial^2 u}{\partial y^2}+\frac{\partial^2 u}{\partial z^2}\bigg)
\\&波动方程：\frac{\partial^2 u}{\partial t^2}=v^2\Delta^2 u（涵盖线性、无色散、无耗散介质的一切波动形式）
\\&简谐波u(\boldsymbol r,t)=Ce^{i(\omega t-\boldsymbol{k\cdot r})}是波动方程的解，但不是唯一解

\end{align}
$$

			- 

$$
\begin{align} &一阶差分：\Delta u_n=u_{n+1}-u_n，二阶差分：\Delta^2 u_n=\Delta(\Delta u_n)=u_{n+1}-2u_n+u_{n-1}
\\&n阶差分：\Delta^n u_n=\Delta^{n-1} u_{n+1}-\Delta^{n-1} u_n=u_{n+1}-2u_n+u_{n-1}=\sum_{k=0}^i(-1)^k\frac{i!}{k!(i-k)!}u_{t+i-k}
\\&一阶差商：\frac{\Delta u}{\Delta x}=\frac{u_{n+1}-u_n}{\Delta x}
\\&二阶差商：\frac{\Delta (\frac{\Delta u}{\Delta x})}{\Delta x}=\frac{\frac{u_{n+1}-u_n}{\Delta x}-\frac{u_n-u_{n-1}}{\Delta x}}{\Delta x}=\frac{u_{n+1}-2u_n+u_{n-1}}{(\Delta x)^2}
\end{align}
$$

- 波的色散

	- 对任意波，在频率不同时导致波速v不同，则称这支波有色散.由于v=ω(k)/k,则ω(k)与k为线性关系时，波无色散。
	- 无限长弹簧链

		- 

$$
\begin{align} &小球m全同，弹簧\kappa全同，考虑纵波，无限长规避边界
\\&第0质点平衡位置为坐标原点，第n质点x_n=na，偏离平衡长度u_n
\\&牛二：m\ddot u_n=\kappa(u_{n+1}-u_n)-\kappa(u_{n}-u_{n-1})
\\&得到弹簧波的运动方程（递推形式）： \ddot u_n=\omega_0^2(u_{n+1}-2u_n+u_{n-1})
\\
\\&代入简谐波方程的解：u(x_n,t)=Ce^{i(\omega t-kna)}
\\&\Rightarrow -\omega^2=\omega_0^2(e^{-ika}-2+e^{ika})=-2\omega_0^2(1-\cos ka)=-4\omega_0^2\sin^2(\frac{ka}{2})
\\&则无限长弹簧链模型中，频率和波数关系(色散关系)：\omega(k)=2\omega_0\sin(\frac{ka}{2}),
\\&弹性波的波速：v=\frac{\omega }{k}=\frac{2\omega_0}{k}\sin(\frac{ka}{2})，为色散波

\\\\&研究连续固体中的弹性波(宏观声波),ka\ll 1,\omega(k)=\omega_0 ka,v=\omega_0 a,无色散波

\end{align}
$$

	- 群速与相速

		- 

$$
\begin{align} &波包传播速度称为群速，也是能量传播的速度，v_g=\frac{d\omega}{dk}。
\\&振动传播的速度为相速,v=\frac{\omega}{k}，存在色散时二者速度不同。
\end{align}
$$

## 刚体力学

### 刚体运动学

- 基本概念

	- 刚体自由度：不共线的三个点共9个自由度，三点之间满足互相距离为常数的约束，故空间总自由度恒为s=9-3=6
	- 运动类型：空间平动s=3，定轴转动s=1，平面平行运动s=3（分解为质心平面平动和绕质心轴转动），定点转动s=3（瞬时转轴过定点，两角度确定转轴取向，一个角度确定旋转角），一般运动s=6（分解为质心平动和绕质心定点转动）
	- 角位移未必满足交换律，转动先后顺序调换，结果未必相同。因此有限转动不具备矢量性质。
但是角位移无限小时，两次转动叠加可以省略二阶小量，无限小转动可以看做矢量，以至于通过极限定义的角速度也看做矢量，故角速度可以按照速度的极限定义。

- 欧拉角与欧拉运动学方程

	- 

$$
\begin{align} &欧拉角(\phi,\theta,\psi)，初始本体坐标系与固定坐标系重合
\\&进动角\phi:刚体并绕固定坐标系\boldsymbol{Z轴}转动\phi角(x',y',z')轴=(x',y',z)轴
\\&章动角\theta:刚体绕本体坐标系\boldsymbol{x'轴}转过\theta 角，(x'',y'',z'')轴=(x',y'',z'')轴
\\&转动角\psi:刚体整体绕新的瞬时转轴\boldsymbol{z''}轴旋转\psi角至(x,y,z)
\\&对角速度矢量\omega:\begin{cases}
固定坐标系：\boldsymbol \omega=\omega_X\boldsymbol e_X+\omega_Y\boldsymbol e_Y+\omega_Z\boldsymbol e_Z\\
本体坐标系：\boldsymbol \omega=\omega_x\boldsymbol e_x+\omega_y\boldsymbol e_y+\omega_z\boldsymbol e_z\\
欧拉角坐标系：\boldsymbol \omega=\dot\phi \boldsymbol e_Z+\dot \theta\boldsymbol {e_x'}+\dot\psi\boldsymbol {e_z''}
\end{cases}
\\&欧拉运动学方程：\begin{cases}
\omega_x=\dot \phi\sin\theta\sin\psi+\dot\theta\cos\psi\\
\omega_y=\dot \phi\sin\theta\cos\psi-\dot\theta\sin\psi\\
\omega_z=\dot\phi\cos\theta+\dot\psi

\end{cases}


\end{align}
$$

		- 
		- 

- 转动矩阵

	- 

$$
\begin{align} &矩阵实质就是空间变换，即变换坐标系
\\&在平面系中，\boldsymbol A=A_x\boldsymbol {e_x}+A_y\boldsymbol {e_y}=A_r\boldsymbol{e_r}+A_\phi\boldsymbol {e_\phi} ,\quad \boldsymbol {R^{-1}R=I}
\\&\left [ \begin{matrix}
\boldsymbol{e_r}& \boldsymbol{e_\phi} \\
\end{matrix} \right ]
\left [ \begin{matrix}
A_r \\
A_\phi\\
\end{matrix} \right ]
=\left [ \begin{matrix}
\boldsymbol{e_x}& \boldsymbol{e_y} \\
\end{matrix} \right ]
\left [ \begin{matrix}
\cos\phi& -\sin\phi \\
\sin\phi& \cos\phi \\
\end{matrix} \right ]
\left [ \begin{matrix}
\cos\phi& \sin\phi \\
-\sin\phi& \cos\phi \\
\end{matrix} \right ]
\left [ \begin{matrix}
A_x \\
A_y\\
\end{matrix} \right ]
=
\left [ \begin{matrix}
\boldsymbol{e_x}& \boldsymbol{e_y} \\
\end{matrix} \right ]
\left [ \begin{matrix}
A_x \\
A_y\\
\end{matrix} \right ]
\\&(x,y)坐标轴绕原点逆时针转动\phi成为(x',y'),\boldsymbol A=A_x\boldsymbol {e_x}+A_y\boldsymbol {e_y}=A_x'\boldsymbol {e_x;}+A_y'\boldsymbol {e_y'}
\\&\left [ \begin{matrix}
A_x' \\
A_y'\\
\end{matrix} \right ]
=
\left [ \begin{matrix}
\cos\phi& \sin\phi \\
-\sin\phi& \cos\phi \\
\end{matrix} \right ]
\left [ \begin{matrix}
A_x \\
A_y\\
\end{matrix} \right ]
\Rightarrow 
\left [ \begin{matrix}
A_x' \\
A_y'\\
A_z'\\
\end{matrix} \right ]
=
\left [ \begin{matrix}
\cos\phi& \sin\phi &0\\
-\sin\phi& \cos\phi &0\\
0&0&1\\
\end{matrix} \right ]
\left [ \begin{matrix}
A_x \\
A_y\\
A_z\\
\end{matrix} \right ]
\\&绕那根轴旋转，其方向上的分量不变：\boldsymbol A^{(x'y'z')}=\boldsymbol R_{\phi}^{(z)}\boldsymbol A^{(xyz)},转动矩阵即\boldsymbol R_{\phi}^{(z)}
\\
\\&将任意矢量\boldsymbol A从固定坐标系(X,Y,Z)转换到本体坐标系(x,y,z)''共三个转动矩阵参与
\\&\begin{cases}
\boldsymbol A^{(xyz)}=\boldsymbol R_{\psi}^{(z'')}\boldsymbol R_{\theta}^{(x')}\boldsymbol R_{\phi}^{(Z)}\boldsymbol A^{(XYZ)}\\
\boldsymbol R=\boldsymbol R_{\psi}^{(z'')}\boldsymbol R_{\theta}^{(x')}\boldsymbol R_{\phi}^{(Z)}
\end{cases}
,
\begin{cases}
\boldsymbol R_{\phi}^{(Z)}=\left [ \begin{matrix}
\cos\phi& \sin\phi &0\\
-\sin\phi& \cos\phi &0\\
0&0&1\\
\end{matrix} \right ]
\\
\boldsymbol R_{\theta}^{(x')}=
\left [ \begin{matrix}
1&0&0\\
0&\cos\theta& \sin\theta \\
0&-\sin\theta& \cos\theta \\
\end{matrix} \right ]
\\
\boldsymbol R_{\psi}^{(z'')}=
\left [ \begin{matrix}
\cos\psi& \sin\psi &0\\
-\sin\psi& \cos\psi &0\\
0&0&1\\
\end{matrix} \right ]
\end{cases}
\\&\boldsymbol R=
\left [ \begin{matrix}
\cos\psi\cos\phi-\cos\theta\sin\phi\sin\psi
& \cos\psi\sin\phi+\cos\theta\cos\phi\sin\psi 
&\sin\psi\sin\theta\\
-\sin\psi\cos\phi-\cos\theta\sin\phi\cos\psi
& -\sin\psi\sin\phi+\cos\theta\cos\phi\cos\psi &\cos\psi\sin\theta\\
\sin\theta\sin\phi & -\sin\theta\cos\phi &\cos\theta\\
\end{matrix} \right ]

\end{align}
$$

### 刚体动力学

- 转动惯量张量

	- 

$$
\begin{align} &(转动问题)总角动量分量出发点：刚体角动量等于质点角动量之和，\boldsymbol L=\sum_{(a)}\boldsymbol L^{(a)}
\\&选取定点O建立固定坐标系(X,Y,Z)
\\&\boldsymbol L=\sum_{(a)}\boldsymbol L^{(a)}=\sum_{(a)}m^{(a)}\boldsymbol r^{(a)}\times\boldsymbol v^{(a)}=\sum_{(a)}m^{(a)}\boldsymbol r^{(a)}\times(\boldsymbol \omega\times\boldsymbol r^{(a)})
\\&\qquad=\sum_{(a)}m^{(a)}\bigg[\bigg(r^{(a)}\bigg)^2\boldsymbol \omega-\bigg(\boldsymbol r^{(a)}\cdot \boldsymbol \omega\bigg)\boldsymbol r^{(a)}\bigg]
\\&将分量式代入：\begin{cases}
\big(r^{(a)}\big)^2=\big(X^{(a)}\big)^2+\big(Y^{(a)}\big)^2+\big(Z^{(a)}\big)^2\\
\boldsymbol \omega=\omega_X\boldsymbol e_X+\omega_Y\boldsymbol e_Y+\omega_Z\boldsymbol e_Z
\end{cases}
\\&得到L分量\begin{cases}
L_X=I_{XX}\omega_X-I_{XY}\omega_Y-I_{XZ}\omega_Z\\
L_Y=-I_{YX}\omega_X+I_{YY}\omega_Y-I_{YZ}\omega_Z\\
L_Z=-I_{ZX}\omega_X-I_{ZY}\omega_Y+I_{ZZ}\omega_Z
\end{cases}
\\&转动惯量I的系数\begin{cases}
I_{XX}=\sum_{(a)}m^{(a)}\bigg[\big(Y^{(a)}\big)^2+\big(Z^{(a)}\big)^2\bigg]=\int(Y^2+Z^2)dm\\
I_{YY}=\sum_{(a)}m^{(a)}\bigg[\big(Z^{(a)}\big)^2+\big(X^{(a)}\big)^2\bigg]\int(X^2+Z^2)dm\\
I_{ZZ}=\sum_{(a)}m^{(a)}\bigg[\big(X^{(a)}\big)^2+\big(Y^{(a)}\big)^2\bigg]\int(Y^2+X^2)dm
\end{cases}
\\&惯量积I的系数\begin{cases}
I_{XY}=I_{YX}=\sum_{(a)}m^{(a)}\big(X^{(a)}\big)\big(Y^{(a)}\big)=\int XYdm\\
I_{YZ}=I_{ZY}=\sum_{(a)}m^{(a)}\big(Y^{(a)}\big)\big(Z^{(a)}\big)=\int YZdm\\
I_{ZX}=I_{XZ}=\sum_{(a)}m^{(a)}\big(Z^{(a)}\big)\big(X^{(a)}\big)=\int ZXdm
\end{cases}
\\&可以写作\boldsymbol L=\boldsymbol{I\omega}\Rightarrow
\left [ \begin{matrix}
L_X \\L_Y\\L_Z\\
\end{matrix} \right ]
=
\left [ \begin{matrix}
I_{XX}& -I_{XY} &-I_{XZ} \\
-I_{YX}& I_{YY} &-I_{YZ}\\
-I_{ZX}& -I_{ZY} &I_{ZZ}\\
\end{matrix} \right ]
\left [ \begin{matrix}
\omega_X \\\omega_Y\\\omega_Z\\
\end{matrix} \right ]
\\&此处\boldsymbol{I}为固定坐标系转动惯量张量(二阶张量)，矢量是一阶张量

\end{align}
$$

		- 

$$
\begin{align} &双重矢量积辅助记忆
\\&\boldsymbol a\times(\boldsymbol b\times \boldsymbol c)=(\boldsymbol a\cdot\boldsymbol c)\boldsymbol b-(\boldsymbol a\cdot \boldsymbol b)\boldsymbol c
\\&\boldsymbol y=m\boldsymbol b-n\boldsymbol c,利用垂直和共线，括号在前加负号
\end{align}
$$

	- 

$$
\begin{align} &将固定坐标系的转动惯量张量迁移到本体坐标系，利用其实对称矩阵性质
\\&求出实对称矩阵本征矢，选相互正交三组构建新坐标系写成对角矩阵形式，
\\&\boldsymbol I=\left [ \begin{matrix}
I_{xx}& 0&0\\
0&I_{yy} &0 \\
0& 0& I_{zz} \\
\end{matrix} \right ],构建主轴坐标系(x,y,z)，三根坐标轴为惯量主轴
\\&\boldsymbol L=\boldsymbol {I\omega}\Rightarrow
\begin{cases}
L_x=I_{xx}\omega_x\\
L_y=I_{yy}\omega_y\\
L_z=I_{zz}\omega_z
\end{cases}
\\&空间表示:惯量椭球。表面任一点到椭球中心O距离\rho满足I_{OA}=\frac{1}{\rho^2_{OA}}

\end{align}
$$

		- 
		- 例题

- 刚体动力学微分方程

	- 

$$
\begin{align} &任意空间定点O为基点情况下，\sum\boldsymbol M_o=\frac{d\boldsymbol L_o}{dt}=\boldsymbol {I_o\beta}
\\&假设取空间任一点A，位矢\boldsymbol r_0，速度\boldsymbol v_0
\\&\boldsymbol L_A=\sum_{(a)}\boldsymbol L^{(a)}_A
=\sum_{(a)}m^{(a)}\big(\boldsymbol {r_0+r^{(a)}_A}\big)
\times\big(\boldsymbol{ v_0+\omega\times r^{(a)}_A}\big)

\\&\quad=m\boldsymbol r_0\times \boldsymbol v_0
+\boldsymbol r_0\times\bigg[\boldsymbol \omega\times\bigg(\sum_{(a)}m^{(a)}\boldsymbol r^{(a)}_A\bigg) \bigg]
+\bigg(\sum_{(a)}m^{(a)}\boldsymbol r^{(a)}_A\bigg)\times\boldsymbol v_0+\boldsymbol {I_A\omega}

\\&\quad=m\boldsymbol r_0\times \boldsymbol v_0+\boldsymbol {I_A\omega}\quad(当A为质心时)
\\
&刚体动力学微分方程（2组6个）\begin{cases}
合外力决定动量变化率&
\frac{d\boldsymbol p}{dt}=\sum\boldsymbol F\\
合外力矩决定角动量变化率&\frac{d\boldsymbol L_o}{dt}=\sum\boldsymbol M_o
\end{cases}
\\&(平动问题)质心运动定理：\sum\boldsymbol F=m\boldsymbol a_c
\\&(转动问题)质心转动定理：\sum\boldsymbol M_c=\frac{d\boldsymbol L_A}{dt}=\boldsymbol {I_c\beta}

\end{align}
$$

- 刚体的动能

	- 

$$
\begin{align} &定点运动的刚体（固定坐标系中）：
\\&\boldsymbol T=\sum_{(a)}\boldsymbol T^{(a)}
=\sum_{(a)}\frac{1}{2}m^{(a)}\big(v^{(a)}\big)^2=\frac{1}{2}\sum_{(a)}m^{(a)}\boldsymbol v^{(a)}\cdot\big(\boldsymbol\omega\times \boldsymbol r^{(a)}\big)=\frac{1}{2}\boldsymbol\omega\boldsymbol L

\\&一般运动的刚体（取刚体上A为基点）
\\&\boldsymbol T=\sum_{(a)}\boldsymbol T^{(a)}
=\sum_{(a)}\frac{1}{2}m^{(a)}\big(\boldsymbol v_0 +\boldsymbol{\omega\times r^{(a)}_A}\big)^2

\\&\quad =\sum_{(a)}\frac{1}{2}m^{(a)} v_0^2
+\sum_{(a)}m^{(a)}\boldsymbol v_0 \cdot \big(\boldsymbol{\omega\times r^{(a)}_A}\big)+\sum_{(a)}\frac{1}{2}m^{(a)}\big(\boldsymbol{\omega\times r^{(a)}_A}\big)^2
\\&\quad =\frac{1}{2}m v_0^2+\big(\boldsymbol{v_0\times \omega}\big)\cdot \sum_{(a)}m^{(a)}\boldsymbol r^{(a)}_A+\frac{1}{2}\boldsymbol{\omega\cdot I_A\omega}
\\&\quad =\frac{1}{2}m v_c^2+\frac{1}{2}\boldsymbol{\omega\cdot I_c\omega}
=\frac{1}{2}m v_c^2+\frac{1}{2}I_{cxx}\omega_x^2+\frac{1}{2}I_{cyy}\omega_y^2+\frac{1}{2}I_{czz}\omega_z^2
\\&（主轴坐标系）欧拉运动学方程：\begin{cases}
\omega_x=\dot \phi\sin\theta\sin\psi+\dot\theta\cos\psi\\
\omega_y=\dot \phi\sin\theta\cos\psi-\dot\theta\sin\psi\\
\omega_z=\dot\phi\cos\theta+\dot\psi
\end{cases}

\\&代入T=\frac{1}{2}I_{xx}\omega_x^2+\frac{1}{2}I_{yy}\omega_y^2+\frac{1}{2}I_{zz}\omega_z^2（这里不需要平动动能）
\end{align}
$$

- 欧拉动力学方程

	- 

$$
\begin{align} &选取欧拉角(\phi,\theta,\psi)为广义坐标,在主轴坐标系中
\\&拉格朗日量\mathcal L=T-V=\frac{1}{2}I_{xx}\omega_x^2+\frac{1}{2}I_{yy}\omega_y^2+\frac{1}{2}I_{zz}\omega_z^2-V(\phi,\theta,\psi)
\\&代入含有广义力的拉格朗日方程，对\psi:\frac{d}{dt}\big(\frac{\partial T}{\partial \dot \psi}\big)-\frac{\partial T}{\partial  \psi}=M_z（V=0）
\\&得刚体运动的欧拉动力学方程(主轴坐标系)
\begin{cases}
I_{xx}\dot \omega _x-(I_{yy}-I_{zz})\omega_y\omega_z=M_x\\
I_{yy}\dot \omega _y-(I_{zz}-I_{xx})\omega_z\omega_x=M_y\\
I_{zz}\dot \omega _z-(I_{xx}-I_{yy})\omega_x\omega_y=M_z
\end{cases}
\\&矢量形式：\boldsymbol{\dot L-L\times\omega=M}(主轴坐标系)
\\&已知外力矩，刚体角速度只由三个主转动惯量决定，与形状和质量分布无关
\\&研究转动的时候，任意刚体可等效为具有相同主转动惯量的均质椭球
\end{align}
$$

### 陀螺运动

- 重力影响下刚体定点运动问题

	- 能解析求解的三种情况：

第一种：欧拉-潘索情况（欧拉陀螺），固定点O与刚体重心重合。

第二种：拉格朗日-泊松情况（拉格朗日陀螺），刚体动力学意义具有旋转对称性，重心在旋转对称轴z上，不必和固定点O重合，Ixx=Iyy。

第三种：柯凡律夫斯卡娅情况（柯凡律夫斯卡娅陀螺），刚体动力学意义具有旋转对称性，Ixx=Iyy=2Izz，不必和固定点O重合。
	- 我们的地球其实也是一个巨大的、在宇宙空间中不停旋转的陀螺。我们所有人都生活在陀螺上。

		- 

- 拉格朗日陀螺

	- 图像说明

		- 
		- 
		- 

	- 

$$
\begin{align} &拉格朗日陀螺：对称轴底端固定O点，重心C在对称轴上，距O点l，I_{xx}=I_{yy}
\\&\begin{cases}
I_{xx}\dot \omega _x-(I_{yy}-I_{zz})\omega_y\omega_z=mgl\sin\theta\cos\psi\\
I_{yy}\dot \omega _y-(I_{zz}-I_{xx})\omega_z\omega_x=mgl\sin\theta\sin\psi\\
I_{zz}\dot \omega _z=0
\end{cases}
\\&\mathcal L不显含角度\psi \Rightarrow \frac{d\omega_z}{dt}=0\Rightarrow 守恒量\omega_z=\dot\phi\cos\theta+\dot\psi：陀螺角速度在陀螺对称轴z上分量不变
\\&\mathcal L不显含时间t\Rightarrow \frac{d\mathcal L}{dt}=0 \Rightarrow E=\frac{1}{2}(I_{xx}\omega_x^2+I_{yy}\omega_y^2+I_{zz}\omega_z^2)+mgl\cos\theta ：能量守恒
\\&\mathcal L不显含角度\phi,Z轴方向无力矩\Rightarrow L_Z=I_{xx}\dot\phi\sin^2\theta+I_{zz}\omega_z\cos\theta\Rightarrow对应的广义动量p_\phi守恒
\\&守恒量\begin{cases}
L_z=I_{zz}(\dot\phi\cos\theta+\dot\psi)\\
L_Z=I_{xx}\dot\phi\sin^2\theta+I_{zz}\omega_z\cos\theta\\
E=\frac{1}{2}I_{xx}(\dot\theta^2+\dot\phi^2\sin^2\theta)+\frac{1}{2I_{zz}}L_z^2+mgl\cos\theta
\end{cases}
\\&\begin{cases}
进动角速度：\dot\phi=\frac{L_Z-L_z\cos\theta}{I_{xx}\sin^2\theta}\\
自转角速度：\dot\psi=\frac{L_z}{I_{zz}}-\frac{L_Z-L_z\cos\theta}\cos\theta\\
章动角速度（微分方程）E=\frac{1}{2}I_{xx}\dot\theta^2+\frac{(L_Z-L_z\cos\theta)^2}{2I_{xx}\sin^2\theta}+\frac{L_z^2}{2I_{zz}}+mgl\cos\theta
\end{cases}
\\&章动角不是无限制 的，只能介于最值之间反复震荡，z,Z两轴指向夹角的开合摆荡
\\&进动是z轴绕Z轴旋转，边自转边绕轴前进。章动和进动只描述转轴的运动

\end{align}
$$
	- 

$$
\begin{align} 
&快速自转的对称陀螺（陀螺仪），即自转角速度\dot\psi很大
\\&初始章动和进动角速度均为零，初始条件：\begin{cases}
\dot\theta(t=0)=0\qquad \dot\phi(t=0)=0\\
L_z=I_{zz}\dot\psi_0\qquad
L_Z=L_z\cos\theta_0\\
E=\frac{1}{2I_{zz}}L_z^2+mgl\cos\theta_0
\end{cases}
\\&此时\dot\theta_0=0，则\theta_0为极值，必为边界值
\\&\theta=\theta_1，\dot\theta_1=0时，守恒量方程\begin{cases}
L_z=I_{zz}(\dot\phi_1\cos\theta+\dot\psi_1)\\
L_Z=I_{xx}\dot\phi_1\sin^2\theta_1+L_{zz}\cos\theta_1\\
E=\frac{1}{2}I_{xx}(\dot\theta_1^2+\dot\phi_1^2\sin^2\theta_1)+\frac{1}{2I_{zz}}L_z^2+mgl\cos\theta_1
\end{cases}

\\&联立求解（存疑？）：\frac{I_{zz}^2\dot\psi_0^2}{2I_{xx}mgl}(\cos\theta_0-\cos\theta_1)=\sin^2\theta_1,\quad \theta_{min}<\theta_0<\theta<\theta_1=\theta_{max}
\\&p\gg e\Rightarrow pe=\sin^2\theta_0\Rightarrow 陀螺自转越快，偏离竖直越小，章动越小。自转越快，进动越慢


\end{align}
$$

## 弹性力学

### 基本概念

- 连续介质假设-质元模型而非质点，包括弹性体和流体，研究问题时需要首先满足连续介质假设，变形为小变形，固体为连续、均匀、各向同性。
- 

$$
\begin{align} 1.&应力(内力在微小截面的集中度)：\boldsymbol p=\frac{d\boldsymbol F}{dS},
\\&分量为垂直截面的正应力\sigma和平行截面的切应力\tau，
\\2.&应变(衡量单位质元变形程度)：正应变\varepsilon=\frac{\Delta x}{x_0}
\\&切应变\gamma=\Delta\theta(相互垂直的两条微小线段所夹角度改变值)
\\3.&胡克定律：\sigma=Y\varepsilon=Y\frac{\Delta l}{l_0},Y为杨氏模量，在比例限度内成立
\\4.&应力不超过比例极限，有泊松比：\nu=-\frac{\varepsilon'}{\varepsilon},即横纵应变之比为常数
\\&根据热力学原理，各向同性材料\nu取值为-1\le \nu\le -\frac{1}{2}
\\5.&体应变：\Theta=\frac{\Delta \Omega}{\Omega},且\sigma=K\Theta，K为体积模量，\frac{1}{K}为压缩率
\\&杨氏模量，体积模量和泊松比：K=\frac{Y}{3(1-2\nu)}
\\6.&扭转
\\7.&弯曲

\end{align}
$$

### 弹性形变的一般理论

### 弹性体动力学与弹性波

## 流体力学

### 流体的运动学

- 拉格朗日描述：追踪质元，质元轨迹为迹线
欧拉描述：观察位置上的质元，速度切线为流线
欧拉描述中，v不依赖于坐标称为均匀流动，不依赖于时间称定常流动

流体质元一般运动分解：
一般运动= 纯平移 + 纯旋转 + 线变形 + 切变形

$$
\begin{align} &欧拉描述中的局部(当地)导数：\frac{\partial \boldsymbol v}{\partial t}=\frac{\partial v_x}{\partial t}+\frac{\partial v_y}{\partial t}+\frac{\partial v_z}{\partial t}

\\&本体（物质）导数：\boldsymbol a=\frac{d \boldsymbol v}{d t}=\frac{\partial \boldsymbol v}{\partial t}+v_x\frac{\partial \boldsymbol v}{\partial x}+v_y\frac{\partial \boldsymbol v}{\partial y}+v_z\frac{\partial \boldsymbol v}{\partial z}=\frac{\partial \boldsymbol v}{\partial t}+(\boldsymbol v\cdot\nabla)\boldsymbol v
\\&对任意标志着流体质元性质物理量F，都有\frac{d \boldsymbol F}{d t}=\frac{\partial \boldsymbol F}{\partial t}+(\boldsymbol v\cdot\nabla)\boldsymbol F

\\&局部导数只描述固定点附近局部区域加速度，本体导数是流体质元真正加速度
\\&本体导数由非定常流动部分（当地导数）和非均匀流动部分（对流、迁移导数）组成
\\&单位时间管内截面通过质量为流量：Q=\int_S\rho \boldsymbol v\cdot d\boldsymbol S
\\&流体连续性定理:\int_V \frac{\partial \rho}{\partial t}dV=-\oint_S\rho \boldsymbol v\cdot d\boldsymbol S=-\int_V [\nabla\cdot(\rho\boldsymbol v)]dV
\\&则连续性方程：\frac{\partial \rho}{\partial t}+\nabla\cdot(\rho\boldsymbol v)=0，定常流动\nabla\cdot(\rho\boldsymbol v)=0


\end{align}
$$
- 

$$
\begin{align} &流速场\boldsymbol v(x,y,z,t)

\\&\begin{cases}
密度本体导数：\frac{d \boldsymbol \rho}{d t}=\frac{\partial \boldsymbol \rho}{\partial t}+(\boldsymbol v\cdot\nabla)\boldsymbol \rho
\\连续性方程：\frac{\partial \rho}{\partial t}+\nabla\cdot(\rho\boldsymbol v)=\frac{\partial \rho}{\partial t}+\rho\nabla\cdot\boldsymbol v+\nabla\cdot\boldsymbol v\rho=0
\end{cases}\Rightarrow 得到\frac{d \boldsymbol \rho}{d t}+\rho\nabla\cdot\boldsymbol v=0
\\&流体散度为0时，\frac{d \boldsymbol \rho}{d t}=0，密度为常数，称不可压缩流体
\\&仿照应变张量分析，\varepsilon,\Theta是线应变和体应变
\\&\nabla\cdot\boldsymbol v=
\frac{\partial v_x}{\partial x}+
\frac{\partial v_y}{\partial y}+
\frac{\partial v_z}{\partial z}=
\frac{\partial }{\partial t}\big(\frac{\partial s_x}{\partial x}\big)+
\frac{\partial }{\partial t}\big(\frac{\partial s_y}{\partial y}\big)+
\frac{\partial }{\partial t}\big(\frac{\partial s_z}{\partial z}\big)=\dot\varepsilon_x+\dot\varepsilon_y+\dot\varepsilon_z=\dot\Theta
\\&\nabla\times\boldsymbol v
=\bigg(\frac{\partial v_z}{\partial y}-\frac{\partial v_y}{\partial z}\bigg)\boldsymbol e_x+\bigg(\frac{\partial v_x}{\partial z}-\frac{\partial v_z}{\partial x}\bigg)\boldsymbol e_y+\bigg(\frac{\partial v_y}{\partial x}-\frac{\partial v_x}{\partial y}\bigg)\boldsymbol e_z
\\&
\quad=\frac{\partial d }{\partial dt}\bigg[\bigg(\frac{\partial s_z}{\partial y}-\frac{\partial s_y}{\partial z}\bigg)\boldsymbol e_x+\bigg(\frac{\partial s_x}{\partial z}-\frac{\partial s_z}{\partial x}\bigg)\boldsymbol e_y+\bigg(\frac{\partial s_y}{\partial x}-\frac{\partial s_x}{\partial y}\bigg)\boldsymbol e_z\bigg]
\\&\quad
=\frac{\partial  }{\partial t}\big(2\phi_x\boldsymbol e_x+2\phi_y\boldsymbol e_y+2\phi_z\boldsymbol e_z\big)=2\boldsymbol\omega
\\&流体旋度为0，不存在绕某点旋转，为无旋流动，
\\&速度可写成标量函数取梯度的速度势\psi：\boldsymbol v=\nabla\psi
\\&若流体还不可压缩，\nabla\cdot\boldsymbol v=\nabla\cdot(\nabla\psi)=\nabla^2\psi=0(拉普拉斯方程)
\\&速度\boldsymbol v的环流量即涡度\nabla\times\boldsymbol v=\boldsymbol\Omega=2\boldsymbol\omega的通量
\\&\Gamma_{v(C)}=\oint_C \boldsymbol {v\cdot dl}=\int_S(\nabla\times\boldsymbol v)\cdot d\boldsymbol S=\Phi_{\Omega(S)}

\end{align}
$$

### 理想流体的动力学

- 理想流体

	- 忽略黏性，不存在任何切向应力（剪切模量μ为0），系统为保守系统，机械能严格守恒。

即理想流体只存在正应力。

常用于低速运动的空气和水。
	- 开尔文环流定理：流体内任何一条闭合回路上速度环量为守恒量。

理想流体初始无旋则永久无旋，初始有旋则永久有旋，只能漂移不能产生或消灭。即涡度随流体一起运动。

理想流体中任一点所有方向正应力相等，应力大小与方向无关，则定义流体压强-p=σx=σy=σz。压强总是压缩的，拉伸应力为正，故加负号。

- 理想流体动力学方程

	- 

$$
\begin{align} &理想流体基本属性：密度场\rho(\boldsymbol r ,t)，压强场p(\boldsymbol r ,t)，流速场\boldsymbol v(\boldsymbol r ,t)
\\&基本方程应允许已知受力解得三个函数5个未知数
\\&\begin{cases}
\frac{\partial \rho}{\partial t}+\nabla\cdot(\rho\boldsymbol v)=0\\
\rho\frac{d\boldsymbol v}{d t}=\rho\frac{\partial \boldsymbol v}{\partial t}+\rho(\boldsymbol v\cdot\nabla)\boldsymbol v=-\nabla p+\boldsymbol{\bar f}，\boldsymbol{\bar f}=-\nabla\bar U (欧拉方程-推导)\\
\rho=\rho(p)(流体的状态方程-特性)
\end{cases}
\\&欧拉方程解释为单位体积收到的压强差导致得力=负的压强梯度
\\&流体静力学平衡：\boldsymbol{\bar f}=-\nabla p\Rightarrow \nabla(p+\bar U)=\boldsymbol 0
\end{align}
$$

- 不可压缩的
理想流体的
定常流动
-伯努利方程

	- 

$$
\begin{align} &\begin{cases}
\rho\frac{d\boldsymbol v}{d t}=-\nabla p+\boldsymbol{\bar f}\\
\frac{d \boldsymbol v}{d t}=\frac{\partial \boldsymbol v}{\partial t}+(\boldsymbol v\cdot\nabla)\boldsymbol v\\
矢量公式：\boldsymbol{(A\cdot\nabla)A+A\times(\nabla\times A)}=\frac{1}{2}\nabla|A|^2\\
定常流动：\frac{\partial \boldsymbol v}{\partial t}=0\\
不可压缩：\rho=\rho_0\\
外力保守：\boldsymbol{\bar f}=-\nabla\bar U 
\end{cases}
\\&\int_L\bigg[
\rho[(\nabla\times\boldsymbol v)\times\boldsymbol v]
+\nabla\bigg(\frac{1}{2}\rho v^2+p+\bar U\bigg)
\bigg]\cdot d\boldsymbol r=\boldsymbol 0 
\Rightarrow \frac{1}{2}\rho v^2+p+\bar U=常量（L）
\\&V=mgh：\frac{1}{2}\rho v^2+p+\rho gh=常量（L）,\quad \frac{v^2}{2g}+\frac{p}{\rho g}+h=常量（L）

\end{align}
$$

- 理想流体中的声波

	- 

$$
\begin{align} &欧拉方程存在非线性项：\rho\frac{\partial \boldsymbol v}{\partial t}+\rho(\boldsymbol v\cdot\nabla)\boldsymbol v=-\nabla p+\boldsymbol{\bar f}

\\&线性化/微扰法：只要扰动够小，那么非线性项就可以近似为线性项
\\&快速传播来不及交换热量，不受外力，不可压缩流体，声波状态方程：\frac{p}{p_0}=\big(\frac{\rho}{\rho_0}\big)\gamma
\\&欧拉方程组
\begin{cases}
\frac{\partial \rho}{\partial t}+\nabla\cdot(\rho  \boldsymbol v)=0\\
\rho\frac{\partial \boldsymbol v}{\partial t}+\rho(\boldsymbol v\cdot\nabla)\boldsymbol v=-\nabla p\\
\frac{p}{p_0}=\big(\frac{\rho}{\rho_0}\big)\gamma
\end{cases}
，一阶微扰分解
\begin{cases}
\rho(\boldsymbol r,t)=\rho_0(\boldsymbol r)+\rho_1(\boldsymbol r,t)\\
p(\boldsymbol r,t)=p_0(\boldsymbol r)+p_1(\boldsymbol r,t)\\
\boldsymbol v(\boldsymbol r,t)=0+\boldsymbol v_1(\boldsymbol r,t)
\end{cases}
\\&联立，只保留一阶，忽略零阶和高阶：\begin{cases}
\frac{\partial \rho_1}{\partial t}+\rho_0\nabla\cdot \boldsymbol v_1=0\\
\rho_0\frac{\partial \boldsymbol v_1}{\partial t}+\nabla p_1=\boldsymbol 0\\
p_1=\frac{\gamma p_0}{\rho_0}\rho_1
\end{cases}
\Rightarrow \begin{cases}\frac{\partial^2 \rho_1}{\partial t^2}=\bigg(\frac{\gamma p_0}{\rho_0}\bigg)\nabla^2 \rho_1
\\v_s=\sqrt{\frac{\gamma p_0}{\rho_0}}
\end{cases}


\end{align}
$$

### 黏滞流体的动力学

- 牛顿黏性定律
- 管道中的定常流动：泊肃叶公式
- 黏滞流体动力学方程：纳维-斯托克斯方程
- 雷诺数 · 从层流到湍流

## [非线性力学与混沌](https://zhuanlan.zhihu.com/p/500075340)

