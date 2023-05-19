# 近独立子系的
最概然分布

## 近独立子系与
最概然分布

### 近独立子系

- 组成系统粒子相互作用很弱，可以忽略不计，以至于系统总能量等于各粒子能量之和。

需注意粒子如果完全无相互作用，则粒子不可能交换能量，系统不可能达到并保持平衡。

### 最概然分布

- 组成系统的粒子数目很大，出现几率最大的那个分布就等于平均分布。

成立前提：等概率原理，微观态连续变化，各态遍历假设
- 

$$
\begin{align} &对平衡态孤立系统，某微观分布对应系统微观态越大，分布出现的几率越大。
\\&即对微观分布\{a_l\}:P(\{a_l\})\propto \Omega(\{a_l\})
\\&微观状态数\Omega又称为热力学几率（未归一化的相对几率）


\end{align}
$$
- 最可几分布要点
对平衡态的孤立系统，先求出任意分布的相对几率（微观状态数）Ω，再利用拉格朗日乘子法找出宏观允许的分布中使得Ω取极大值的分布
粒子可分辨（定域系统）情形：麦克斯韦-玻尔兹曼分布
非定域玻色子系统：玻色-爱因斯坦分布
非定域费米子系统：费米-狄拉克分布

## 定域子系与
玻尔兹曼分布

### 概率观点

- 

$$
\begin{align} &一个热源，温度T，能量E-\varepsilon,微观状态数\Omega(E-\varepsilon)
\\&一个系统，\Omega=1，能量\varepsilon，处在该能量概率P(\varepsilon)\propto \Omega(E-\varepsilon)\times 1
\\&一阶展开:\ln\Omega(E-\varepsilon)=\ln\Omega(E)-\frac{d\ln\Omega(E)}{dE}\varepsilon=\ln\Omega(E)-\frac{\varepsilon}{k_BT}
\\&则有玻尔兹曼分布（正则分布）：P(\varepsilon)\propto e^{-\frac{\varepsilon}{k_BT}}
\\&P(E_r)=\frac{e^{-\frac{E_r}{k_BT}}}{\sum_i e^{-\frac{E_i}{k_BT}}},配分函数Z=\sum_i e^{-\frac{E_i}{k_BT}},玻尔兹曼因子e^{-\beta E}
\\&这种能量分布能够使得微观状态数目达到最大（系统选择最概然分布）
\end{align}
$$

### 微观状态观点

- 

$$
\begin{align} &汪书：粒子按能级的分布为\{a_l\},导出某个分布对应了多少微观状态
\\&已知第l能级上所有粒子个数为a_l,量子态个数为\omega_l,第
l个能级能量为\varepsilon_l

\\&玻色系统:每个能级\varepsilon_l上a_l个粒子占据\omega_l个量子态的方式
\\&玻尔兹曼系统：还需要关注每个能级\varepsilon_l上是哪a_l个粒子

\\&对平衡态孤立系统，必然有：\sum_l a_l=N，\sum_l a_l\varepsilon_l=E
\\&这是宏观状态对微观分布所加的约束条件


\end{align}
$$
- 详细推导

	- 

$$
\begin{align} 1.&玻尔兹曼系统：
\\&第l个能级上每个粒子占据一个量子态方式为\omega_l种，
\\&第l个能级上\omega_l个量子态，a_l个粒子分在不同量子态占据方式为\omega_l^{a_l}种
\\&每个粒子占据的微观状态（量子态）所处能级为\varepsilon_l可能性为l种，
\\&所有粒子占据的微观状态的能级分布可能性为\prod_l \omega_l^{a_l}种
\\&(此处已经包括了同能级不同量子态的交换)
\\&对N个粒子的N个位置，N个位置排列先后顺序有N!种排列方式
\\&对第l个能级的a_l个粒子，a_l个位置有a_l!种排列方式
\\&对N个粒子按顺序分成l份，第l份为a_l个粒子，一共\frac{N!}{\prod_l a_l!}种组合方式
\\&(交换不同能级的粒子才能得到系统新的状态，分子分母均包括了同能级不同量子态的交换)
\\&分成l组的N个粒子分配到不同的量子态，得到的微观状态有\frac{N!}{\prod_l a_l!}\prod_l \omega_l^{a_l}种
\\2.&玻色系统:
\\&粒子不可分别，每个量子态容纳粒子数无限制
\\&对第l个能级上的a_l个粒子分配进\omega_l个量子态中，\\&将a_l个粒子和\omega_l个量子态都看做排列元素，\\&且第一个量子态元素固定，一共(a_l+\omega_l-1)!种排列方式
\\&同能级粒子的交换a_l!不给出新的微观状态,而量子态的交换(\omega_l-1)!，但是其不需要交换
\\&N粒子玻色系统与分布\{a_l\}对应的可能微观状态数：\Omega_{B.E.}=\prod_l\frac{(a_l+\omega_l-1)!}{a_l!(\omega_l-1)!}
\\3.&费米系统：
\\&每个量子态最多只能容纳一个粒子，从\omega_l量子态中挑出a_l个被粒子占据(\omega_l\ge a_l)
\\&N粒子费米系统与分布\{a_l\}对应的可能微观状态数：\Omega_{F.D.}=\prod_l\frac{(\omega_l)!}{a_l!(\omega_l-a_l)!}

\end{align}
$$

- 

$$
\begin{align} &N粒子玻尔兹曼系统与分布\{a_l\}对应的可能微观状态数：\boldsymbol{\Omega_{M.B.}(\{a_l\})=\frac{N!}{\prod_l a_l!}\prod_l \omega_l^{a_l}}
\\&\ln \Omega(\{a_l\})=N(ln N-1)-\sum_l a_l(\ln a_l -1)+\sum _l a_l\ln \omega_l=Nln N-\sum_l a_l\ln\big(\frac{ a_l}{\omega_l})
\\&\delta\ln\Omega-\alpha\delta N-\beta\delta E=-\sum_l(\ln\frac{ a_l}{\omega_l}+\alpha+\beta\varepsilon_l)\delta a_l\Rightarrow\quad \ln\frac{ a_l}{\omega_l}+\alpha+\beta\varepsilon_l=0
\\&[麦克斯韦-玻尔兹曼分布]:\boldsymbol{a_l'=\omega_l e^{-\alpha-\beta\varepsilon_l}=\frac{\omega_l}{ e^{\alpha+\beta\varepsilon_l}}}，子系配分函数\boldsymbol{Z=\sum_l \omega_l e^{-\beta\varepsilon_l}}
\\
\\&N=\sum_l a_l=\sum_l\omega_le^{-\alpha-\beta \varepsilon_l}=e^{-\alpha}Z，\alpha=\ln\frac{Z}{N}
\\&E=\sum_l a_l\varepsilon_l=\sum_l\varepsilon_l\omega_le^{-\alpha-\beta \varepsilon_l}=e^{-\alpha}\sum_l\varepsilon_l e^{-\beta \varepsilon_l}=-\frac{N}{Z}\frac{\partial Z}{\partial \beta}=-N\frac{\partial\ln Z}{\partial \beta}
\\&经典统计中运动状态\varepsilon(\boldsymbol q,\boldsymbol p),pq为连续变量，不可数，故划分相格h^r=\prod_i\delta p_i\delta q_i,
\\&每个体积元\Delta\omega内相格个数即微观状态个数，即简并度从\omega_l变为\frac{\Delta\omega}{h^r}:
\\&\Omega_{cl}=\frac{N!}{\prod_l a_l!}\prod_l\bigg(\frac{\Delta\omega}{h^r}\bigg)^{a_l}，a_l'=\frac{\Delta\omega}{h^r} e^{-\alpha-\beta\varepsilon_l}，Z_1=\int e^{-\beta\varepsilon_l}\frac{d\omega}{h^r}=\int e^{-\beta\varepsilon_l(p,q)}\frac{\prod_i dp_idq_i}{h^r}
\end{align}
$$

### 配分函数与
热力学态函数

- 配分函数定义

	- 配分函数Z定义为对所有态的玻尔兹曼因子之和，每个态用指标α标记，所有热力学量都能有配分函数得到。

配分函数反映了Z量度能量如何在系统不同微观态之间被分割的方式。

统计力学问题步骤
（1）写出配分函数Z
（2）按照标准程序得到态函数

$$
Z=\sum_{\alpha}e^{-\beta E_\alpha}
$$

- 单粒子配分函数
实例(简并度均为1)

	- 二能级系统

		- 

$$
\begin{align} &系统能量\frac{\Delta}{2}或-\frac{\Delta}{2}，简并度\omega_l=1
\\&Z=\sum_{\alpha}e^{-\beta E_{\alpha}}=e^{-\beta \frac{\Delta}{2}}+e^{\beta \frac{\Delta}{2}}=2\cosh(\frac{\beta\Delta}{2})

\end{align}
$$
		- 自旋1/2顺磁体

			- 

$$
\begin{align} &磁场B沿z方向，自旋角动量1/2粒子存在于两个本征态之一,表现为一个二态系统
\\&态：|\uparrow\rangle,\mu_z=-\mu_B,E=\mu_BB；|\downarrow\rangle,\mu_z=\mu_B,E=-\mu_BB
\\&单粒子配分函数：Z_1=e^{\beta\mu_BB}+e^{-\beta\mu_BB}=2\cosh (\beta\mu_BB)
\\
\\&对N个粒子集合，自旋不相互作用，Z_N=Z_1^N=-Nk_BT\ln[2\cosh(\beta\mu_BB)]
\\&磁矩：m=-\bigg(  \frac{\partial F}{\partial B}\bigg)_T=N\mu_B\tanh(\beta\mu_BB)
\\&B很大、T很小时，\tanh 函数趋近1，m\rightarrow N\nu_B,所有磁矩指向上。
\\&T很大、B很小时，\tanh 函数趋近0，磁矩一半向上，一半向下。
\\&磁化强度：M=\frac{m}{V}=\frac{N\mu_B}{V}\tanh(\beta\mu_BB)，
\\&弱磁场下：x\ll1,\tanh x\approx, x,M\approx \frac{N\mu_B ^2B}{Vk_BT}
\\&弱磁材料(顺磁体):M\approx \chi H,\chi\ll 1,B=\mu_0(H+M)\approx (1+\chi)H\approx\frac{\mu_0 M}{\chi}
\\&则\chi\approx \frac{N\mu_B ^2\mu_0}{Vk_BT}\propto \frac{1}{T}，（居里定律）

\end{align}
$$

	- 简谐振子

		- 

$$
\begin{align} &系统能量(n+\frac{1}{2})\hbar\omega

\\&Z=\sum_{n=0}^{\infty}e^{-\beta (n+\frac{1}{2})\hbar\omega}=e^{-\beta \frac{1}{2}\hbar\omega}
\sum_{n=0}^{\infty}e^{-\beta n\hbar\omega}
\\&\quad=\frac{e^{- \frac{1}{2}\beta\hbar\omega}}{1-e^{-\beta \hbar\omega}}=\frac{1}{2\sinh(\frac{\beta \hbar\omega}{2})}
\\&
U=-\frac{d\ln Z}{d\beta}=\hbar\omega(\frac{1}{2}+\frac{1}{e^{\beta\hbar\omega}-1})
\end{align}
$$

	- N-能级系统

		- 

$$
\begin{align} &系统能量0,\hbar\omega,2\hbar\omega,\dots,(N-1)\hbar\omega
\\&Z=\sum_{j=0}^{N-1}e^{-j\beta \hbar\omega}=\frac{1-e^{- N\beta\hbar\omega}}{1-e^{-\beta \hbar\omega}}

\end{align}
$$

	- 转动能级

		- 

$$
\begin{align} &分子转动动能\frac{\hat J^2}{2I},
\\&系统能级：E_J=\frac{\hbar^2}{2I}J(J+1),J=0,1,\dots
\\&每个能级的简并度为(2J+1)
\\&Z=\sum_{\alpha}e^{-\beta E_{\alpha}}=\sum_{J=0}^{\infty}(2J+1)e^{-\frac{J(J+1)}{2}\beta \hbar^2}

\end{align}
$$

- 从单粒子配分函数
导出单粒子态函数

	- 

$$
\begin{align} 1.&内能:U=\frac{\sum_i E_i e^{-\beta E_i}}{\sum_i e^{-\beta E_i}}=-\frac{1}{Z}\frac{dZ}{d\beta}=\boldsymbol{-\frac{d\ln Z}{d\beta}}=k_BT^2\frac{d\ln Z}{dT}
\\&C_V=\big(\frac{\partial U}{\partial T}\big)_V=\frac{1}{\beta}\bigg[2\big(\frac{\partial\ln Z}{\partial T}\big)_V+T\big(\frac{\partial^2\ln Z}{\partial T^2}\big)_V\bigg]
\\
\\2.&熵:假设一个系统含有N个不同的等概率微观态，被分成各种宏观态
\\&第i个宏观态包含个n_i微观态，宏观态可通过实验区分,\sum_i n_i=N

\\&P_i=\frac{n_i}{N}，S_总=S_{测量宏观态}+S_{微观态}，\sum_i P_i=1
\\&S_总=k_B\ln N，S_{微观态}=\langle S\rangle=\sum_i P_i S_i,S_i=k_B\ln n_i
\\&S=S_总-S_{微观}=k_B(\ln N-\sum_i P_i\ln n_i)=k_B\sum_i P_i(\ln N-\ln n_i)=-k_B\sum_i P_i\ln P_i
\\&约束\sum_i P_i=1,\sum_i P_i E_i=U,拉格朗日乘子函数L(\alpha,\beta,P_i)=\frac{S}{k_B}-\alpha\sum_i P_i-\beta\sum_i P_i E_i
\\&用拉氏乘子法求S取极大值的分布：\frac{\partial }{\partial P_j}\sum_i(-P_i\ln P_i-\alpha P_i-\beta P_i E_i)=0
\\&\boldsymbol\Rightarrow -P_i\ln P_i-\alpha P_i-\beta P_i E_i=0\boldsymbol\Rightarrow P_i=\frac{e^{-\beta E_i}}{e^{1+\alpha}}=\frac{e^{-\beta E_i}}{Z}\boldsymbol\Rightarrow\ln P_i=-\beta E_i-\ln Z
\\&S=-k_B\sum_i P_i\ln P_i=k_B\sum_i P_i(\beta E_i+\ln Z)=\boldsymbol{k_B(\beta U+\ln Z)}=\frac{U}{T}+k_B\ln Z
\\
\\3.&亥姆霍兹函数：F=U-TS=-k_BT\ln Z \Rightarrow Z=e^{-\beta F}
\\&可以利用麦克斯韦关系式求出其他量
\\\\4.&压强：p=-\big(\frac{\partial F}{\partial V}\big)_T=\frac{1}{\beta}\big(\frac{\partial\ln Z}{\partial \ln V}\big)_T
\\\\5.&H=U+pV,\quad G=F+pV\dots
\end{align}
$$
	- 利用以上关系式可对不同配分函数练习，发现不同系统特性。尤其是低温和高温两种情况。双原子分子低温情况可导出理想气体性质。
	- 1.kBT<<最低能级与第一激发能级间隔，则系统处于最低能级

2.kBT>>最低能级与最高能级间隔，且能级数目有限，则每一能级都会有相同概率被占据

3.kBT>>相邻能级间隔，且能级数目无限，则平均能量随T线性增长，与能量均分定理结果一致。

### 热辐射与光子

- 

$$
\begin{align} &空腔中电磁波可用简谐振子描述，且每个模有色散关系\omega=ck，\frac{\omega}{k}=\frac{d\omega}{dk}
\\&三维电磁波有偏振态(两种可能极化)，则g(k)dk=\frac{Vk^2}{\pi^2}dk,g(\omega)=g(k)\frac{dk}{d\omega}=\frac{g(k)}{c},g(\omega)d\omega=\frac{V \omega^2d\omega}{\pi^2c^3}
\\
\\&\boldsymbol{对于简谐振子，单粒子配分函数Z=\frac{e^{- \frac{1}{2}\beta\hbar\omega}}{1-e^{-\beta \hbar\omega}}，U=-\frac{d\ln Z}{d\beta}=\hbar \omega(\frac{1}{2}+\frac{1}{e^{\beta \hbar\omega}-1})}
\\
\\&光子气体内能：U=\int_0^\infty g(\omega)d\omega\cdot \hbar \omega(\frac{1}{2}+\frac{1}{e^{\beta \hbar\omega}-1}),辐射场总自由度无穷大，真空能级无限大
\\&重新定义能量零点有：U=\int_0^\infty g(\omega)d\omega\cdot \hbar \omega\frac{1}{e^{\beta \hbar\omega}-1}=\frac{V\hbar}{\pi^2 c^3}\int_0^\infty \frac{\omega^3 d\omega}{e^{\beta \hbar\omega}-1}
\\&令x=\hbar \beta\omega，U=\frac{V\hbar}{\pi^2 c^3}\big(\frac{1}{\hbar\beta}  \big)^4\int_0^\infty \frac{x^3 dx}{e^x-1}=\big(\frac{V\pi^2k_B^4}{15c^3\hbar^3}  \big)T^4
\\&[黑体分布/普朗克辐射公式]：改写为谱能量密度形式，\begin{cases}
u_\omega=\frac{\hbar}{\pi^2c^3}\frac{\omega^3 }{e^{\beta \hbar\omega}-1}\\
u_\nu=\frac{8\pi h}{c^3}\frac{\nu^3 }{e^{\beta h\nu}-1}
\\u_\nu=\frac{8\pi hc}{\lambda^5}\frac{\nu^3 }{e^{\beta hc/\lambda}-1}
\end{cases}
\\&[瑞利金斯公式]：低频，长波长近似：u_\omega d\omega=\frac{\omega^2}{\pi^2c^3}k_BTd\omega
\\&[辐射亮度]:单位频率间隔内每立方弧度sr的辐射通量：B_\nu=\frac{c}{4\pi}u_\nu,同理B_\lambda=\frac{c}{4\pi}u_\lambda
\\&[维恩定律]：\frac{d u_\lambda}{d\lambda}=0\Rightarrow \lambda_{max}=Const
\\&[爱因斯坦系数]
\\&[布居反转]
\\&[宇宙微波背景辐射]

\end{align}
$$
- 

$$
\begin{align} 1.&证明体积为V光子气体的巨正则分布：\ln\mathcal Z=-\frac{V}{\pi^2c^3}\int_0^\infty \omega^2\ln(1-e^{-\beta \hbar\omega})d\omega=\frac{V\pi^2(k_BT)^3}{45\hbar^3c^3}
\\&U=-3F,pV=\frac{U}{3},S=\frac{4U}{3T}
\\2.&证明包含在体积V中黑体辐射总光子数N，与经典理想气体差别
\end{align}
$$

### 晶格振动与声子

- 声子

	- 量子化的格波，描述晶格振动的元激发。
关注系统的简正模，每个模包含整数个能量子，即声子。

- 爱因斯坦模型

	- 

$$
\begin{align} &固体所有振动模具有相同频率\omega_E，共3N个振动模，彼此独立且不相互作用
\\&Z=\prod_{k=1}^{3N} Z_k=(Z_k)^{3N}，Z_k=\frac{e^{- \frac{1}{2}\beta\hbar\omega_E}}{1-e^{-\beta \hbar\omega_E}}，\ln Z=\sum _{k=1}^{3N}\ln Z_k=3N\big[- \frac{1}{2}\beta\hbar\omega_E-\ln(1-e^{-\beta \hbar\omega_E})\big]
\\&U=-\frac{\partial \ln Z}{\partial \beta}=\frac{3N}{2}\hbar\omega_E+\frac{3N\hbar\omega_E}{e^{\beta \hbar\omega_E}-1}
\\&固体摩尔内能：U=3R\Theta_E(\frac{1}{2}+\frac{1}{e^{\Theta_E/T}-1})，定义温度\Theta_E=\frac{\hbar\omega_E}{R},x=\frac{\Theta_E}{T}=\frac{\hbar\omega_E}{k_BT}
\\&固体摩尔热容：C_p\approx C_V=\frac{\partial }{\partial T}=3R\Theta_E\frac{-e^{\Theta_E/T}}{(e^{\Theta_E/T}-1)^2}\big(-\frac{\Theta_E}{T^2}\big)=3R\frac{x^2e^x}{(e^x-1)^2}
\\&杜隆帕蒂定律：T\Rightarrow\infty,C\Rightarrow 3R
\end{align}
$$

- 德拜模型

	- 

$$
\begin{align} &假设（1）固体所有振动模的频率\omega符合频率分布函数（振动态密度）g(\omega)，且\int g(\omega)d\omega=3N

\\&爱因斯坦模型实质：g(\omega)=3N\delta(\omega-\omega_E)
\\&假设（2）晶格振动对应于具有相同速度v_s(固体声速)的一些波，设\omega=v_s q，q为晶格振动波矢
\\&即将固体看做具有线性色散关系的连续弹性介质
\\&V=L^3固体的三维情形晶格振动态密度g(q)dq=\frac{4\pi q^2dq}{(2\pi/L)^3}\times 3=\frac{3V q^2}{2\pi^2}dq，g(q)dq=\frac{3V \omega^2}{2\pi^2 v_s^3}d\omega
\\&注：晶格振动有三种可能极化（每个q一个纵向、两个横向极化）
\\&设直到最大频率（德拜频率）\omega_D的各种晶格振动均可能，\int_0^{\omega_D} g(\omega)d\omega=3N，\omega_D=\bigg( \frac{6N \pi^2 v_s^3}{V} \bigg)^{1/3}
\\&则g(\omega)d\omega=\frac{9N \omega^2}{\omega_D^3}d\omega，定义德拜温度\Theta_D=\frac{\hbar\omega_D}{k_B}，越硬材料声子频率越高。德拜温度越高
\\&德拜固体内能：U=\int_0^{\omega_D}g(\omega)d\omega\hbar\omega(\frac{1}{2}+\frac{1}{e^{\beta\hbar\omega}-1})=\frac{9}{8}N\hbar\omega_D+\frac{9N\hbar}{\omega_D^3}\int_0^{\omega_D}\frac{\omega^3d\omega}{e^{\beta\hbar\omega}-1}

\\&德拜固体摩尔热容：C=\frac{9N\hbar}{\omega_D^3}\int_0^{\omega_D}\frac{-\omega^3d\omega}{(e^{\beta\hbar\omega}-1)^2}e^{\beta\hbar\omega}\big(-\frac{\hbar\omega}{k_BT^2}\big)
=\frac{9R}{x_D^3}\int_0^{x_D}\frac{x^4e^xdx}{(e^x-1)^2}
\\&高温下，C\Rightarrow 3R，低温下,直接积分得到C=
\frac{12R\pi^4}{5x_D^3}=3R\times \frac{4\pi^4}{5}\big(\frac{T}{\Theta_D}\big)^3\propto T^3


\end{align}
$$

- 声子色散关系

	- 

$$
\begin{align} &单原子线性链振动：原子质量m，弹簧K，偏移平衡位置u_n，晶格间距a
\\&第n个原子：m\ddot u_n=K(u_{n+1}-2u_n+u_{n-1}),\omega_0^2=\frac{K}{m}

\\&其解必然为简谐波形式u_n=e^{i(\omega t-nqa)},代入整理得\omega=2\omega_0|\sin(\frac{qa}{2})|

\\&长波极限下，qa\rightarrow 0,有\omega\rightarrow v_s q,v_s=a\sqrt{\frac{K}{m}},\omega=v_s q

\\&声学支，光学支
\\&德拜：声学模，爱因斯坦：光学模

\end{align}
$$

### 理想气体

- 

$$
\begin{align} 1.&配分函数因子对系统所有态求和，这要求已知所有态的数目和每个态的能级（角标1表示单粒子）
\\&理想气体配分函数：Z_1=\int_{0}^{\infty} e^{-\beta E(\boldsymbol k)}g(\boldsymbol k)d\boldsymbol k，单分子能量：E(\boldsymbol k)=\frac{\boldsymbol p^2}{2m}=\frac{\hbar^2\boldsymbol  k^2}{2m}

\\&则有Z_1=\int_{0}^{\infty} e^{-\beta \frac{\hbar^2\boldsymbol  k^2}{2m}}\frac{V\boldsymbol k^2}{2\pi^2}d\boldsymbol k=\frac{V}{\hbar^3}\bigg(\frac{mk_BT}{2\pi}\bigg)^{3/2}=\frac{V}{\hbar^3}\bigg(\frac{m}{2\pi\beta}\bigg)^{3/2}=Vn_{Q}=\frac{V}{\lambda_{th}^3}

\\&量子密度：n_{Q}=\frac{1}{\hbar^3}\bigg(\frac{mk_BT}{2\pi}\bigg)^{3/2}，分子热波长：\lambda_{th}=n_{Q}^{-1/3}=\frac{h}{\sqrt{2\pi mk_B T}}
\\
\\2.&若N个粒子可分辨，则Z_N=(Z_1)^N
\\&若N个粒子不可分辨，近似忽略多个粒子占据相同能级的位形，仅考虑单一重复计算态数因子N!
\\&对不可分辨：Z_N=\frac{(Z_1)^N}{N!}，(粒子可及态数目远大于粒子数目，只有一个粒子占据任意给定态)
\\&理想气体热可及能级数远大于气体分子数，此时分子粒子数密度与态的量子密度为：n\ll n_Q
\\&满足如上条件，理想气体N粒子配分函数：Z_N=\frac{1}{N!}(\frac{V}{\lambda_{th}^3})^N=Const\frac{(VT^{3/2})^N}{N!}，n=\frac{N}{V}
\\&\ln Z_N=N\ln V+\frac{3N}{2}\ln T+Const
=N\ln V-3N\ln\lambda_{th}-N\ln N+N
\\&U=-\frac{d\ln Z_N}{d\beta}=k_BT^2\frac{d\ln Z_N}{d T}=\frac{3}{2}Nk_BT，F=-Nk_BT[\ln(n\lambda_{th}^3)-1]
\\&S=\frac{U-F}{T}=Nk_B[\frac{5}{2}-\ln(n\lambda_{th}^3)]，G=H-TS=Nk_BT\ln(n\lambda_{th}^3)
\end{align}
$$

	- 局域全同粒子可以通过便被物理位置变为可分辨的。
未标记的气体中的电子不可分辨。
位于特定磁轨道的电子是可分辨的。

### 相对论性气体

- 

$$
\begin{align} &E=pc=\hbar kc，g(k)dk=\frac{Vk^2dk}{2\pi^2}，\Lambda= \frac{\hbar c\pi^{2/3}}{k_BT}
\\&Z_1=\int_0^{\infty}e^{-\beta \hbar kc}\cdot g(k)dk=\frac{V}{\pi^2}\big(  \frac{k_BT}{\hbar c}\big)^3=\frac{V}{\Lambda^3}
\\&可导出：p=\frac{u}{3}
\end{align}
$$

## 非定域子系与
玻色/费米分布

### 交换对称性

- 二维还有任意子，具有分数统计
- 全同粒子波函数有两种交换对称性
- 交换对称性影响量子气体允许态的占据情况。低密度可忽略

### 全同粒子的分布
（微正则系综）

- 

$$
\begin{align} &N粒子费米系统与分布\{a_l\}对应的可能微观状态数：\Omega_{F.D.}=\prod_l\frac{(\omega_l)!}{a_l!(\omega_l-a_l)!}
\\&[费米-狄拉克分布]\boldsymbol{a_l'=\frac{\omega_l}{ e^{\alpha+\beta\varepsilon_l}+1}}
\\&S=k_B\ln\bigg[\prod_l\frac{(\omega_l)!}{a_l!(\omega_l-a_l)!}\bigg]\approx -k_B\sum_l\omega_l[a_l\ln a_l-\omega_l\ln\omega_l+(\omega_l-a_l)\ln(\omega_l-a_l)],
\\&上式考虑约束对\delta a_l变分取极大值得到每个量子态的平均占据数\frac{a_l}{\omega_l}=\frac{1}{e^{\alpha+\beta E_l}+1}

\\&经典极限条件a_l\ll \omega_l下,\Omega_{F.D.}\approx \prod_l\frac{\omega_l^{a_l}}{a_l!}=\frac{\Omega_{M.B.}}{N!}

\\\\&N粒子玻色系统与分布\{a_l\}对应的可能微观状态数：\Omega_{B.E.}=\prod_l\frac{(a_l+\omega_l-1)!}{a_l!(\omega_l-1)!}
\\&[玻色-爱因斯坦分布]\boldsymbol{a_l'=\frac{\omega_l}{ e^{\alpha+\beta\varepsilon_l}-1}}，同理\frac{a_l}{\omega_l}=\frac{1}{e^{\alpha+\beta E_l}-1}

\\&经典极限条件a_l\ll \omega_l下,\Omega_{B.E.}\approx \prod_l\frac{\omega_l^{a_l}}{a_l!}=\frac{\Omega_{M.B.}}{N!}

\end{align}
$$

### 全同粒子的统计
（巨正则系综）

- 

$$
\begin{align} &对玻色费米系统，利用巨配分函数最容易导出
\\1.&假设系统只有一个态\alpha能容纳粒子,每个粒子能量E，每个位形粒子数n，只需对位形求和
\\&\mathcal Z=\sum_\alpha e^{\beta(\mu N_\alpha-E_\alpha)}=\sum_n e^{n\beta(\mu-E)},
\langle n\rangle=\frac{\sum_n ne^{n\beta(\mu-E)}}{\sum_n e^{n\beta(\mu-E)}}=-\frac{1}{\beta\mathcal Z }\frac{\partial \mathcal Z}{\partial E}=-\frac{1}{\beta }\frac{\partial \ln\mathcal Z}{\partial E}
\\&对费米子，n=0,1，\mathcal Z=\sum_{n=0}^{1} e^{n\beta(\mu-E)}=1+e^{\beta(\mu-E)},\ln\mathcal Z=\ln(1+e^{\beta(\mu-E)})
\\&对玻色子，n从0到\infty，\mathcal Z=\sum_{n=0}^{\infty} e^{n\beta(\mu-E)}=\frac{1}{1-e^{\beta(\mu-E)}},\ln\mathcal Z=-\ln(1-e^{\beta(\mu-E)})
\\&则一个态中的平均粒子数：\langle n\rangle=-\frac{1}{\beta }\frac{\partial \ln\mathcal Z}{\partial E}=\frac{1}{e^{\beta(E-\mu)}\pm 1},费米子+，玻色子-。
\\2.&系统的第i个单粒子态能级E_i，在第i个态放入n_i个粒子，n_i为第i个态的占据数
\\&则系统的一个特定位形：[e^{\beta(\mu -E_1)}]^{n_1}\times [e^{\beta(\mu -E_2)}]^{n_2}\times\dots=\prod_ie^{n_i\beta(\mu -E_i)}
\\&巨配分函数\mathcal Z=\sum_{\{n_i\}}\prod_ie^{n_i\beta(\mu -E_i)}，\{n_i\}表示粒子对称性允许的占据数的一个集合，
\\&费米子\{n_i\}=\{0,1\}，，与i无关,\mathcal Z=\prod_i [1+e^{\beta(\mu-E_i)}]

\\&玻色子\{n_i\}=\{0,1,2\dots\}，与i无关,\mathcal Z=\prod_i\frac{1}{1-e^{\beta(\mu-E)}}
\\&第i个态的平均占据数：\langle n_i\rangle=-\frac{1}{\beta }\frac{\partial \ln\mathcal Z}{\partial E_i}=\frac{1}{e^{\beta(E_i-\mu)}\pm 1},费米子+，玻色子-。
\\3.&分布函数f即能量E_i的一个单粒子态平均占据数n_i：f(E)=\frac{1}{e^{\beta(E_i-\mu)}\pm 1},费米子+,玻色子-
\\&玻色子化学势总是低于最低能量态，否则发散
\end{align}
$$

### 量子气体和凝聚

- 无相互作用
的量子流体

	- 

$$
\begin{align} &对自旋为S的粒子，每个允许的动量态\boldsymbol k对应2S+1个可能的自旋态
\\&忽略粒子之间相互作用，巨配分函数即对各个态配分函数之积
\\&\quad\mathcal Z=\prod_k \mathcal Z_k^{2S+1},Z_k=[1\pm e^{-\beta(E_k-\mu)}]^{\pm1}
\\1.&三维气体巨势：\Phi_G=-k_BT\ln\mathcal Z=\mp k_BT(2S+1)\sum_k\ln[1\pm e^{-\beta(E_k-\mu)}]
\\&\qquad=\mp k_BT\int_0^\infty\ln(1\pm e^{-\beta(E_k-\mu)})g(E)dE
\\&态密度g(k)dk=\frac{4\pi k^2dk}{(2\pi/L)^3}\times(2S+1)=\frac{(2S+1)Vk^2}{2\pi^2}dk
\\&\Rightarrow
g(E)dE=\frac{(2S+1)VE^{1/2}dE}{(2\pi)^2}\bigg(\frac{2m}{\hbar^2}\bigg)^{3/2}\propto E^{1/2}
\\&分部积分得到：\Phi_G=-\frac{2}{3}\frac{(2S+1)V}{(2\pi)^2}\bigg(\frac{2m}{\hbar^2}\bigg)^{3/2}\int_0^\infty\frac{E^{3/2}dE}{e^{\beta(E-\mu)}\pm 1}
\\2.&波矢为\boldsymbol k的态的平均占据数n_{\boldsymbol k}=k_BT\frac{\partial \ln\mathcal Z_{\boldsymbol k}}{\partial \mu}=\frac{1}{e^{\beta(E_{\boldsymbol k}-\mu)}\pm 1}
\\&N=\sum_k n_{\boldsymbol k}=\int_0^\infty\frac{g(E)dE}{e^{\beta(E-\mu)}\pm 1},U=\sum_k n_{\boldsymbol k}E_{\boldsymbol k}=\int_0^\infty\frac{Eg(E)dE}{e^{\beta(E-\mu)}\pm 1}
\\&定义逸度z=e^{\beta\mu},\begin{cases}
N=\big[\frac{(2S+1)V}{(2\pi)^2}\bigg(\frac{2m}{\hbar^2}\bigg)^{3/2}\big]\int_0^\infty\frac{E^{1/2}dE}{z^{-1}e^{\beta E}\pm 1}\\
U=\big[\frac{(2S+1)V}{(2\pi)^2}\bigg(\frac{2m}{\hbar^2}\bigg)^{3/2}\big]\int_0^\infty\frac{E^{3/2}dE}{z^{-1}e^{\beta E}\pm 1},\Psi_G=-\frac{2}{3}U
\end{cases}
\\&\int_0^\infty\frac{E^{n-1}dE}{z^{-1}e^{\beta E}\pm 1}=(k_BT)^n\Gamma(n)[\mp Li_n(\mp z)]，\lambda_{th}=\frac{h}{\sqrt{2\pi mk_BT}}=\hbar\sqrt{\frac{2\pi}{mk_BT}},
\\&N=\frac{(2S+1)V}{\lambda_{th}^3}[\mp Li_{3/2}(\mp z)]，U=\frac{3}{2}Nk_BT\frac{Li_{5/2}(\mp z)}{Li_{3/2}(\mp z)}
\\&选取z=e^{\beta\mu}\ll 1,即(\frac{N}{V})\lambda_{th}^3\ll 1,此时Li_n(z)\approx z
\end{align}
$$

- 理想费米气体

	- 

$$
\begin{align} &考虑T=0，费米子占据最低能态，泡利不相容，每个能级l只有2S+1个费米子，
\\&直至填充到达费米能级E_F,即绝对零度费米子最高态占据的能量,且此时\beta\Rightarrow \infty
\\&利用差分\mu(T=0)=\frac{\partial E}{\partial N}=E(N)-E(N-1)=E_F定义：E_F=\mu(T=0)
\\&绝对零度态\boldsymbol k占据数f(E_k)=n_k=\frac{1}{e^{\beta(E_k-\mu)}+ 1}=\theta(\mu-E_k)=\theta(E_F-E_k),\theta(x)为阶跃函数
\\&绝对零度费米子数数:N=\int_0^{k_F} f(E_k)g(\boldsymbol k)d\boldsymbol k=\frac{(2S+1)V}{2\pi^2}\frac{k_F^3}{3},\\&费米波矢k_F,费米能级E_F=\frac{\hbar^2k_F^2}{2m}=\frac{\hbar^2}{2m}\big(\frac{6\pi^2 n}{2S+1}\big)^{2/3}

\end{align}
$$
	- 金属中的电子，费米温度T_F=E_F/k_B一般极高，使得f(E)= 1恒成立，故对多数金属，低于熔点的几乎所有温度，费米函数非常接近于阶跃函数.

这种情况下，金属中电子处于简并极限。(非相对论电子)

费米面是k空间中能量与化学势相等的点的集合，存在于晶体金属的周期势导致能隙形成，即其中没有允许的量子态。化学势处在能带之间的能隙中，则材料是半导体或绝缘体，没有费米面。

$$
\begin{align} &\Phi_G=-pV恒成立，又量子气体中\Phi_G=-\frac{2}{3}U，得到金属电子压强：p=\frac{2U}{3V}
\\&T=0时，\langle E\rangle=\frac{\int_0^\infty Eg(E)dE}{\int_0^\infty g(E)dE}=\frac{3}{5}E_F

\end{align}
$$

- 理想玻色气体

	- 光子气体

$$
\begin{align} &光子自旋为1，但0态不允许，简并因子为2
\\&无质量的光子引力子都只有两个CPT下对称的态，
\\&利用E=\hbar kc得到g(E)dE=\frac{V}{\pi^2\hbar^3 c^3}E^2dE
\\&U=\int_0^\infty \frac{Eg(E)dE}{z^{-1}e^{\beta E}-1}=\frac{V}{\pi^2\hbar^3 c^3}\int_0^\infty \frac{E^3dE}{z^{-1}e^{\beta E}-1}=(k_BT)^4\Gamma(4)Li_4(z)
\\&光子化学势\mu=0,z=1,Li_4(z)=\zeta(4)=\frac{\pi^4}{90},U=\frac{V\pi^2}{15\hbar^3 c^3}(k_BT)^4


\end{align}
$$
	- 玻色-爱因斯坦凝聚(BEC)

$$
\begin{align} &具有色散关系像E=\frac{\hbar^2k^2}{2m}一样（无隙色散,k=0或无限波长的最低能级处于零能处）的玻色系统

\\&化学势必须是负的，否则E=0能级出现无限的占据。因此逸度也要满足0<z<1。
\\&整理玻色气体粒子数方程:Li_{3/2}(z)=\frac{n\lambda^3_{th}}{2S+1}=\frac{h^3}{(2\pi mk_B T)^{3/2}}\frac{n}{2S+1}，z=e^{\frac{\mu}{k_BT}}
\\&数学处理失效分析：求解巨配分函数将求和化为积分近似失效
\\&临界温度：T_c=\frac{2\pi\hbar^2}{mk_B}[\frac{n}{2.612(2S+1)}]^{2/3}
\\&低于T_c时，基态上有宏观数量粒子占据的现象称为玻色-爱因斯坦凝聚，是k空间的凝聚
\\&这种转变不是由粒子间相互作用驱动，而是玻色子量子统计交换对称性要求
\\&【超流体】【超冷原子气体】【激光制冷】

\end{align}
$$

## 非简并性条件
经典极限条件
粒子可分辨性

### 

$$
\begin{align} &统计力学中的量子性质：能量量子化和粒子全同性原理（定域子系不成立）
\\1.&微观粒子全同性影响可以忽略
\\&定域子系或者满足经典极限条件（非简并性条件）：任一能级粒子数均远小于量子态数
\\&\frac{a_l}{\omega_l}\ll 1，或n\ll n_Q
\\&对满足经典极限条件的玻色、费米系统，S和F等与微观状态数有关的量需要计入因子N!
\\2.&能量量子化的影响可以忽略
\\&能级密集，任意两个相邻能级能量差远小于k_BT:\frac{\Delta\varepsilon}{k_BT}\ll 1
\end{align}
$$

## 课后习题

### 热物理概念：
10:1-6
17:1-7
20:1-9
21:4-6
22:1-7
23:5-7
24:3-7
25:1-3
28:1-6
29:5-6
30:1-6

