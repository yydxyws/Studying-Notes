# 统计系综理论：
平衡态普遍理论

## 统计系综

### 处于相同条件下，微观组元和结构完全相同，并各自处于某个可能微观态，彼此独立的大量系统集合，称为统计系综。

- 系统处于各个微观态的概率=系综中该微观态的系统分配数目/系综中系统总数

### 经典情形

- 经典刘维尔定理

	- 系综密度函数不显含时间

### 量子情形

- 统计平衡条件（量子刘维尔定理）

## 微正则系综

### 定义

- 处于平衡态的孤立系统组成，每个系统能量相同且确定

### 经典与量子表达

### 微正则系综的熵

### 系综总结

- 

$$
\begin{align} 1.&微正则系综：在系统处于确定能量的特定宏观态定义熵的统计意义
\\&\boldsymbol {\Omega=e^{\beta T S}}\quad(从S=k_B\ln\Omega变形得到，此时一般为绝热孤立系统)
\\2.&正则系综：\boldsymbol {Z=e^{-\beta F}},F为亥姆霍兹函数
\\3.&巨正则系综：\boldsymbol {\mathcal Z=e^{-\beta \Phi_G}},\Phi_G为巨势

\end{align}
$$

## 正则系综与
玻尔兹曼分布

### 定义

- 通过热交换与大热源达成热平衡的封闭系统组成，每个系统温度相同且确定。

正则系综遵从玻尔兹曼分布（正则分布）

### 微正则系综推导正则系综

### 能量均分定理

- 大量粒子组成的经典系统，热平衡时内能均匀分布于系统的粒子可及的每个二次自由度上。

$$
\begin{align} &系统能量往往依赖于某个变量的平方，这样的系统与热源相互作用，求系统平均热能

\\&E=ax^2,P(x)=\frac{e^{-\beta ax^2}}{\int_{-\infty}^{\infty}e^{-\beta ax^2}dx},
\left \langle E\right \rangle=\int_{-\infty}^{\infty}EP(x)dx=\frac{\int_{-\infty}^{\infty}ax^2e^{-\beta ax^2}dx}{\int_{-\infty}^{\infty}e^{-\beta ax^2}dx}=\frac{1}{2\beta}=\frac{1}{2}k_BT
\\&能量均分定理：(系统每个平方形式能量依赖关系称为一个模或自由度，弹簧有两个)
\\&若一个经典系统能量是n个相互独立的平方模之和，且该系统与温度为T热源进行热接触，
\\&则系统平均能量: \langle E \rangle=n\times\frac{1}{2}k_BT

\\&这说明能量在系统所有独立模之间平均分配\frac{1}{2}k_BT能量

\end{align}
$$
- 应用

$$
\begin{align} 1.&单原子气体中的平动
\\&E=\frac{1}{2}mv_x^2+\frac{1}{2}mv_y^2+\frac{1}{2}mv_z^2 \Rightarrow 
\langle E \rangle=3\times\frac{1}{2}k_BT=\frac{3}{2}k_BT
\\2.&双原子气体中的转动
\\&E=\frac{1}{2}mv_x^2+\frac{1}{2}mv_y^2+\frac{1}{2}mv_z^2+\frac{L_1^2}{2I_1}+\frac{L_2^2}{2I_2} \Rightarrow 
\langle E \rangle=5\times\frac{1}{2}k_BT=\frac{5}{2}k_BT
\\&沿着双原子键轴方向转动模常温下对应转动动能极大，不能被激发，忽略
\\3.&双原子气体中的振动（多了相对运动动能和化学键势能）
\\&E=\frac{1}{2}m(v_x^2+v_y^2+v_z^2)+\frac{L_1^2}{2I_1}+\frac{L_2^2}{2I_2}+ \frac{1}{2} \mu(\boldsymbol{\dot r_1-\dot r_2})^2+\frac{1}{2} k(|\boldsymbol{\dot r_1-\dot r_2}|-l_0)^2
\\&\Rightarrow 
\langle E \rangle=7\times\frac{1}{2}k_BT=\frac{7}{2}k_BT
\\&\gamma=\frac{c_p}{C_V}=\frac{(\frac{n}{2}+1)R}{\frac{n}{2}R}=1+\frac{2}{n}
\\4.&固体热容(原子固定在晶格上只有热振动，化学键看做弹簧)
\\&每个原子6根弹簧，N个原子分到3N个弹簧，每个弹簧两个模
\\&\Rightarrow 
\langle E \rangle=3\times2\times\frac{1}{2}k_BT=3k_BT
\\&固体摩尔热容预期为3N_Ak_B=3R(杜隆帕蒂定律)

\end{align}
$$
- 要求热能远大于量子化能级之间间隔：kT>>hω，使得能量的参数可以对变量连续积分。

几乎所有势阱底部都趋近于近似的二次函数形式（泰勒展开），称为简谐近似。温度过高，高阶项不能省略。

即：能够忽略能谱量子性质，同时相关势阱简谐近似，能量均分定理成立。

### 实际气体

- 范德瓦尔斯气体状态方程

$$
(p+\frac{a}{V_m^2})(V_m-b)=RT
$$

	- 

$$
\begin{align} &对N个单原子分子经典气体：E=\sum_{i=1}^{N}\frac{p_i^2}{2m}+\sum_{i<j}\phi(r_{ij})
\\&
\\&
\\&
\\&
\\&
\\&
\\&
\\&
\\&
\\&
\\&
\\&
\end{align}
$$

- 迪特里奇状态方程

$$
p(V_m-b)=RTe^{-a/RTV_m}
$$
- 气体的位力展开

$$
\frac{pV_m}{RT}=1+\frac{B}{V_m}+\frac{C}{V_m^2}+\dots
$$
- 对应态定律
- 冷却真实气体

	- 焦耳膨胀
	- 等温膨胀
	- 焦耳-汤姆逊膨胀
	- 气体液化
	- 绝热去磁

## 巨正则系综与
吉布斯分布

### 定义

- 与大热源和大粒子源达到平衡的开放系统，每个系统温度和化学势相同

### 微正则系综导出巨正则系综

### 吉布斯分布

- 吉布斯分布推导

	- 

$$
\begin{align} &一个热和粒子源，粒子数\mathcal N-N，能量E-\varepsilon,微观状态数\Omega(E-\varepsilon)
\\&一个小系统，固定体积V，能量\varepsilon，含N个粒子,\mathcal N\gg N,E\gg \varepsilon
\\&对源的熵在\varepsilon=0,N=0处进行泰勒展开\\&\quad S(U-\varepsilon,\mathcal N-N)=S(U,\mathcal N)-\bigg(\frac{\partial S}{\partial U} \bigg)_{N,V}-\bigg(\frac{\partial S}{\partial N} \bigg)_{U,V}=S(U,\mathcal N)-\frac{\varepsilon-\mu N}{T}
\\&系统处在该能量和粒子数概率P(\varepsilon,N)\propto \Omega_{(E-\varepsilon,\mathcal N-N)}=e^{S_{(E-\varepsilon,\mathcal N-N)}/k_B}\propto
e^{\beta(\mu N-\varepsilon)}

\\&即吉布斯分布（巨正则分布）：P(\varepsilon,N)\propto
e^{\beta(\mu N-\varepsilon)}P(\varepsilon)\propto e^{-\frac{\varepsilon}{k_BT}}
\end{align}
$$

- 巨配分函数

	- 

$$
\begin{align} &归一化后：P_i=P(E_i,N_i)=\frac{e^{\beta(\mu N_i-E_i)}}{\mathcal Z},
\\&巨配分函数\boldsymbol {Z=\sum_i e^{\beta(\mu N_i-E_i)}}=\sum_{N=0}^{\infty}\sum_{s} e^{\beta\mu N-\beta E_s}=\sum_{N=0}^{\infty}\sum_{s} e^{-\alpha N-\beta E_s}
\\&两重求和：在某粒子数N下对所有微观状态求和，在对所有可能粒子数求和
\\&化学势为零不能说明粒子数不变，例如光子气体系统
\\
\\&巨配分函数结合统计平均值导出热力学量：
\\&N=\sum_i N_iP_i=\frac{1}{\mathcal Z}\bigg( -\frac{\partial }{\partial \alpha} \bigg)\sum_{N=0}^{\infty}\sum_{s} e^{-\alpha N-\beta E_s}=-\frac{\partial \ln \mathcal Z}{\partial \alpha}=k_BT\bigg(\frac{\partial \ln \mathcal Z}{\partial \mu}  \bigg)_\beta
\\&U=\sum_i E_iP_i=\frac{1}{\mathcal Z}\bigg( -\frac{\partial }{\partial \beta} \bigg)\sum_{N=0}^{\infty}\sum_{s} e^{-\alpha N-\beta E_s}+\mu N=-\bigg(\frac{\partial \ln \mathcal Z}{\partial \beta}  \bigg)_\mu+\mu N
\\&S=\sum_i (-k_B\ln P_i )P_i=k_B\bigg(\ln \mathcal Z-\alpha\frac{\partial\ln\mathcal Z}{\partial\alpha}-\beta\frac{\partial\ln\mathcal Z}{\partial\beta}\bigg)=\frac{U-\mu N+k_BT\ln \mathcal Z}{T}
\\&Y=\sum_i (\frac{\partial E}{\partial y})P_i
=\frac{1}{\mathcal Z} \sum_{N=0}^{\infty}\sum_{s}\frac{\partial E_s}{\partial y} e^{-\alpha N-\beta E_s}

=\frac{1}{\mathcal Z}\big( -\frac{1}{\beta}\frac{\partial }{\partial y} \big)\sum_{N=0}^{\infty}\sum_{s} e^{-\alpha N-\beta E_s}= -\frac{1}{\beta}\frac{\partial \ln\mathcal Z}{\partial y}
\\&p=\frac{1}{\beta}\frac{\partial \ln\mathcal Z}{\partial V}
\end{align}
$$

### 化学势与化学反应

- 向系统中加入粒子而不改变系统体积或熵，系统的内能改变量即化学势μ。

dN对小尺度粒子，加入电子，化学势μ不连续的跃变
- 

$$
\begin{align} &dU=TdS-pdV+\mu dN,
\\&\mu=\bigg(\frac{\partial U}{\partial N} \bigg)_{S,V}=\bigg(\frac{\partial F}{\partial N} \bigg)_{T,V}=\bigg(\frac{\partial G}{\partial N} \bigg)_{p,V}

\\&S=S(U,V,N),dS=\frac{dU+pdV-\mu dN}{T}
\\&dS=\bigg(\frac{\partial S}{\partial U} \bigg)_{N,V} dU+\bigg(\frac{\partial S}{\partial V} \bigg)_{N,U} dV+\bigg(\frac{\partial S}{\partial N} \bigg)_{U,V} dN
\\&\bigg(\frac{\partial S}{\partial U} \bigg)_{N,V}=\frac{1}{T},\bigg(\frac{\partial S}{\partial V} \bigg)_{N,U} =\frac{p}{T},\bigg(\frac{\partial S}{\partial N} \bigg)_{U,V}  =\frac{-\mu }{T}

\end{align}
$$

	- 对于理想气体，N=1时，化学势可以看做单粒子吉布斯函数。

$$
\mu=k_BT\ln(n\lambda_{th}^3)=\frac{G}{N}，G=\mu N
$$
	- 多种类型的粒子

$$
粒子项：\sum_i\mu_idN_i，dG=\sum_i\mu_idN_i
$$
	- 対粒子数不守恒的系统，化学势等于0，例如光子。

- 巨势

	- 

$$
\begin{align} &定义态函数-巨势：\mathcal Z=e^{-\beta \Phi_G}\Rightarrow\Phi_G=-k_BT\ln\mathcal Z

\\&则\Phi_G=-k_BT\ln\mathcal Z=U-TS-\mu N=F-\mu N
\\&则d\Phi_G=dF-\mu dN-Nd\mu
\\&又dF=-pdV-SdT+\mu dN，F=F(N,T,V)
\\&有d\Phi_G=-pdV-SdT-Nd\mu，\Phi_G=\Phi_G(\mu,T,V)
\\&有：S=-\bigg(\frac{\partial \Phi_G}{\partial T} \bigg)_{V,\mu}，p=-\bigg(\frac{\partial \Phi_G}{\partial V} \bigg)_{T,\mu}，N=\bigg(\frac{\partial \Phi_G}{\partial \mu} \bigg)_{T,V}
\\&若熵是一个广延性质，U-TS+pV=\mu N，则\Phi_G=-pV
\end{align}
$$

- 摩尔化学势与化学反应

### 渗透

