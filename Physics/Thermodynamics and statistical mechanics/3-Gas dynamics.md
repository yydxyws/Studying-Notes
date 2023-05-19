# 气体动力学

## 麦克斯韦-玻尔兹曼分布

### 麦克斯韦分布

- 单位体积内v附近运动分子数：nf(v)dv，n为单位体积分子总数

$$
\begin{align} &E_\alpha=\frac{1}{2}mv_x^2，\int_{-\infty}^{\infty}e^{-mv_x^2/2k_BT}dv_x=\sqrt \frac{2\pi k_BT}{m}

\\& 速度分布函数
g(v_x)=\sqrt {\frac{m}{2\pi k_BT}} e^{-mv_x^2/2k_BT}
\\&d\Omega=4\pi v^2dv，f(v)dv\propto v^2dv e^{-mv^2/2k_BT},
\\&\int_{-\infty}^{\infty}v^2e^{-mv^2/2k_BT}dv=\frac{1}{4}\sqrt \frac{\pi }{(m/2k_BT)^3}
\\&速率分布函数：f(v)dv=\frac{4}{\sqrt \pi}\bigg(\frac{m}{2k_BT}\bigg)^{3/2}v^2 e^{-mv^2/2k_BT}dv
\\&以上为[麦克斯韦分布]

\end{align}
$$
- 

$$
\begin{align} &平均速率：v_{s}=\sqrt{\frac{8k_BT}{\pi m}}
\\&最概然速率：v_{max}=\sqrt{\frac{2k_BT}{m}}
\\&方均根速率：v_{rms}=\sqrt{\frac{3k_BT}{m}}
\end{align}
$$

### 压强

- 

$$
\begin{align} &立体角定义：\Omega=\frac{A}{r^2}，A为张角对应球面积，整个球面\Omega=4\pi
\\&\theta\sim\theta+d\theta环形区域面积:d \Omega=2\pi\sin\theta d\theta，立体角元\frac{d \Omega}{4\pi}
\\&以速度v附近，任意方向\theta附近角度运动的单位体积分子数：nf(v)dv\frac{1}{2}\sin\theta d\theta
\\&单位时间\theta方向撞击单位面积器壁扫出体积：vdt\cos\theta
\\&假设均为弹性碰撞，每个分子撞击器壁动量改变量2mv\cos\theta
\\&【压强】p=\int dN p_s=\int_{0}^{\infty}\int_{0}^{\pi/2}(2mv\cos\theta)(vdt\cos\theta\cdot nf(v)dv\frac{1}{2}\sin\theta d\theta)=\frac{1}{3}nm\langle v^2\rangle
\\&改写得到pV=Nk_BT(理想气体方程)，R=N_Ak_B为气体常量
\\&动能密度u=\frac{1}{3}nm\langle v^2\rangle，p=\frac{2}{3}u

\end{align}
$$
- 

$$
\begin{align} &气体从极小孔中逃逸：dN=vdt\cos\theta\cdot nf(v)dv\frac{1}{2}\sin\theta d\theta，分子通量\Phi=\int_{0}^{\infty}\int_{0}^{\pi/2}dN=\frac{1}{4}n\langle v\rangle
\\&对理想气体：\Phi=\frac{1}{4}n\langle v\rangle=\frac{1}{4}\frac{p}{k_BT}\sqrt\frac{8k_BT}{\pi m}=\frac{p}{\sqrt{2\pi mk_BT}}\propto\frac{1}{\sqrt{m}}[格拉姆泻流定律]
\\&泻流气体中的分子具有更高能量，其分布函数\propto v^3 e^{-mv^2/2k_BT}。这要求泻流孔直径D\ll \lambda(平均自由程)
\\&泻流分子通量平衡时，有克努森效应：\frac{p_1}{\sqrt{T_1}}=\frac{p_2}{\sqrt{T_2}}
\\&可用分子通量推导低压气体顺管道流下速率（克努森流动）
\end{align}
$$

### 平均自由程

- 

$$
\begin{align} &气体中大角度散射为主导输运过程，能量、温度无关，故可以使用碰撞刚球模型
\\&平均碰撞时间：\tau=\int_{0}^{\infty}t\cdot P(t)= \int_{0}^{\infty}t\cdot( e^{-n\sigma vt}n\sigma vdt)=\frac{1}{n\sigma v},\sigma为单个分子碰撞截面
\\&根据硬球势定义碰撞截面\sigma=\pi(a_1+a_2)^2=\pi d^2,(温度较低同时能忽略量子效应)
\\&平均自由程\lambda=\langle v_r\rangle\approx \frac{1}{\sqrt 2n\sigma},相对平均速度\langle v_r^2\rangle=\langle v_1^2\rangle+\langle v_2^2\rangle-\langle v_1v_2\rangle=2\langle v^2\rangle
\end{align}
$$

## 输运与热扩散

### 气体输运性质

- 黏性-输运动量
viscosity

	- 

$$
\begin{align} &黏性：流体对剪切力产生形变抵抗程度量度
\\&对平直、平行和均匀的流动，层间剪应力正比于垂直于层方向速度梯度，这种流体为牛顿流体。
\\&其比例系数为黏性系数（黏度）\eta:\tau_{xz}=\frac{F}{A}=\eta\frac{d\langle u_x(z)\rangle}{dz},
\\&剪应力\tau_{xz}是每秒每平方米输运横向动量，等于动量通量\Pi_z=-\eta\frac{\partial \langle u_x(z)\rangle}{\partial z}
\\&动理学理论计算动量通量：\Pi_z= \int \!_{\Delta_\lambda } p_x dN
\\&\quad=\int_{0}^{\infty}\int_{0}^{\pi}\big(vdt\cos\theta\cdot nf(v)dv\frac{1}{2}\sin\theta d\theta\big)\big(
-m\lambda\cos\theta\frac{\partial \langle u_x(z)\rangle}{\partial z}\big)=-\frac{1}{3}nm\lambda \langle v\rangle\frac{\partial \langle u_x(z)\rangle}{\partial z}
\\&则黏性系数为\eta=\frac{1}{3}nm\lambda \langle v\rangle=\frac{1}{3}nm \cdot\frac{1}{\sqrt 2n(\pi d^2)} \cdot\sqrt{\frac{8k_BT}{\pi m}}=\frac{2}{3\pi d^2}\bigg( \frac{mk_BT}{\pi} \bigg)^{1/2}\propto \frac{\sqrt m}{d^2}\sqrt T
\\&黏性系数与压强无关，温度升高黏性增大，
\\&以上需要近似：容器大小L \gg平均自由程\lambda \gg分子直径d，实现单粒子碰撞和分子间碰撞为主
\\&

\end{align}
$$

- 热传导-输运热量
thermal conductivity

	- 

$$
\begin{align} &热量抵抗温度梯度流动,用热通量\boldsymbol J描述热流:J_z=-\kappa \big( \frac{\partial T}{\partial z} \big),\boldsymbol J=-\kappa\nabla T,材料的热导率\kappa 
\\&单位时间过单位面积输运热能J_z= \int C_{分子}{\Delta T}dN\\&
\quad=\int_{0}^{\infty}\int_{0}^{\pi}\big(vdt\cos\theta\cdot nf(v)dv\frac{1}{2}\sin\theta d\theta\big)\big(
-C_{分子}\lambda\cos\theta\frac{\partial T}{\partial z}\big)=-\frac{1}{3}nC_{分子}\lambda \langle v\rangle\frac{\partial T}{\partial z}
\\&\qquad \kappa=-\frac{1}{3}C_V\lambda \langle v\rangle，\frac{\kappa}{\eta}=\frac{C_{分子}}{m}

\end{align}
$$
	- 热扩散方程

		- 

$$
\begin{align} &热传导公式\boldsymbol J=-\kappa\nabla T\Rightarrow 热扩散方程\frac{\partial T}{\partial t} =D\nabla^2 T,D=\frac{\kappa}{C}为热扩散率


\end{align}
$$

	- 对流
	- 辐射

- 扩散-粒子的输运

	- 

$$
\begin{align} &平行于Z轴的单位体积中标记分子数n^*(z)的分子通量\Phi_z=-D \big( \frac{\partial n^*}{\partial z} \big),D是材料自扩散系数
\\&由于分子数守恒，\frac{\partial}{\partial t} 
(n^*Sdz)=- S\frac{\partial \Psi_z}{\partial z} dz,得到扩散方程：\frac{\partial n^*}{\partial t} =D\frac{\partial^2 n^*}{\partial z^2}
\\&对三维：\int_S\boldsymbol\Phi\cdot d\boldsymbol S=-\frac{\partial}{\partial t}\int_V n^*dV,得到扩散方程：\frac{\partial n^*}{\partial t} =D\nabla^2 n^*
\\&同理，\Psi_z=\int_{0}^{\infty}\int_{0}^{\pi}\big(vdt\cos\theta\cdot nf(v)dv\frac{1}{2}\sin\theta d\theta\big)\big(
-\lambda\cos\theta\frac{\partial n^*}{\partial z}\big)=-\frac{1}{3}\lambda \langle v\rangle\frac{\partial n^*}{\partial z}，D=\frac{1}{3}\lambda \langle v\rangle
\\&\quad D\propto \frac{1}{p},D\propto T^{3/2},D\propto \frac{1}{\sqrt m d^2},D=\rho\eta
\end{align}
$$

