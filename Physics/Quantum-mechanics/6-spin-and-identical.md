# 自旋与全同粒子

## 电子自旋

### 电子自旋假设

- 

$$
\begin{align} 假设：&1.每个电子都具有内禀(自旋)角动量\vec s,在空间任意方向，自旋角动量投影取值只能为s_z=\pm \frac{1}{2}\hbar

\\&2.每个电子都具有自旋磁矩:\vec \mu_s=-\frac{e}{m}\vec s，磁矩空间投影为\mu_{s,z}=\pm \frac{e\hbar}{2m_e}=\pm \mu_B
\\定义：&作为算符本征值的各角动量
\begin{cases}
L=\sqrt{l(l+1)}\hbar,\quad l=0,1,\dots,(n-1) &\mbox{l为轨道角动量量子数}\\
S=\sqrt{s(s+1)}\hbar,\quad s=\frac{1}{2} &\mbox{s为自旋角动量量子数}\\
J=\sqrt{j(j+1)}\hbar,\quad j=l\pm s=l\pm \frac{1}{2} &\mbox{j为总角动量量子数}
\end{cases}\\&
\begin{cases}
L_z=m_l\hbar,\quad m_l=0,\pm 1,\dots ,\pm l& m_l 为轨道磁量子数\\
S_z=m_s\hbar,\quad & m_s=\pm\frac{1}{2},\quad\vec s=\frac{\sqrt{3}}{2}\hbar) 为轨道磁量子数
\end{cases}


\\&电子自旋磁矩相对轨道磁矩只有平行或反平行两种情形，\\&则外磁场与自旋磁场相互耦合产生的相互作用能\Delta E有两种取值

\end{align}
$$

### 自旋角动量

- 

$$
\begin{align} &自旋角动量S:与坐标、动量无关，表征电子内部状态,无法用坐标描述
\\&\vec S\times \vec S=i\hbar \vec S,\quad [S_x,S_y]=i\hbar S_z,在空间任意方向投影均为\pm\frac{\hbar}{2}
\\&S^2=\frac{3}{4}\hbar^2=s(s+1)\hbar^2,s=\frac{1}{2}为自旋量子数
\\&由于自旋本征态不是函数，使用右矢\ket{sm}标记两个量子数代表的量子态
\\&本征矢满足的代数关系：\begin{cases}
S^2\ket{sm}=s(s+1)\hbar^2\ket {sm}\\
S_z\ket{sm}=m\hbar\ket{sm}\\
S_\pm\ket{sm}=\sqrt{s(s+1)-m(m\pm 1)}\hbar\ket{s(m\pm 1)}
\end{cases}
\end{align}
$$

### 1/2自旋

- 子主题 1

$$
\begin{align} &1/2自旋：质子，中子，电子，夸克，轻子.S^2和S_z本征态只有两个
\\态：&\begin{cases}
上自旋态：\ket{\frac{1}{2},\frac{1}{2}}&\ket{\uparrow}&\ket{+}&\ket{\frac{1}{2}}&\chi_+=\left [ \begin{matrix}
1\\0 \\
\end{matrix} \right ]&本征值\frac{\hbar}{2}
\\
下自旋态：\ket{\frac{1}{2},{-\frac{1}{2}}}
&\ket{\downarrow}&\ket{-}&\ket{-\frac{1}{2}}&\chi_-=\left [ \begin{matrix}
1\\0 \\
\end{matrix} \right ]&本征值-\frac{\hbar}{2}
\end{cases}
\\&s=\frac{1}{2}的一般态表示为本征态线性组合：\chi=\left [ \begin{matrix}
a \\b \\
\end{matrix} \right ]=a\chi_++b\chi_-=a\left [ \begin{matrix}
1\\0 \\
\end{matrix} \right ]+b\left [ \begin{matrix}
0 \\1 \\
\end{matrix} \right ]
\\算符：&自旋算符为2\times 2矩阵
\\&\begin{cases}
S^2\chi_+=\frac{3}{4}\hbar^2\chi_+&S_z\chi_+=\frac{\hbar}{2}\chi_+\\
S^2\chi_-=\frac{3}{4}\hbar^2\chi_-
&S_z\chi_-=\frac{\hbar}{2}\chi_-
\end{cases}
\Rightarrow \color{orangered}S^2=\frac{3}{4}\hbar^2
\left [ \begin{matrix}
1& 0 \\
0& 1 \\
\end{matrix} \right ],
S_z=\frac{\hbar}{2}
\left [ \begin{matrix}
1& 0 \\
0& -1 \\
\end{matrix} \right ]
\\&\begin{cases}
S_-\chi_+=\hbar\chi_-,\quad S_+\chi_-=\hbar\chi_+\\
S_-\chi_-=S_+\chi_+=0
\end{cases}
\Rightarrow\color{orangered} S_+=\hbar
\left [ \begin{matrix}
0& 1 \\
0& 0 \\
\end{matrix} \right ],
S_-=\hbar
\left [ \begin{matrix}
0& 0 \\
1& 0 \\
\end{matrix} \right ](非厄米矩阵)
\\&\begin{cases}
S_x=\frac{1}{2}( S_++S_-)\\
S_y=\frac{1}{2i}( S_+-S_-)
\end{cases}
\Rightarrow\color{orangered} S_x=\frac{\hbar}{2}
\left [ \begin{matrix}
0& 1 \\
1& 0 \\
\end{matrix} \right ],
S_y=\frac{\hbar}{2}
\left [ \begin{matrix}
0& -i \\
i& 0 \\
\end{matrix} \right ]
\\&\color{orangered} 泡利算符\hat \sigma：S=\frac{\hbar}{2}\sigma，\vec{\sigma}\times\vec{\sigma}=2i\vec{\sigma}，\hat \sigma_i本征值为\pm 1
\\&\color{orangered} \sigma_i^2=1,且\sigma分量满足反对易关系：\sigma_x\sigma_y+\sigma_y\sigma_x=0

\\&\color{orangered} 泡利矩阵：\sigma_x=\begin{bmatrix}
0& 1\\
1& 0\\
\end{bmatrix}，
\sigma_y=\begin{bmatrix}
0& -i\\
i& 0\\
\end{bmatrix}
，\sigma_z=\begin{bmatrix}
1 & 0\\
0& -1\\
\end{bmatrix}
\\&本征旋量需满足归一化,\Braket{F}=\chi^+F\chi=\left [ \begin{matrix}
\Psi_1^*& \Psi_2^* \\
\end{matrix} \right ]\left [ \begin{matrix}
F_{11}&F_{12} \\
F_{21}& F_{22} \\
\end{matrix} \right ]
\left [ \begin{matrix}
\Psi_1\\\Psi_2\\
\end{matrix} \right ]
\end{align}
$$

### 磁场中的电子

- 拉莫尔进动

	- 

$$
\begin{align} &自旋1/2粒子静止在z方向均匀磁场中，\boldsymbol B=B_0\hat k，\boldsymbol H=-\gamma B_0S_z=-\frac{1}{2}\gamma B_0\hbar\left [ \begin{matrix}
1& 0 \\0& -1 \\
\end{matrix} \right ]
\\&\boldsymbol H与\boldsymbol S_z本征矢相同，\begin{cases}
\chi_+,E_+=-\frac{\gamma B_0 \hbar}{2}\\
\chi_-,E_-=\frac{\gamma B_0 \hbar}{2}
\end{cases},偶极矩平行磁场能量最低
\\&i\hbar\frac{\partial \chi}{\partial t}=\boldsymbol H\chi：
\begin{cases}
\chi(t)=a\chi_+ e^{-\frac{i}{\hbar}E_+ t}+b\chi_- e^{-\frac{i}{\hbar}E_- t}=
\left [ \begin{matrix}
ae^{\frac{i\gamma B_0 t}{2}} 
\\  be^{-\frac{i\gamma B_0 t}{2}} 
\end{matrix} \right ]，
\\
\chi(0)=\left [ \begin{matrix}
a
\\  b
\end{matrix} \right ]，|a|^2+|b|^2=1
\end{cases}
\\&令\begin{cases}
a=\cos\frac{\alpha}{2}\\b=\sin\frac{\alpha}{2}
\end{cases}，\chi(t)=
\left [ \begin{matrix}
\cos\frac{\alpha}{2}e^{\frac{i\gamma B_0 t}{2}} 
\\  \sin\frac{\alpha}{2}e^{-\frac{i\gamma B_0 t}{2}} 
\end{matrix} \right ]，
\begin{cases}
\Braket{S_x}=\chi(t)^+S_x\chi(t)=\frac{\hbar}{2}\sin\alpha \cos(\gamma B_0 t)\\
\Braket{S_x}=\chi(t)^+S_x\chi(t)=-\frac{\hbar}{2}\sin\alpha \sin(\gamma B_0 t)\\
\Braket{S_z}=\chi(t)^+S_z\chi(t)=\frac{\hbar}{2}\cos\alpha
\end{cases}
\\&\Braket S与z轴夹角为不变的倾角\alpha,且绕磁场旋转拉莫尔频率\omega=\gamma B_0

\end{align}
$$

- 施特恩-盖拉和实验

	- 量子态制备的范例
	- 

$$
\begin{align} &非均匀磁场\frac{\partial B_x}{\partial x}=\frac{\partial B_y}{\partial y}=0,F_z=\gamma S_z\frac{\partial B_z}{\partial z}
,观察到原子束分为2S+1个分离束
\\&经典讨论：\begin{cases}
\tan\alpha=\frac{F_zt}{mv}=\frac{F_zd}{mv^2},\\z_2=D\tan\alpha,\\mv^2=3kT
\end{cases}\Rightarrow z_2=\mu \cos\beta \frac{\partial B_z}{\partial z}\frac{dD}{3kT}
\\&量子讨论：运动坐标系中，H(t)=\begin{cases}
0&t<0或t>T\\
-\gamma B_zS_z &0<t<T
\end{cases}
\\&则\chi(t)=\begin{cases}
a\chi_++b\chi_-& t\le 0\\
a\chi_+e^{\frac{i\gamma B_z t}{2}}+b\chi_-e^{-\frac{i\gamma B_z T}{2}}& 0\le t\le T\\
a\chi_+e^{\frac{i\gamma B_z t}{2}}+b\chi_-e^{-\frac{i\gamma B_z T}{2}} & t\ge T
\end{cases}
\\&
\end{align}
$$

### 双粒子体系的自旋态

- 自旋单态与三重态

	- 

$$
\begin{align} &考虑两个自旋1/2的粒子：基态氢原子的电子和质子
\\&定态解得到四种状态,每个粒子的上下自旋态都用一个箭头表示：\begin{cases}
\ket{\uparrow\uparrow}=\ket{\frac{1}{2}\frac{1}{2}\frac{1}{2}\frac{1}{2}},m=1\\
\ket{\downarrow\uparrow}=\ket{\frac{1}{2}\frac{1}{2}\frac{-1}{2}\frac{1}{2}},m=0\\
\ket{\uparrow\downarrow}=\ket{\frac{1}{2}\frac{1}{2}\frac{1}{2}\frac{-1}{2}},m=0\\
\ket{\downarrow\downarrow}=\ket{\frac{1}{2}\frac{1}{2}\frac{-1}{2}\frac{-1}{2}},m=-1
\end{cases}
\\&实际上每个粒子都是处在上下自旋的线性组合态，复合体系则处于以上四个\ket{sm}态的线性组合态
\\&利用升降算符\begin{cases}
S_-=S_-^{(1)}+S_-^{(2)}\\
S_+=S_+^{(1)}+S_+^{(2)}
\end{cases}作用于以上四个态得到\color{orangered}\begin{cases}
s=1（三重态）\begin{cases}
\ket{11}=\ket{\uparrow\uparrow}\\
\ket{10}=\frac{1}{\sqrt 2}(\ket{\uparrow\downarrow}+\ket{\downarrow\uparrow})\\
\ket{1\text{-1}}=\ket{\downarrow\downarrow}
\end{cases}
\\
s=0（单态）\begin{cases}
\ket{00}=\frac{1}{\sqrt 2}(\ket{\uparrow\downarrow}-\ket{\downarrow\uparrow})

\end{cases}
\end{cases}
\\&则两个自旋1/2粒子组合总自旋s=0或s=1，取决于他们占据的是单态还是三重态
\\&\begin{cases}
S^2=(S^{(1)})^2+(S^{(2)})^2+2\boldsymbol S^{(1)}\cdot \boldsymbol S^{(2)}\\
\boldsymbol S^{(1)}\cdot \boldsymbol S^{(2)}=\sum_{x,y,z}S_i^{(1)}S_i^{(2)}
\end{cases},代入得本征矢：\color{orangered}\begin{cases}
三重态：&S^2\ket{10}=2\hbar^2\ket{10}\\
单态：&S^2\ket{00}=0\ket{00}
\end{cases}


\end{align}
$$

- CG系数

	- 

$$
\begin{align} &双粒子自旋态：\ket{s_1s_2m_1m_2},\begin{cases}
S^{(1)^2}\ket{s_1s_2m_1m_2}=s_1(s_1+1)\hbar^2\ket{s_1s_2m_1m_2}\\
S^{(2)^2}\ket{s_1s_2m_1m_2}=s_2(s_2+1)\hbar^2\ket{s_1s_2m_1m_2}\\
S_z^{(1)}\ket{s_1s_2m_1m_2}=m_1\hbar\ket{s_1s_2m_1m_2}\\
S_z^{(2)}\ket{s_1s_2m_1m_2}=m_2\hbar\ket{s_1s_2m_1m_2}
\end{cases}
\\&组合的自旋z分量：S_z\ket{s_1s_2m_1m_2}=(S_z^{(1)}+S_z^{(2)})\ket{s_1s_2m_1m_2}=m\hbar\ket{s_1s_2m_1m_2},m=m_1+m_2
\\&组合的总自旋量s：(s_1+s_2),(s_1+s_2-1),\cdots,|s_1-s_2|
\\&两粒子自旋同向平行，总自旋最大；自旋反向平行，总自旋最小
\\&两粒子复合体系的一般态：\ket{sm}=\sum_{m_1+m_2=m}C^{s_1s_2s}_{m_1m_2m}\ket{s_1m_1}\ket{s_2m_2}
\\&\sum_{m_1+m_2=m}C^{s_1s_2s}_{m_1m_2m}为克莱布希-高登系数（Clebsch-Gordan，CG）

\end{align}
$$

		- 

- 自旋纠缠态

## 电磁场中的粒子

### 电磁场中的薛定谔方程

- 

$$
\begin{align} &经典电动力学中，电荷q粒子受力\boldsymbol F=q(\boldsymbol  E+\boldsymbol v\times\boldsymbol  B),不能表示为标量势能函数的梯度
\\&但适用于i\hbar\frac{\partial \Psi}{\partial t}=H\Psi,H=\frac{1}{2m}(\boldsymbol p-q\boldsymbol A)^2+q\varphi,\begin{cases}
矢势\boldsymbol A：\boldsymbol B=\nabla\times \boldsymbol A\\
标势\varphi：E=-\nabla \varphi-\frac{\partial \boldsymbol A}{\partial t}
\end{cases}
\\&电磁场中的薛定谔方程(最小耦合规则)：i\hbar\frac{\partial \Psi}{\partial t}=\bigg[\frac{1}{2m}(-i\hbar\nabla-q\boldsymbol A)^2+q\varphi\bigg]\Psi
\\&此即洛伦兹力的量子表示方式
\\\\&埃伦费斯特定理：\frac{d\Braket{\boldsymbol r}}{t}=\frac{1}{m}\Braket{\boldsymbol p-q\boldsymbol A}
\\&m\frac{d\Braket{\boldsymbol v}}{t}=q\Braket{{\boldsymbol E}}+
\frac{q}{2m}\Braket{(\boldsymbol p\times\boldsymbol B-\boldsymbol B\times\boldsymbol p)}-\frac{q^2}{m}\Braket{(\boldsymbol A\times\boldsymbol B)}
\\&若E和B在波包所处体积内均匀，有m\frac{d\Braket{\boldsymbol v}}{t}=q(\boldsymbol E+\Braket{\boldsymbol v}\times \boldsymbol B)

\end{align}
$$

### 电磁场的规范不变性

- 

$$
\begin{align} &经典电动力学中，势A和\varphi不是唯一确定的，物理量是场E和B
\\&规范变换与规范不变性：\varphi'=\varphi-\frac{\partial \Lambda}{\partial t},\boldsymbol A'=\boldsymbol A+\nabla\Lambda,(\Lambda=\Lambda(r,t)的任意实函数)
\\&加上规范变换的势\varphi'和\boldsymbol A'满足薛定谔方程：\Psi'=e^{\frac{i}{\hbar}q\Lambda}\Psi，表示相同物理状态


\end{align}
$$
- 玻姆-阿哈拉诺夫效应
- 贝瑞相和贝尔相位

### 均匀磁场中各向同性带电谐振子的壳结构

### 超导现象

- 唯象描述
Meissner效应
超导环内的磁通量量子化

## 全同粒子体系

### 全同粒子

- 双粒子体系

	- 

$$
\begin{align} &势能不显含时间,对\psi(r_1,r_2)：-\frac{\hbar^2}{2m_1}\nabla_1^2\psi-\frac{\hbar^2}{2m_2}\nabla_2^2\psi+V(r_1,r_2)\psi=E\psi
\\1.&非相互作用粒子：V(r_1,r_2)=V(r_1)+V(r_2),\psi(r_1,r_2)=\psi_a(r_1)\psi_b(r_2),E=E_a+E_b
\\&\Psi(r_1,r_2,t)=\psi_ae^{-\frac{i}{\hbar}E_at}\psi_be^{-\frac{i}{\hbar}E_bt}
\\&线性组合满足纠缠态：不能写成单粒子态的乘积
\\2.&中心势场：V(r_1,r_2)\rightarrow V(|r_1-r_2|),两体问题等效为单体问题（仅适用于二体问题）
\\&对氢原子：R=\frac{m_1r_1+m_2r_2}{m_1+m_2},r=r_1-r_2,\mu=\frac{m_1m_2}{m_1+m_2},M=m_1+m_2
\\&定态薛定谔方程写作:\bigg[-\frac{\hbar^2}{2M}\nabla^2_R-\frac{\hbar^2}{2\mu}\nabla_r^2+V(r)\bigg]\psi(R,r)=E\psi(R,r)
\\&分离变量\psi(R,r)=\psi_R(R)\psi_r(r)\rightarrow [-\frac{\hbar^2}{2M}\nabla^2_R\psi_R]+[-\frac{\hbar^2}{2\mu}\nabla_r^2+V(r)\psi_r+V(r)]=E_R+E_r



\end{align}
$$

- 全同粒子与泡利原理

	- 

$$
\begin{align} &全同粒子：质量、电荷、自旋等固有性质完全相同的微观粒子
\\&全同性原理：全同粒子组成的体系中，两全同粒子调换不改变体系状态
\\&描述双粒子的波函数：\begin{cases}
可区分：\psi(\boldsymbol r_1,\boldsymbol r_2)=\psi_a(\boldsymbol r_1)\psi_b(\boldsymbol r_2)\\
玻色子：\psi_+(\boldsymbol r_1,\boldsymbol r_2)=\frac{1}{\sqrt 2}[\psi_a(\boldsymbol r_1)\psi_b(\boldsymbol r_2)+\psi_b(\boldsymbol r_1)\psi_a(\boldsymbol r_2)]\\
费米子：\psi_-(\boldsymbol r_1,\boldsymbol r_2)=\frac{1}{\sqrt 2}[\psi_a(\boldsymbol r_1)\psi_b(\boldsymbol r_2)-\psi_b(\boldsymbol r_1)\psi_a(\boldsymbol r_2)]

\end{cases}
\\&费米子：自旋为\frac{\hbar}{2}的奇数倍,两粒子不能占据同一状态,否则波函数为0,概率为0（泡利不相容原理）

\end{align}
$$

- 交换力与广义对称性

	- 

$$
\begin{align} 
&一维情况：两个粒子在\psi_a(x)态和\psi_b(x)态，\Braket{(x_1-x_2)^2}=\Braket{x_1^2}+\Braket{x_2^2}-\Braket{2x_1x_2}
\\&为便于操作，认为波函数没有重叠部分的电子可分辨。
\\&可区分：\psi(\boldsymbol x_1,\boldsymbol x_2)=\psi_a(\boldsymbol x_1)\psi_b(\boldsymbol x_2) 
\Rightarrow \Braket{(x_1-x_2)^2}_d=\Braket{x^2}_a+\Braket{x^2}_b-2\Braket{x}_a\Braket{x}_b
\\&
不可区分：\psi_\pm(\boldsymbol x_1,\boldsymbol x_2)=\frac{1}{\sqrt 2}[\psi_a(\boldsymbol x_1)\psi_b(\boldsymbol x_2)\pm \psi_b(\boldsymbol x_1)\psi_a(\boldsymbol x_2)]
\\&\Rightarrow \Braket{x_1^2}=\Braket{x_2^2}=\frac{1}{2}(\Braket{x^2}_a+\Braket{x^2}_b)
,\Braket{x_1x_2}=\Braket{x}_a\Braket{x}_b\pm|\Braket{x}_{ab}|^2
\\&\begin{cases}
玻色子：\Braket{(\Delta x)^2}_+=\Braket{(\Delta x)^2}_d - 2|\Braket{x}_{ab}|^2,趋向于靠近\\
费米子：\Braket{(\Delta x)^2}_-=\Braket{(\Delta x)^2}_d + 2|\Braket{x}_{ab}|^2，趋向于远离
\end{cases}
\\&称重叠时系统内部吸引或排斥的力为交换力，实质是量子中对称性要求的几何结果

\\\\&完整的电子态满足交换反对称，要考虑电子的自旋:\Psi=\psi(\boldsymbol r)\chi(\boldsymbol s)(位置和自旋解耦合)
\\&对两电子自旋合成态，\begin{cases}
自旋单态\chi(\boldsymbol s)反对称&要求空间波函数\psi(\boldsymbol r)对称
\\自旋三态\chi(\boldsymbol s)对称&要求空间波函数\psi(\boldsymbol r)反对称

\end{cases}
\\&空间函数对称，交换力使得电子聚拢到质子连线区域，质子受向内吸引力（共价键）

\\\\&广义对称原理：波函数是对称或反对称的，对称性不随时间改变
\\&定义交换算符Pf(\boldsymbol r_1,\boldsymbol r_2)=f(\boldsymbol r_2,\boldsymbol r_1),\hat P本征值为\pm 1\Rightarrow[\hat P,\hat H]=0,\frac{d\Braket{\hat P}}{dt}=0

\\&故\Ket{(1,\dots,i,\dots,j,\dots,n)}=\pm\ket{(1,\dots,j,\dots,i,\dots,n)},玻正费负

\end{align}
$$

### 原子

- 氦原子

	- 

$$
\begin{align} &假定原子核固定，单原子系统哈密顿量=N个单电子的势能和动能+不同电子排斥势能：
\\&\hat H=\sum_{j=1}^Z\bigg[-\frac{\hbar^2}{2m}\nabla_j^2-\bigg(\frac{1}{4\pi\varepsilon_0}\bigg)\frac{Ze^2}{r_j}\bigg]+\frac{1}{2}\bigg(\frac{1}{4\pi\varepsilon_0}\bigg)\sum_{j\ne k}^Z\frac{e^2}{|r_j-r_k|}
\\&H\psi=E\psi要求所有的解满足总波函数在交换任意两电子为反对称，且两电子不能占据同一个态
\\&实际只有Z=1能得到精确解，其余均需要借助近似方法和各种修正


\end{align}
$$

- 元素周期表

	- 

$$
\begin{align} &细节参见原子物理。（近似忽略所有电子间排斥力）
\\&轨道：每个电子占据的一个单粒子的类氢原子态
\\&单电子态：nl（n表示所处壳层，l表示轨道角动量）
，
\\&电子组态中指数用来表示某个态被几个电子占据

\\&洪特定则：\quad^{2S+1}L_J,用于表示某个原子总角动量J

\end{align}
$$

		- 
		- 
		- 

### 固体

- 索末菲自由电子气体理论

	- 

$$
\begin{align} &讨论方形固体，电子不受力，V(x,y,z)=\begin{cases}
0&0<x,y,z<l_x,l_y,l_z\\
\infty&Else
\end{cases}
\\&\begin{cases}
\psi(x,y,z)=\psi(x)\psi(y)\psi(z)\\
E=E_x+E_y+E_z
\end{cases}
\Rightarrow\begin{cases}
-\frac{\hbar^2}{2m}\frac{d^2X}{dx^2}=E_xX,&k_x=\frac{\sqrt{2mE_x}}{\hbar}\\
-\frac{\hbar^2}{2m}\frac{d^2Y}{dy^2}=E_yY,&k_y=\frac{\sqrt{2mE_y}}{\hbar}\\
-\frac{\hbar^2}{2m}\frac{d^2Z}{dz^2}=E_zZ,&k_z=\frac{\sqrt{2mE_z}}{\hbar}
\end{cases}
\\&边界条件：\begin{cases}
X(0)=Y(0)=Z(0)\\
X(l_x)=Y(l_y)=Z(l_z)=0
\end{cases}\Rightarrow
\begin{cases}
k_xl_x=n_x\pi\\k_yl_y=n_y\pi\\k_zl_z=n_z\pi
\end{cases}
\\&\begin{cases}
\psi_{n_xn_yn_z}=\sqrt{\frac{8}{l_xl_yl_z}}\sin(\frac{n_x\pi}{l_x}x)\sin(\frac{n_y\pi}{l_y}y)\sin(\frac{n_z\pi}{l_z}z)
\\E_{n_xn_yn_z}=\frac{\hbar^2\pi^2}{2m}(\frac{n_x^2}{l_x^2}+\frac{n_y^2}{l_y^2}+\frac{n_z^2}{l_z^2})=\frac{\hbar^2 k^2}{2m}
\\\boldsymbol k=(k_x,k_y,k_z)=(\frac{\pi}{l_x},\frac{\pi}{l_y},\frac{\pi}{l_z})
\end{cases}
\\&N个原子Nq个自由电子，泡利不相容，每个态两个相反自旋的电子
\\&每个单位方格代表一个态，每对电子在k空间所占用体积为\Omega=\frac{\pi^3}{l_xl_yl_z}=\frac{\pi^3}{V}
\\&每个态占据k空间一个球的1/8（因为方格是0\sim l_xl_yl_z）
\\&三维空间电子态对应等能面为费米球:\frac{1}{8}(\frac{4}{3}\pi k_F^3)=\frac{Nq}{2}\frac{\pi^3}{V}
\\&费米半径:k_F=(3\rho\pi^2)^{\frac{1}{3}},\rho=\frac{Nq}{V}为自由电子密度
\\&占据态和空态分界面为费米面，对应费米能量E_F=\frac{\hbar^2}{2m}(3\rho\pi^2)^{\frac{2}{3}}
\\&自由电子气体总能量：dE_{tot}=\int_0^{k_F}\frac{1}{8}4\pi k^2dk\cdot \frac{2}{\frac{\pi^3}{V}}\cdot \frac{\hbar^2k^2}{2m}=\frac{\hbar^2(3\pi^2Nq)^{\frac{5}{3}}}{10\pi^2m}V^{-\frac{2}{3}}
\\&对E求V导数，盒子扩大，能量下降，简并压：p=\frac{2E_{tot}}{3V}=\frac{\hbar^2(3\pi^2)^{\frac{2}{3}}}{5m}\rho^{\frac{5}{3}}
\\&简并压保证固体在低温不会坍缩，这来源于全同费米子反对称，与电子间排斥力和热运动无关

\end{align}
$$

- 布洛赫能带理论

	- 

$$
\begin{align} &布洛赫定理：对含周期势的薛定谔方程，解必满足\psi(x+a)=e^{iKa}\psi(x)
\\&证明：令D为位移算符:Df(x)=f(x+a),对周期势有[D,H]=0
\\&\quad 故本征函数满足D\psi(x)=\psi(x+a)=H\psi(x)=\lambda\psi(x)\rightarrow \lambda=e^{iKa}.完.
\\&\psi(x)不是周期函数，但是有|\psi(x+a)|^2=|\psi(x)|^2
\\&宏观晶体边界破坏周期势，修正周期为N\approx 10^{23}:\psi(x+Na)=\psi(x)\rightarrow K=\frac{2\pi n}{Na}


\end{align}
$$
	- [说明]粒子在周期势的稳态是行波的乘积的周期函数，电子速度非0
这意味着电子可以在没有散射的情况下穿过完美的晶体
哈密顿量平移不变不是稳态平移不变，而是稳态可被选择为平移算子本征态。平移算子是离散平移算符
	- 

$$
\begin{align} &一维狄拉克梳：由无数平均分布的\delta函数峰组成:V(x)=\alpha\sum_{j=0}^{N-1}\delta(x-ja)
\\&k=\frac{\sqrt{2mE}}{\hbar},x=0波函数连续：B=e^{-iKa}[A\sin(ka)+B\cos(ka)]
\\&波函数的差分与狄拉克函数强度正比：kA-e^{-iKa}k[A\cos(ka)-B\sin(ka)]=\frac{2m\alpha}{\hbar^2}B
\\&则\cos(Ka)=\cos(ka)+\frac{m\alpha}{\hbar^2k}\sin(ka)
\\&令z=ka,\beta=\frac{m\alpha a}{\hbar^2},则\cos(Ka)=f(z)=\cos (z)+\beta\frac{\sin (z)}{z}
\\&由于\cos(Ka)\le 1，则f(z)超出范围的间隙成为禁戒能量，被允许能量的能带分离
\\&三维势场中，仍有禁带分割允带，每条能带最多容纳两个电子
\\\\&更精细的模型：克勒尼希-彭尼模型（Kronig-Penney）：一维周期方势场

\end{align}
$$

### 量子统计力学

- 

$$
\begin{align} &在任意势场单粒子能量E_1,E_2,\dots,共d_n个能量为E_n的不同单原子态，势场放入N个粒子
\\&求解组态，即能量E_n的有N_n个粒子，取决于粒子可分辨或全同费米子、玻色子
\\&可分辨粒子：Q(N_1,N_2,\dots)=N!\prod_{n=1}^{\infty}\frac{d_n^{N_n}}{N_n!}
\\&全同费米子：Q(N_1,N_2,\dots)=\prod_{n=1}^{\infty}\frac{d_n!}{N_n!(d_n-N_n)!}
\\&全同玻色子：Q(N_1,N_2,\dots)=\prod_{n=1}^{\infty}\frac{(N_n+d_n-1)!}{N_n!(d_n-1)!}
\\&利用约束条件：\sum_{n=1}^{\infty}N_n=N,\sum_{n=1}^{\infty} N_nE_n=E,拉格朗日乘子法对N_n求导解最概然组态
\\&最概然占有数：\begin{cases}
可分辨粒子：N_n=d_ne^{-(\alpha+\beta E)}\\
全同费米子：N_n=\frac{d_n}{e^{\alpha+\beta E_n}+1}\\
全同玻色子：N_n=\frac{d_n}{e^{\alpha+\beta E_n}-1}
\end{cases}
\Rightarrow
\begin{cases}
\beta=\frac{1}{k_BT}\\
\mu(T)=-\alpha k_B T
\end{cases}
\end{align}
$$

