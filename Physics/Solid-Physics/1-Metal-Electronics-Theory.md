# 金属电子论

## 固体研究历史

### （金属最外层电子无相互作用，看做自由粒子气体，用麦克斯韦玻尔兹曼分布处理）Drude模型

### （麦克斯韦玻尔兹曼分布换成费米统计）索末菲自由电子模型

### （将固体电子运动问题，转化成单电子在正电背景下的周期性势场运动问题）布洛赫能带理论

### （无相互作用的电子态在绝热演化时可以一一对应的演化到有相互作用的电子态，称个体的“准粒子”）朗道费米液体理论

### （考虑了电子之间相互作用）Hatree-Fock模型

### （考虑电子之间交换关联能）DFT密度泛函理论

### 考虑电子轨道耦合的，考虑电声子耦合等等

## 金属自由电子模型

### Drude模型(经典电子气模型)

- 将金属中自由电子视为经典气体，遵从玻尔兹曼分布，并假设电子受到离子实散射，电子密度n和弛豫时间τ为独立参量。
成功说明欧姆定律、电导、热导联系。

### 金属电子气模型(现代量子)

- 将金属看做价电子构成的大量均匀量子金属自由电子气体（费米狄拉克统计）（索末菲模型）
基本参数：自由电子数密度和弛豫时间。

$$
\begin{align} &自由电子密度：n=\frac{N}{V}=N_A\frac{Zm}{MV}
\\&每个电子平均占据体积看做电子球：\frac{1}{n}=\frac{V}{N}=\frac{4}{3}\pi r_s^3

\end{align}
$$

### 基本假设

- 忽略价电子和离子实相互作用。
电子在表面势垒内自由运动，离子实充当均匀正电荷背景。
计算时，电子在金属中势能为常数，可取为0.
（自由电子近似）

	- 存在较大问题，进一步发展的理论更换为单电子近似

- 忽略电子间相互作用（独立电子近似）
- （弛豫时间近似）

### 金属基态性质
(绝对零度性质)

- 

$$
\begin{align} &T=0,V=L^3,N个自由电子，单电子近似
\\1.&单电子本征态(类自由电子)：\psi_k(r)=\frac{1}{\sqrt V}e^{i\boldsymbol{ k\cdot r}},能量:E=\frac{\hbar^2\boldsymbol k^2}{2m}动量：\boldsymbol p=\hbar\boldsymbol k
\\&周期性边界条件：波矢\boldsymbol k取值量子化，本征能量分立，
\\&每个点在k空间体积\Delta \boldsymbol k=(\frac{V}{8\pi^3})，单电子态密度\frac{1}{\Delta \boldsymbol k}=\frac{V}{8\pi^3}
\\2.&[电子是费米子]每个单电子态有两个自旋态，最多被两个自旋相反电子所占据
\\&[泡利不相容]N个电子逐级填充，在k空间形成费米球，球面为费米面，
\\&[费米分布]理想电子气热平衡态服从费米分布f(E)=n=\frac{1}{e^{\beta(E-\mu)}+ 1}，\lim_{T\rightarrow}f(E)=\begin{cases}
1,E<\mu\\
\frac{1}{2},E=\mu\\
0,E>\mu
\end{cases}
\\&[费米球与费米半径]根据k空间体积计算得到，费米半径k_F^3=3\pi^2n,绝对零度费米子数n=\frac{k_F^3}{3\pi^2}
\\&[费米能量]费米面上单电子态能量为费米能量\varepsilon_F=\frac{\hbar^2k_F^2}{2m},T=0时，\langle \varepsilon_F\rangle=\frac{\int_0^\infty \varepsilon g( \boldsymbol k)d \boldsymbol k}{\int_0^\infty g( \boldsymbol k)d \boldsymbol k}=\frac{3}{5}\varepsilon_F
\\&[单粒子态密度]k空间中单位体积的能量态密度：g(\boldsymbol k)d\boldsymbol k=2\times d\Omega =8\pi \boldsymbol k^2d\boldsymbol k
\Rightarrow g(\varepsilon)d\varepsilon=\frac{1}{\pi^2\hbar^3}\sqrt{2m^3\varepsilon}

\\&[费米面态密度]N=\frac{V}{3\pi^2}(\frac{2m\varepsilon}{\hbar^2})^{3/2},\ln N=\frac{3}{2}\ln\varepsilon+C,\frac{dN}{N}=\frac{3}{2}\frac{d\varepsilon}{\varepsilon}\Rightarrow g(\varepsilon)=\frac{dN}{d\varepsilon}=\frac{3N}{2\varepsilon}=\frac{mk_F}{\pi^2\hbar^2}

\end{align}
$$

### 温度T≠0的平衡态性质

- 电子比热

	- 

$$
\begin{align} &N个电子从0K加热至T(k_BT\ll \varepsilon),\Delta U=\int_0^\infty \varepsilon g(\varepsilon)f(\varepsilon)d\varepsilon
-\int_0^{\varepsilon_F} \varepsilon g(\varepsilon)f_{T=0}d\varepsilon
\\&N=\int_0^{\varepsilon_F} g(\varepsilon)d\varepsilon=\int_0^\infty g(\varepsilon)f(\varepsilon)d\varepsilon
\Rightarrow \varepsilon_F(\int_0^{\varepsilon_F}+\int_{\varepsilon_F}^\infty )g(\varepsilon)f(\varepsilon)d\varepsilon=\varepsilon_F \int_0^{\varepsilon_F} g(\varepsilon)d\varepsilon
\\&则\Delta U=\int_{\varepsilon_F}^\infty 
 (\varepsilon-\varepsilon_F) g(\varepsilon)f(\varepsilon)d\varepsilon
+\int_0^{\varepsilon_F}  (\varepsilon_F-\varepsilon) g(\varepsilon)[1-f(\varepsilon)]d\varepsilon
\dots
\\&索末菲幂级数公式，温度修正因子
\\&\boldsymbol{(T\ll T_F), C_{el}=\frac{\pi^2k_B^2}{3}g(\varepsilon_F)T=
\frac{\pi^2}{2}Nk_B\frac{T}{T_F}+O(T^3)\propto g(\varepsilon_F)}

\end{align}
$$

- 泡利顺磁性

	- 

$$
\begin{align} 1.&经典电子气：磁场B沿z方向，电子有两个自旋态，设各电子自旋不相互作用
\\&若施加磁场引起磁矩同向排列，则称该系统显示顺磁性.大多数顺磁体\chi\ll1
\\$&对N个粒子集合，Z_N=Z_1^N=(e^{\beta\mu_BB}+e^{-\beta\mu_BB})^N=-Nk_BT\ln[2\cosh(\beta\mu_BB)]
\\$&根据dU=TdS-mdB,总磁矩：m=-\bigg(  \frac{\partial F}{\partial B}\bigg)_T=N\mu_B\tanh(\beta\mu_BB)

\\&在T很大或B很小时，x\ll1,\tanh x\approx x,m=0,磁矩一半向上，一半向下。

\\$&弱磁材料(顺磁体):\chi\ll 1,B=\mu_0(H+M)\approx \mu_0(1+\chi)H\approx\frac{\mu_0 M}{\chi}
\\&[居里定律]M=\frac{m}{V}=\frac{N\mu_B}{V}\tanh(\beta\mu_BB)\approx \frac{N\mu_B ^2B}{Vk_BT},则\chi\approx \frac{N\mu_B ^2\mu_0}{Vk_BT}\propto \frac{1}{T}
\\\\2.&现代金属电子气：在T很小(T\ll T_F)的情况下，简单金属磁化率近似为常数
\\&外磁场B将态密度曲线正反平行磁矩部分沿能量各自平移\mu_BB
\\&对磁矩与外场相反的电子，能量较高的电子将磁矩翻转，填到磁矩同向的空态
\\&直到体系平衡，两种磁矩的电子达到相同的化学势，电子达到最大能量费米能
\\&发生磁矩反转的电子数：\frac{1}{2}\mu_B B g(\varepsilon_F),每个电子沿磁场方向增加2\mu_B磁矩
\\&产生总磁矩M=\mu^2_Bg(\varepsilon_F)B,泡利顺磁磁化率\chi=\frac{\mu_0M}{B}=\mu_0\mu_B^2g(\varepsilon_F)\propto g(\varepsilon_F)
\\&
\end{align}
$$

## 弛豫时间近似与准经典模型

### 准经典模型

- 外场作用下自由电子遵循外加电场含时薛定谔方程，根据量子力学与经典对应的Ehrenfest定理，只有粒子动能较大，外场变化缓慢时，过渡到经典情形。

此时方程取波包解。波包中心坐标和动量期待值变化满足经典运动方程，但需要满足不确定原理。
- 

$$
\begin{align} &金属中电子动量典型值为\hbar k_F，确定动量要求\Delta p\ll \hbar k_F,又k_F\sim n^{1/3}\sim\frac{1}{r_s},
\\&金属中r_s为电子平均占据球半径，与离子实间距数量级相同
\\&不确定原理：\Delta x\approx\frac{\hbar}{\Delta p}\gg\frac{1}{k_F}\approx r_s，坐标不确定度应满足多个离子实间距
\\&实际电子平均自由程l和外场变化尺度波长\lambda远大于r_s,故电子行为可经典方式描述
\\&经典模型电子速度取平均热运动速度:v_{th}^2\approx\frac{k_BT}{m}，费米统计下v_F^2\approx \frac{2\varepsilon_F}{m}
\\&准经典模型：外场作用下电子，使用经典处理，取费米速度为平均速度

\end{align}
$$

### 金属自由电子气体的输运过程

- 电子动力学方程

	- 

$$
\begin{align} &时刻t电子平均动量p(t),dt后电子未被碰撞概率1-\frac{dt}{\tau}
\\&时刻t+dt平均动量p(t+dt)=(1-\frac{dt}{\tau})[p(t)+F(t)dt]
\\&一阶近似：p(t+dt)-p(t)=F(t)dt-p(t)\frac{dt}{\tau}
\\&即自由电子在外场下动力学方程：\frac{d\boldsymbol p(t)}{dt}=\boldsymbol F(t)-\frac{\boldsymbol p(t)}{\tau}
\\&即引入依赖速度的阻尼项：m\frac{d\boldsymbol v(t)}{dt}=\boldsymbol F(t)-m\frac{\boldsymbol v(t)}{\tau}

\end{align}
$$

- 电导率

	- 

$$
\begin{align} 1.&恒定电场稳态情形：\boldsymbol E=-e\boldsymbol E,电子以恒定速度运动，即漂移速度：v_d=-\frac{e\tau\boldsymbol E }{m}
\\&电流密度：\boldsymbol J=-ne\boldsymbol v_d=\frac{ne^2\tau}{m}\boldsymbol E=\sigma \boldsymbol E,电导率\sigma=\frac{ne^2\tau}{m},平均自由程l=v_d\tau
\\&漂移速度对应费米球波矢k：\hbar\Delta \boldsymbol k=-e\boldsymbol E\tau,电子气中所有电子在k空间平移\Delta \boldsymbol k
\\&一般\Delta \boldsymbol k\ll \boldsymbol k_F，即费米球在\varepsilon_F附近微小扰动
\\2.&交变电场情形(电子受电场空间平均作用)\boldsymbol E=\boldsymbol E_0e^{-i\omega t},\boldsymbol v=\boldsymbol v_0e^{-i\omega t},\boldsymbol v_d=\frac{-e\boldsymbol E}{m(1-i\omega\tau)},
\\&\sigma=\frac{ne^2\tau}{m}\frac{1}{1-i\omega\tau}=\frac{\sigma_0}{1+(\omega\tau)^2}+i\frac{\sigma_0\omega\tau}{1+(\omega\tau)^2}


\end{align}
$$

- 霍尔效应、磁阻

	- 

$$
\begin{align} &自由电子在外场下动力学方程：\frac{d\boldsymbol p(t)}{dt}=-e(\boldsymbol E+\boldsymbol{v\times B})-\frac{\boldsymbol p(t)}{\tau},
\\&磁场z方向，电场xz平面，稳态\frac{d\boldsymbol p(t)}{dt}=0，\boldsymbol J=-ne\boldsymbol v
\\&分量式：\sigma_0E_x=J_x+\omega_c \tau J_y,\sigma_0E_y=J_y-\omega_c \tau J_x,回旋频率\omega_c=\frac{eB}{m},直流电导率\sigma_0=\frac{ne^2\tau}{m}
\\&J_y=0时存在霍尔电场E_y=-\frac{\omega_c\tau}{\sigma_0}J_x=-\frac{B}{ne}J_x，
\\&霍尔系数R_H=\frac{E_y}{J_xB_z}=-\frac{1}{ne}，只依赖于自由电子气体密度，实际与实验值相差很大

\\&横向磁阻：与电流方向垂直的磁场作用下，电流方向电阻的变化，此处即电阻率的变化，实际不为0
\\&z方向速度非零时，电子螺旋前进，投影为圆，角频率\omega_c


\end{align}
$$

- 热导率

	- 

$$
\begin{align} &魏德曼-弗兰兹定律：给定温度下，金属热导率和电导率比值为常数。
\\&洛伦兹发现洛伦兹数L=\frac{\kappa}{\sigma T}与温度无关
\\&\kappa=\frac{1}{3}C_Vv^2\tau=\frac{\pi^2k_B^2 n\tau}{3m}T,\frac{\kappa}{\sigma T}=\frac{1}{3}(\frac{\pi k_B^2}{e})^2
\\&实际以上结论有问题

\end{align}
$$

### 金属电子气体光学性质

- 

$$
\begin{align} &考虑交变电场时空变化：\boldsymbol J(\boldsymbol r,\omega)=\sigma(\omega)\boldsymbol E(\boldsymbol r,\omega),
\\&要求低频电场\lambda\gg l，此时到达r处电子感受到的仍为同一时刻电场,且忽略磁场洛伦兹力
\\&对于更高频率电磁场，不满足同时刻电场相同，需要采用非局域理论
\\&材料性质：介电常数和磁导率，光学性质描述：消光系数、折射率、反射率
\\&\sigma=\frac{ne^2\tau}{m}\frac{1}{1-i\omega\tau}=\frac{\sigma_0}{1+(\omega\tau)^2}+i\frac{\sigma_0\omega\tau}{1+(\omega\tau)^2}

\\&由麦克斯韦方程组导出自由电子气体中的波动方程\nabla^2\boldsymbol E-\mu_0\sigma\frac{\partial \boldsymbol E}{\partial t}-\varepsilon_0\mu_0\frac{\partial^2 \boldsymbol E}{\partial t^2}=0
\\&对于单色波解\boldsymbol E=\boldsymbol E_0e^{i(\boldsymbol {k\cdot r}-\omega t)},方程给出k^2=\varepsilon_0\mu_0\omega^2+i\mu_0\sigma\omega=\mu_0\omega^2(\varepsilon_0+i\frac{\sigma}{\omega})=\mu_0\omega^2\varepsilon
\\&引入等离子体频率\omega_p^2=\frac{ne^2}{\varepsilon_0 m},描述自由电子气体整体相对于正电荷背景集体运动频率
\\&根据复数介电系数计算，金属自由电子气体对光学响应分为吸收区、反射区与透明区
\\&[等离子体振荡]位移电子受电场作用运动方程解为纵向电荷密度振荡，类似电离气体

\end{align}
$$

## 自由电子气体模型的局限性

