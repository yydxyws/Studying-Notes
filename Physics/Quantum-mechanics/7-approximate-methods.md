# 微扰论与量子跃迁

## 定态微扰理论

### 微扰理论

- 根据无微扰情况下精确解求出有微扰的近似解（非简并情况）

$$
\begin{align} &施加微扰的哈密顿量(0表示非微扰量,\lambda为小量,可取1):H=H^0+\lambda H'
\\&此时定态情况有新的本征函数和本征值：H\psi_n=E_n\psi_n
\\&利用\lambda的幂级数展开(上标表示n级修正)
\begin{cases}
\psi_n=\psi_n^0+\lambda\psi_n^1+\lambda^2\psi_n^2+\dots\\
E_n=E_n^0+\lambda E_n^1+\lambda^2 E_n^2+\dots
\end{cases}，

\\&(级数展开的唯一性保证了相同幂次系数相等)
\\&带入定态方程得到(H^0+\lambda H')[\psi_n^0+\lambda\psi_n^1+\lambda^2\psi_n^2+\dots]\\&=(E_n^0+\lambda E_n^1+\lambda^2 E_n^2+\dots)[\psi_n^0+\lambda\psi_n^1+\lambda^2\psi_n^2+\dots]
\\&H^0\psi_n^0+\lambda(H^0\psi_n^1+H'\psi_n^0)+\lambda^2(H^0\psi_n^2+H'\psi_n^1)+\dots\\&=E_n^0\psi_n^0+\lambda(E_n^0\psi_n^1+E_n^1\psi_n^0)+\lambda^2(E_n^0\psi_n^2+E_n^1\psi_n^1+E_n^2\psi_n^0)+\dots
\\&零级项\lambda^0:H^0\psi_n^0=E_n^0\psi_n^0,\\&一级项:H^0\psi_n^1+H'\psi_n^0=E_n^0\psi_n^1+E_n^1\psi_n^0,\\&二级项:H^0\psi_n^2+H'\psi_n^1=E_n^0\psi_n^2+E_n^1\psi_n^1+E_n^2\psi_n^0

\end{align}
$$

### 非简并微扰理论

- 一级微扰近似理论

	- 

$$
\begin{align} &将\psi_n^0与一级项做内积:\langle \psi_n^0| H^0\psi_n^1\rangle+\langle \psi_n^0|H'\psi_n^0 \rangle=E_n^0\langle \psi_n^0|\psi_n^1 \rangle+E_n^1\langle \psi_n^0|\psi_n^0 \rangle
\\&利用厄米算符性质有：\langle \psi_n^0| H^0\psi_n^1\rangle=\langle H^0\psi_n^0|\psi_n^1 \rangle=E_n^0\langle \psi_n^0|\psi_n^1 \rangle,又\langle \psi_n^0|\psi_m^0 \rangle=\delta_{mn}
\\&则能量的一级修正就是微扰项在无微扰态的期待值：\boldsymbol{E_n^1=\langle \psi_n^0|H'|\psi_n^0 \rangle}

\\&一级项写为：(H^0-E_n^0)\psi_n^1=-(H'-E_n^1)\psi_n^0,且波函数\psi_n^0是完备的
\\&则\psi_n^1=\sum_{m\ne n}c_m^{(n)}\psi_m^0，代入一级项：\sum_{m\ne n}(E_m^0-E_n^0)c_m^{(n)}\psi_m^0=-(H'-E_n^1)\psi_n^0

\\&(任何\psi_n^0分量都可以并入首项去除，因为对任意\alpha,都有(\psi_n^1+\alpha\psi_n^0)满足修正方程)
\\&用\psi_l^0做内积:\sum_{m\ne n}(E_m^0-E_n^0)c_m^{(n)}\langle \psi_l^0|\psi_m^0\rangle=-\langle \psi_l^0|H'|\psi_n^0\rangle+E_n^1\langle \psi_l^0|\psi_n^0\rangle
\\&\begin{cases}
l=n,&E_n^1=\langle \psi_n^0|H'|\psi_n^0 \rangle\\
l\ne n,& (E_{l(m)}^0-E_n^0)c_{l(m)}^{(n)}=-\langle \psi_l^0|H'|\psi_n^0 \rangle,
\end{cases}即c_m^{(n)}=\frac{\langle \psi_l^0|H'|\psi_n^0 \rangle}{E_n^0-E_m^0}
\\&则波函数的一级修正：\boldsymbol{\psi_n^1=\sum_{m\ne n}\frac{\langle \psi_l^0|H'|\psi_n^0 \rangle}{E_n^0-E_m^0}\psi_m^0}(无微扰能级是非简并的)
\\&一级微扰理论对能量修正值较精确，对波函数则不然

\end{align}
$$

- 二级能量修正

	- 

$$
\begin{align} &将\psi_n^0与二级项做内积:


\langle \psi_n^0| H^0\psi_n^2\rangle+\langle \psi_n^0|H'\psi_n^0 \rangle=E_n^0\langle \psi_n^0|\psi_n^2 \rangle+E_n^1\langle \psi_n^0|\psi_n^1 \rangle+E_n^2\langle \psi_n^0|\psi_n^0 \rangle
\\&利用厄米算符性质有：\langle \psi_n^0| H^0\psi_n^2\rangle=\langle H^0\psi_n^0|\psi_n^2 \rangle=E_n^0\langle \psi_n^0|\psi_n^2 \rangle,又\langle \psi_n^0|\psi_m^0 \rangle=\delta_{mn}
\\&则E_n^2=\langle \psi_n^0|H'|\psi_n^0 \rangle-E_n^1\langle \psi_n^0|\psi_n^1\rangle=\langle \psi_n^0|H'|\psi_n^0 \rangle-E_n^1\sum_{m\ne n}c_m^{(n)}\langle \psi_n^0|\psi_m^0\rangle
\\&\quad=\langle \psi_n^0|H'|\psi_n^0 \rangle=\sum_{m\ne n}c_m^{(n)}\langle \psi_n^0|H'|\psi_m^0\rangle
=\sum_{m\ne n}\frac{\langle \psi_m^0|H'|\psi_n^0 \rangle \langle \psi_n^0|H'|\psi_m^0 \rangle}{E_n^0-E_m^0}

\\&能量的二级近似：\boldsymbol {E_n^2=\sum_{m\ne n}\frac{|\langle \psi_m^0|H'|\psi_n^0 \rangle |^2}{E_n^0-E_m^0}}
\\&令V_{mm}=\langle \psi_m^0|H'|\psi_n^0 \rangle,\Delta_{mn}=E_m^0-E_n^0,
\\&则E_n^1=V_{nn},E_n^2=\sum_{m\ne n}\frac{|V_{nm}|^2}{\Delta_{nm}},E_n^3=\sum_{l,m\ne n}\frac{V_{nl}V_{lm}V_{mn}}{\Delta_{nl}\Delta_{nm}}-\sum_{m\ne n}\frac{|V_{nm}|^2}{\Delta_{nm}^2}


\end{align}
$$

- 弱电场中的带电谐振子

### 简并微扰理论

- 二重简并

	- 

$$
\begin{align} &假设H^0\psi_a^0=E^0\psi_a^0，H^0\psi_b^0=E^0\psi_b^0，\langle \psi_a^0|\psi_b^0 \rangle=0
\\&\psi^0=\alpha \psi_a^0+\beta\psi_b^0依然是H^0本征态,且值为E^0,H^0\psi^0=E^0\psi^0


\\&施加微扰将打破简并态：从0到1增大\lambda，简并能级一般分裂为两个能级
\\&移除微扰，上下能态均变为\psi_a^0和\psi_b^0的线性组合，且二者相互正交

\end{align}
$$
	- 

$$
\begin{align} 
&为得到好的线性组合\psi_a^0和\psi_a^0, 求解H\psi=E\psi,H=H^0+\lambda H'
\\&使用\lambda的幂级数展开
\begin{cases}
\psi=\psi^0+\lambda\psi^1+\lambda^2\psi^2+\dots\\
E=E^0+\lambda E^1+\lambda^2 E^2+\dots
\end{cases}，

\\&H^0\psi^0+\lambda(H'^0\psi^0+H^0\psi^1)+\dots=E^0\psi^0+\lambda(E^1\psi^0+E^0\psi^1)+\dots
\\&使用\psi_a^0做内积:\langle \psi_a^0| H^0\psi^1\rangle+\langle \psi_a^0|H'\psi^0 \rangle=E^0\langle \psi_a^0|\psi^1 \rangle+E^1\langle \psi_a^0|\psi^0 \rangle
\\&利用厄米性质得:\langle \psi_a^0|H'\psi^0 \rangle=E^1\langle \psi_a^0|\psi^0 \rangle
\\&代入\psi^0=\alpha \psi_a^0+\beta\psi_b^0得：\alpha\langle \psi_a^0|H'|\psi_a^0 \rangle+\beta\langle \psi_a^0|H'|\psi_b^0 \rangle=\alpha E^1
\\&令W_{ij}=\langle \psi_i^0|H'|\psi_j^0 \rangle，有\begin{cases}
\alpha W_{aa}+\beta W_{ab}=\alpha E^1\\
\alpha W_{ba}+\beta W_{bb}=\beta E^1
\end{cases}
\\&W是H'关于无微扰的波函数\psi_a^0和\psi_b^0的矩阵元，理论已知
\\&解线性方程组得到\alpha[W_{ab}-W_{ba}-(E^1-W_{aa})(E^1-W_{bb})]=0
\\&\alpha\ne 0 时,注意到W_{ab}=W_{ba}^*,解得两个受到扰动的能量：
\\&\boldsymbol{E^1_\pm=\frac{1}{2}[W_{aa}+W_{bb}\pm\sqrt{(W_{aa}+W_{bb})^2+4|W_{ab}|^2}]}
\\&\alpha=0时,有\beta=1,W_{ab}=0,E^1=W_{bb}
\\&可以得到好的线性组合：\begin{cases}
E^1_+=W_{aa}=\langle \psi_a^0|H'|\psi_a^0 \rangle
\\E^1_-=W_{bb}=\langle \psi_b^0|H'|\psi_b^0 \rangle
\end{cases}

\end{align}
$$
	- 

$$
\begin{align} &【定理】设厄米算符A满足[A,H^0]=0,[A,H']=0
\\&H^0简并本征函数\psi_a^0和\psi_b^0，也是A的本征函数\begin{cases}
A\psi_a^0=\mu\psi_a^0\\
A\psi_b^0=\nu\psi_b^0\\
\nu\ne\mu
\end{cases}
\\&则W_{ab}=0,\psi_a^0和\psi_b^0是好的本征函数

\end{align}
$$

- 多重简并

	- 

$$
\begin{align} &二重简并:\left [ \begin{matrix}
W_{aa}& W_{ab} \\
W_{ba}& W_{bb} \\
\end{matrix} \right ]
\left [ \begin{matrix}
\alpha \\
\beta \\
\end{matrix} \right ]=E^1
\left [ \begin{matrix}
\alpha \\
\beta \\
\end{matrix} \right ],
\\&所有E^1值都是W矩阵本征值,好的无微扰态线性组合就是W的本征矢量
\\&n重简并：找到n\times n矩阵W_{ij}=\langle \psi_i^0|H'|\psi_j^0 \rangle的本征值
\\&寻找好的零级近似波函数：在简并子空间寻找一组基使矩阵W对角化
\end{align}
$$
	- 子主题 2

$$
\begin{align} &假设E_n^{(0)}是k度简并.零级近似波函数\psi_n^{(0)}写成k个\phi_i的线性组合\ket{\psi_n^{0}}=\sum_{i=1}^kc_i^{(0)}\ket{\phi_i}
\\&代入7.2式
(H_0-E^{0})\ket{\psi^{(1)}}=(E^{(1)}-H')\sum_{i=1}^kc_i^{(0)}\ket{\phi_i}
\\&左乘\bra{\phi_l}得，0=E^{(1)}\sum_i^kc_i\delta_{il}-\braket{\phi_l|H'|\phi_i}\sum_i^kc_i \eqno 7.3
\\&上式是系数c_i^{(0)}为未知量的一次齐次方程组.
久期方程：det|H'_{li}-E_n^{(1)}\delta_{li}|=0

\\&解此方程可得能量的一级修正E_n^{(1)}的k个根.因此E_n=E_n^{(0)}+E_n^{(1)},
\\&若E_n^{(1)}的k个根都不相等，则一级微扰可以将k度简并完全消除；
\\&若E_n^{(1)}有几个重根，说明能级简并未完全解除.\\&须考虑能量的二级修正，才有可能使能级完全裂开.

\end{align}
$$

- 对称谐振子高阶修正
- 非谐振子
- 弱电场中的电偶极矩与对称破缺

### 好的量子数

- 一个好量子数代表着对应的算符与哈密顿量对易，也就是该物理量守恒。利用好量子数可以使哈密顿量的矩阵准对角化从而大大简化计算工作量。
- 群论角度：如果有好量子数存在，说明对应的群是可约的，也就是说系统存在一定的对称性，然后可以通过幺正变换，变成块对角的矩阵。而好量子数对应系统的一个不可约表示。
- 只有当算符作用在它的本征态上时，这个操作才有好的定义，即从定义这个状态的状态量中直接提取数字，或者叫好量子数，而不改变状态本身。

不是本征态，就是非绝热的散射，操作起来相当不可控，不符合现代量子力学要求可控测量的核心思想。

从这个意义上讲，算符本身也是状态。就像量子计算里面把算符叫做稳定子（stabilizer），直接当成状态使用，而不需要让狄拉克矢量再显式地出现。现代的密度矩阵重整化群（DMRG），也基本都改用矩阵乘积算符（MPO）或者张量网络来表达，状态矢量确实不怎么需要考虑了。状态，已经与测量高度关联起来。联接它们的，正是好量子数。

## 原子物理的
量子理论

### 氢原子精细结构

- 相对论修正

	- 

$$
\begin{align} &相对论质量:m=\frac{m_0}{\sqrt{1-(\frac{v}{c})^2}}，动量：p=\frac{m_0v}{\sqrt{1-(\frac{v}{c})^2}},动能：T=\frac{m_0}{\sqrt{1-(\frac{v}{c})^2}}c^2-m_0c^2
\\&由于T=\sqrt{p^2c^2+m_0^2c^4}-m_0c^2=m_0c^2\big[\sqrt{1+(\frac{p}{m_0c})^2}-1\big]=m_0c^2\big[1+\frac{1}{2}(\frac{p}{m_0c})^2-\frac{1}{8}(\frac{p}{m_0c})^4+\dots\big]
\\&\qquad =\frac{p^2}{2m}-\frac{p^4}{8m_0^3c^2}+\dots,氢原子基本是非相对论的，动能项取二阶近似展开,哈密顿微扰量H'_r=-\frac{p^4}{8m_0^3c^2}
\\&一级近似微扰能量E_r=\langle H'_r \rangle=-\frac{1}{8m_0^3c^2}\langle \psi|p^4 \psi \rangle=-\frac{1}{8m_0^3c^2}\langle p^2\psi|p^2 \psi \rangle
\\&【注意】上式利用了l\ne0时p^2和(E-V)的厄米性。对l=0，p^4不是厄米算符，微扰存在问题
\\&\qquad但是l=0存在严格解，可以用相对论的狄拉克方程替代非相对论的薛定谔方程求解
\\&无微扰态薛定谔方程:p^2\psi=2m(E-V)\psi,则E_r^1=-\frac{1}{2mc^2}\langle (E-V)^2 \rangle=-\frac{1}{2mc^2}\big[E^2-2E\langle V\rangle+\langle V^2\rangle
 \big]
\\&对于氢原子，V(r)=-\frac{1}{4\pi\varepsilon_0}\frac{e^2}{r},利用无微扰下\psi_{nlm}计算得到\langle \frac{1}{r}\rangle=\frac{1}{n^2a}，\langle \frac{1}{r^2}\rangle=\frac{1}{(l+\frac{1}{2})n^3a^2}
\\&则E_r^1=-\frac{1}{2mc^2}\bigg[E_n^2+2E_n(\frac{e^2}{4\pi\varepsilon_0})\frac{1}{n^2a}+(\frac{e^2}{4\pi\varepsilon_0})^2\frac{1}{(l+\frac{1}{2})n^3a^2}\bigg]=-\frac{(E_n)^2}{2mc^2}\bigg[\frac{4n}{l+\frac{1}{2}}-3\bigg]
\\&【说明】氢原子的微扰是球对称的，和L^2,L_z对易，且对给定E_n的n^2个态，算付的本征值都不同，
\\&\qquad并且波函数\psi_{nlm}是好的量子态，故可以使用非简并态微扰。


\end{align}
$$

- 自旋-轨道耦合

	- 

$$
\begin{align} &电子绕核运动，以电子为原点作坐标系，质子产生磁场作用于有自旋的电子

\\&质子磁场\boldsymbol B=\frac{\mu_0I}{2r},I=\frac{e}{T},L=rmv=\frac{2\pi mr^2}{T}\Rightarrow \boldsymbol B=\frac{1}{4\pi \varepsilon_0 }\frac{e}{mc^2r^3}\boldsymbol L
\\&电子磁偶极矩\boldsymbol \mu=\gamma\boldsymbol S=-\frac{e}{m}\boldsymbol S(电子旋磁比使用g因子进行量子修正)
\\&电子坐标系绕核子旋转，存在加速度，故引入\frac{q}{2}作动力学修正，即托马斯旋进
\\&哈密顿量描述：H_{so}'=-\boldsymbol \mu\cdot \boldsymbol B=\frac{e^2}{8\pi \varepsilon_0 }\frac{1}{m^2c^2r^3}\boldsymbol S\cdot \boldsymbol L
\\&此时哈密顿量不再与\boldsymbol L、\boldsymbol S对易，而是与\boldsymbol L^2,\boldsymbol S^2,和总角动量\boldsymbol J=\boldsymbol L+\boldsymbol S对易
\\&有L\cdot S=\frac{1}{2}(J^2-L^2-S^2)，本征值为\frac{\hbar^2}{2}[j(j+1)-l(l+1)-s(s+1)]
\\&同时\langle \frac{1}{r^3}\rangle=\frac{1}{l(l+\frac{1}{2})(l+1)n^3a^3},
\\&E_{so}^1=\frac{e^2}{8\pi \varepsilon_0 }\frac{1}{m^2c^2}\frac{\frac{\hbar^2}{2}[j(j+1)-l(l+1)-\frac{3}{4}]}{l(l+\frac{1}{2})(l+1)n^3a^3}=\frac{(E_n)^2}{mc^2}\frac{n[j(j+1)-l(l+1)-\frac{3}{4}]}{l(l+\frac{1}{2})(l+1)}


\end{align}
$$

		- 

$$
\begin{align} &磁偶极矩定义为电流与面积乘积：\mu=\frac{q\pi r^2}{T}

\\&对质量为m圆环，角动量为转动惯量与角速度乘积S=\frac{2\pi mr^2}{T}
\\&旋磁比\gamma=\frac{q}{2m}.复杂体系可以分割为小圆环叠加（比荷均匀）
\\&对于量子理论，电子磁矩为经典的2倍，偏差称为g因子：\mu=g(\frac{q}{2m})S


\end{align}
$$

- 精细结构

	- 

$$
\begin{align} &相对论修正和自选轨道耦合量级相同，合并得到完整的精细结构公式：
\\&E_{fs}^1=\frac{(E_n)^2}{2mc^2}\big(3-\frac{4n}{j+\frac{1}{2}}\big)
\\&考虑精细结构的氢原子能级公式：E_{nj}=-\frac{13.6eV}{n^2}\bigg[1+\frac{\alpha^2}{n^2}\bigg(\frac{n}{j+\frac{1}{2}}-\frac{3}{4}\bigg)\bigg]
\\&【说明】精细结构破坏了l的简并度，保留对j的简并度，m_l和m_s不再是好的量子数
\\&定态变为这些量的线性组合，好的量子数是n,l,s,j,m_j

\end{align}
$$

- 碱金属双线结构

### 塞曼效应与朗道能级

- 原子磁矩与塞曼效应

	- 塞曼效应：原子置于外磁场，能级发生改变。

将光源放在磁场内，光源发出的谱线分裂成几条，每条谱线光都是偏振光。谱线分裂表明能量差变化。电子发生跃迁前后的两个原子态总自旋为0，对应的谱线为单态谱线。原子结构中，在任何满轨道中的两个核外层电子，具有大小相等、方向相反的自旋，并彼此互相抵消，称为单态，以字母S表示。

正常塞曼效应：只有电子的数目为偶数，并且形成单态原子（自旋总数S=0）。相当于单态谱线在外磁场分裂为3条。

反常塞曼效应：相当于非单态谱线在外磁场中分裂。（自旋总数S≠0）

帕邢-贝克效应：若外磁场足够强，自旋与轨道耦合被破坏，自旋与轨道磁矩分别独立地与外磁场耦合，m_l,m_s对应的简并能级被外磁场消除。
	- 

$$
\begin{align} &塞曼效应的特性取决于内外磁场的相对强度
\\&\begin{cases}
内磁场：&质子对单电子产生磁场：\boldsymbol B_{int}=\frac{1}{4\pi\varepsilon_0}\frac{e}{mc^2r^3}\boldsymbol L\\
&内磁场导致的自旋轨道相互作用：H'_{so}=\frac{e^2}{8\pi\varepsilon_0}\frac{1}{m^2c^2r^3}\boldsymbol {S\cdot L}\\
外磁场：&B_{ext}为均匀外磁场，
\\&电子自旋偶极矩:\boldsymbol \mu_s=-\frac{e}{m}\boldsymbol S,电子轨道偶极矩:\boldsymbol \mu_l=-\frac{e}{2m}\boldsymbol L\\
&对单电子：H'_Z=-(\boldsymbol \mu_l+\boldsymbol \mu_s)\cdot \boldsymbol B_{ext}=\frac{e}{2m}(\boldsymbol L+2\boldsymbol S)\cdot \boldsymbol B_{ext}
\end{cases}


\\&\begin{cases}
B_{ext}\ll B_{int}&精细结构占主导作用，外场能级附加看做微扰\\
B_{ext}\gg B_{int}&塞曼效应占主导作用，精细结构看做微扰\\
B_{ext} B_{int}相近&应用简并微扰，哈密顿对角化
\end{cases}



\end{align}
$$

- 弱场塞曼效应

	- 原子物理观点

		- 

$$
\begin{align} &体系具有磁矩\vec\mu,在外磁场\vec B中有势能： U=-\vec \mu\cdot \vec B=-\mu_{J_z} B=m_Jg_J\mu_B B(\mu_z=-mg\mu_B)
\\&\mu_z为\vec \mu_J在z投影，m为角动量\vec J的z投影的量子数m_J,g为g_{J*},以下省略了角标J。

\\&无外磁场：两能级差h\nu =E_2-E_1,外加磁场B时：
    \begin{cases}
        E_2'=E_2+m_2g_2\mu_BB\\
        E_1'=E_1+m_1g_1\mu_BB
    \end{cases}
\\&每个能级裂为m个能级，即(2J+1)个能级及简并：
    h\nu'=h\nu+(m_2g_2-m_1g_1)\mu_B B
\\&电偶极矩的跃迁选择规则\begin{cases}
 \Delta m_J=0,\pm 1\\
\Delta l=\pm 1\\
\Delta J=0
\end{cases}
\Rightarrow
\begin{cases}
体系自旋为零时，g_1=g_2=1\\
    h\nu'=h\nu+(m_2-m_1)\mu_B B\end{cases}

\\&(适用于紫外线与可见光等波长远大于原子半径的光，对于X射线，需要考虑四极辐射)
\\&正常塞曼效应:分裂为三条间隔相等的谱线：
    h\nu'=h\nu+\begin{pmatrix}\mu_B B\\0\\-\mu_B B
    \end{pmatrix},
\\&\Rightarrow 
\begin{cases}
\Delta \varepsilon=\mu_BB=\frac{e\hbar}{2m_e}B\\
\Delta\tilde\nu=(m_2g_2-m_1g_1)\Delta \tilde\nu_L
\end{cases}
\Rightarrow \nu'=\nu+\begin{pmatrix}\frac{e}{4\pi m_e}B \\ 0 \\-\frac{e}{4\pi m_e}B \end{pmatrix},洛伦兹单位:\frac{e}{4\pi m_e}B
\end{align}
$$

	- 朗德g因子

		- 

$$
\begin{align} &
朗德g因子：g=\frac{测量到的\mu_z，以\mu_B为单位}{角动量在z方向投影，以\hbar为单位}\\&
g_J=1+\frac{J(J+1)-L(L+1)+S(S+1)}{2J(J+1)}=1+\frac{J(J+1)-L(L+1)+\frac{3}{4}}{2J(J+1)}\\&
从图可知，合成总磁矩\boldsymbol \mu不在总角动量\boldsymbol  j延长线上，但所有矢量绕\boldsymbol j旋进\\&
\boldsymbol \mu分解为沿\boldsymbol j的\boldsymbol \mu_j 和垂直\boldsymbol j的分量，绕\boldsymbol j 转动，对外平均为\boldsymbol 0，认为\boldsymbol \mu_j为总磁矩
\\&\mu_j=\mu_l\cos(\boldsymbol l,\boldsymbol j)+\mu_s\cos(\boldsymbol s,\boldsymbol j)=(-g_l l^*\mu_B)\frac{j^{2*}+l^{2*}-s^{2*}}{2j^*l^*}+(-g_s s^*\mu_B)\frac{j^{2*}+s^{2*}-l^{2*}}{2j^*s^*}
\\&\begin{cases}
j^*=\sqrt{j(j+1)}\\
l^*=\sqrt{l(l+1)}
\\s^*=\sqrt{s(s+1)}
\end{cases}且\mu_j=-g_jj^*\mu_B\Rightarrow 
\begin{cases}
g_j&=\frac{g_l+g_s}{2}+(\frac{g_l-g_s}{2})(\frac{l^{2*}-s^{2*}}{j^{2*}})\\
&=\frac{3}{2}+\frac{1}{2}(\frac{s^{2*}-l^{2*}}{j^{2*}})\\
\end{cases}
\\&前提：s与l能够耦合成j（外磁场不足以破坏s-l耦合），且只考虑单个电子

\end{align}
$$

			- 

	- 微扰理论观点

		- 

$$
\begin{align} &弱场，精细结构主导，对氢原子，好量子数n,l,j,m_j
\\&塞曼效应对能量一级修正：E_Z^1=\Braket{nljm_j|H_Z'|nljm_j}=\frac{e}{2m}\boldsymbol B_{ext}\cdot\Braket{\boldsymbol{L+2S}}
\\&总角动量\boldsymbol{J=L+S}为定值方向固定，\boldsymbol S的平均值是沿\boldsymbol J的投影：\boldsymbol S_{ave}=\frac{\boldsymbol{S\cdot J}}{J^2}\boldsymbol J
\\&\boldsymbol {S\cdot J}=\frac{1}{2}(J^2+S^2-L^2)=\frac{\hbar^2}{2}[j(j+1)+s(s+1)-l(l+1)]
\\&则\Braket{\boldsymbol {L+2S}}=\bigg[1+\frac{J(J+1)-L(L+1)+\frac{3}{4}}{2J(J+1)}\bigg]\Braket{\boldsymbol {J}}

\\&或选择z轴沿外磁场方向计算塞曼效应引起的附加能量：E_Z^1=\mu_B g_J\boldsymbol B_{ext }m_j
\\&例如基态(n=0,l=0,j=\frac{1}{2},g_J=2)分裂为两个能级：-13.6eV(1+\frac{\alpha^2}{4})\pm \mu_B B_{ext}

\end{align}
$$

- 强场塞曼效应
(帕邢巴克效应)

	- 

$$
\begin{align} &强场，塞曼效应主导，B_{ext}沿z轴，对氢原子，好量子数n,l,m_l,m_s
\\&由于外力矩存在，总角动量不守恒，L_z和S_z守恒
\\&H_Z'=\frac{e}{2m}B_{ext}(L_z+2S_z),无微扰能量E_{nm_lm_s}=-\frac{13.6eV}{n^2}+\mu_B B_{ext}(m_l+2m_s)
\\&考虑精细结构，能量一级修正：E_{fs}^1=\Braket{nlm_lm_s|(H_r'+H'_{so})|nlm_lm_s}
\\&\Braket{\boldsymbol{S\cdot L}}=\Braket{S_x}\Braket{L_x}+\Braket{S_y}\Braket{L_y}+\Braket{S_z}\Braket{L_z}=m_lm_s\hbar^2
\\&E_{fs}^1=\frac{13.6eV}{n^3}\alpha^2\bigg[\frac{3}{4n}-\frac{l(l+1)-m_lm_s}{l(l+\frac{1}{2})(l+1)}\bigg],l=0时E_{fs}^1=\frac{13.6eV}{n^3}\alpha^2\times 1

\end{align}
$$

- 中间情况塞曼效应

	- 

$$
\begin{align} &中间场，同等的将H_Z'和H_{fs}'看做哈密顿量微扰：H'=H_Z'+H_{fs}',
\\&l,j,m_j为简并微扰基,主要讨论n=2情况
\\&利用CG系数将\ket{jm_j}表示为\ket{lm_l}\ket{sm_s}的线性组合
\\&写出W矩阵并求解本征值
\\&\dots
\end{align}
$$

- 朗道能级

	- 不对称规范
	- 守恒量和简并
	- 反磁性
	- 对称规范

### 氢原子其余特性

- 超精细结构与
自旋-自旋耦合

	- 质子磁偶极矩形成磁场中电子的哈密顿量……
自旋-自旋耦合打破了基态自旋简并，提高三重态能级并降低单态能级……
21cm线……

- 外电场中的氢原子
与斯塔克效应

	- 原子置于稳恒外电场Eext中，电子能级发生改变……

- 兰姆移位

	- 电场的量子化

- 耦合表象与无耦合表象
- 范德瓦耳斯力

## 变分法

### 变分原理与薛定谔方程

- 计算哈密顿量H的体系的基态能量Egs，但本征值与本征函数未知（不能从定态薛定谔方程求解），变分原理能够给出Egs的上限，但只能用于基态的处理。
- 

$$
\begin{align} &变分原理：选取任意归一化函数\psi,有E_{gs}\le \Braket{\psi|H|\psi}=\Braket H
\\&任意波函数\psi算H的期望值必高于体系基态能量，只\psi恰为体系基态波函数\psi_0取等
\\&证明：H的本征函数组成完全集:H\psi_n=E_n\psi_n,\Braket{\psi_m|\psi_n}=\delta_{mn},\psi=\sum_n c_n\psi_n
\\&\quad对归一化的任意态\psi:1=\Braket{\psi|\psi}=\Braket{\sum_m c_m\psi_m|\sum_n c_n \psi_n}=\sum_n|c_n|^2
\\&\quad\braket H=\Braket{\sum_m c_m\psi_m|H\sum_n c_n \psi_n}=\sum_m\sum_n c_m^*E_nc_n\Braket{\psi_m|\psi_n}=\sum_n E_n|c_n|^2
\\&\quad而基态能量是最小的本征值，有E_{gs}=E_{gs}\sum_n|c_n|^2\le E_n=\braket H

\end{align}
$$
- 

$$
\begin{align} &常用试探函数：
\\1.&高斯函数：\psi(x)=Ae^{-bx^2},1=(\frac{2b}{\pi})^{1/4}
\\&\qquad 高斯函数得到的\Braket{T}=\Braket{\psi|\frac{\hat p^2}{2m}|\psi}=\frac{\hbar^2 b}{2m},\Braket{V}待定
\\2.&三角形函数：\psi(x)=\begin{cases}
Ax& 0\le x\le \frac{a}{2}\\
A(a-x)&\frac{a}{2}\le x\le a\\
0&else
\end{cases},1=\frac{2}{a}\sqrt\frac{3}{a}
\\&\frac{d\psi}{dx}=
\begin{cases}
A& 0\le x\le \frac{a}{2}\\
-A&\frac{a}{2}\le x\le a\\
0&else
\end{cases},\quad \frac{d^2\psi}{dx^2}=A\delta(x)-2A\delta(x-\frac{a}{2})+A\delta(x-a)

\end{align}
$$

### 氦原子

- 氦原子
(类氢原子)

	- 

$$
\begin{align} &\hat H=\big[-\frac{\hbar^2}{2m}\nabla_1^2-\big(\frac{1}{4\pi\varepsilon_0}\big)\frac{2e^2}{r_1}\big]+
\big[-\frac{\hbar^2}{2m}\nabla_2^2-\big(\frac{1}{4\pi\varepsilon_0}\big)\frac{2e^2}{r_2}\big]+
\frac{1}{4\pi\varepsilon_0}\frac{e^2}{|r_1-r_2|}
\\&忽略电子间排斥作用，将氦原子看做两个Z=2类氢原子相加，且核子位于坐标系中心
\\&从而能够变量分离求解：\psi(r_1,r_2)=\psi_{nlm}(r_1)\psi_{n'l'm'}(r_2)
\\&利用类氢原子公式得到E=4(E_n+E_n'),E_n=\frac{-13.6}{n^2}eV
\\&氦原子基态：\psi_0(r_1,r_2)=\psi_{100}(r_1)\psi_{100}(r_2)=\frac{8}{\pi a^3}e^{-\frac{2}{a}(r_1+r_2)}
\\&氦原子空间波函数基态对称，则自旋态反对称，氦原子基态为单态，两电子自旋方向相反
\\&氦原子激发态：\psi_{nlm}\psi_{100},若两电子均为激发态，会变成氦离子和自由电子
\\&任意态可构造出对称(与反对称自旋单态结合成仲氦)和反对称(与对称自旋单态结合成正氦)函数
\\&简单计算值：-109 eV，实验测量值：-79eV
\end{align}
$$

- 氦原子基态
(变分法)

	- 

$$
\begin{align} &忽略精细结构和很小的修正：\hat H=-\frac{\hbar^2}{2m}(\nabla_1^2+\nabla_2^2)-\frac{e^2}{4\pi\varepsilon_0}\bigg(\frac{2}{r_1}+\frac{2}{r_2}-\frac{1}{|r_1-r_2|}\bigg)
\\&氦原子的基态代表了剥离两个电子所需能量，此处应用变分原理
\\1.&试探波函数选择\psi_0(r_1,r_2)=\psi_{100}(r_1)\psi_{100}(r_2)=\frac{8}{\pi a^3}e^{-\frac{2}{a}(r_1+r_2)},其对应能量为8E_1
\\&本征方程中H\psi_0=(8E_1+V_{ee})\psi_0,则\Braket{H}=8E_1+\Braket{V_{ee}}
\\&\Braket{V_{ee}}=\Braket{\psi_0|V_{ee}|\psi_0}=\frac{e^2}{4\pi\varepsilon_0}(\frac{8}{\pi a^3})^2\int \frac{e^{-\frac{4}{a}(r_1+r_2)}}{|r_1-r_2|}d^3r_1d^3r_2，先固定r_1对r_2积分：
\\&I_2=\int \frac{e^{-\frac{4}{a}r_2}}{|r_1-r_2|}d^3r_2=\int\frac{e^{-\frac{4}{a}r_2}}{\sqrt{r_1^2+r_2^2-2r_1r_2\cos\theta_2}} r_2^2\sin\theta_2 dr_2d\theta_2 d\phi_2

\\&\quad \int\frac{\sin\theta_2 }{\sqrt{r_1^2+r_2^2-2r_1r_2\cos\theta_2}} d\theta_2 =\frac{1}{r_1r_2}[(r_1+r_2)-|r_1-r_2|]=\begin{cases}
\frac{2}{r_1}& r_2<r_1\\
\frac{2}{r_2}& r_2>r_1
\end{cases}
\\&
则I_2=4\pi\bigg(\frac{1}{r_1}\int_0^{r_1}e^{-\frac{4}{a}r_2}r_2^2dr_2+\int_{r_1}^{\infty}e^{-\frac{4}{a}r_2}r_2dr_2\bigg)=\frac{\pi a^3}{8r_1}\bigg[1-(1+\frac{2r_1}{a})e^{-\frac{4r_1}{a}}\bigg]
\\&同理积分得到：\Braket{V_{ee}}=\frac{5}{4a}(\frac{e^2}{4\pi\varepsilon_0})=-\frac{5}{2}E_1,\Braket{H}=-109eV+34eV=-75eV
\\2.&寻找比\psi_0更真实的试探函数，注意电子间相互影响，由于电子云屏蔽，实际感受到电荷量较小
\\&试探函数\psi_1(r_1,r_2)=\frac{Z^3}{\pi a^3}e^{-\frac{Z}{a}(r_1+r_2)},Z视为可变参数
，修正库伦项得到新形式哈密顿量：
\\&\hat H=-\frac{\hbar^2}{2m}(\nabla_1^2+\nabla_2^2)-\frac{e^2}{4\pi\varepsilon_0}\bigg(\frac{Z}{r_1}+\frac{Z}{r_2}\bigg)+\frac{e^2}{4\pi\varepsilon_0}\bigg(\frac{Z-2}{r_1}+\frac{Z-2}{r_2}+\frac{1}{|r_1-r_2|}\bigg)
\\&\Braket H=2Z^2E_1+2(Z-2)\frac{e^2}{4\pi\varepsilon_0}\Braket{\frac{1}{r}}+\Braket{V_{ee}}，\Braket{V_{ee}}=-\frac{5Z}{4}E_1
\\&\Braket H=[-2Z^2+\frac{27}{4}Z]E_1，\frac{d\Braket{H}}{dZ}=0时Z=1.69，此时\Braket H==-77.5eV

\end{align}
$$

- 氦原子
（微扰法）

### 氢分子

- 氢分子离子
（变分法）

	- 

$$
\begin{align} &两质子一电子：\hat H=-\frac{\hbar^2}{2m}\nabla^2-\frac{e^2}{4\pi\varepsilon_0}\bigg(\frac{1}{r_1}+\frac{1}{r_2}\bigg)，两质子固定，距离R
\\&量子化学中常用分子波函数的原子轨道线性组合法（LCAO）构造试探电子波函数：
\\&\psi=A[\psi_0(r_1)+\psi_0(r_2)],且归一化基态氢原子波函数\psi_0(r)=\frac{1}{\sqrt{\pi a^3}}e^{-\frac{r}{a}}
\\&归一化试探波函数：1=\int|\psi|^2 d^3r=|A|^2\int\bigg[|\psi_0(r_1)|^2+|\psi_0(r_2)|^2+2\psi_0(r_1)\psi_0(r_2)\bigg]d^3r
\\&选取坐标系使质子分别在坐标原点和z轴R处,电子相对质子r_1=r,r_2=\sqrt{r^2+R^2-2rR\cos\theta}
\\&I=\Braket{\psi_0(r_1)|\psi_0(r_2)}=\frac{1}{\pi a^3}\int e^{-\frac{r}{a}}e^{-\frac{\sqrt{r^2+R^2-2rR\cos\theta}}{a}} r^2\sin\theta drd\theta d\phi
\\&为对\theta 积分，令y=\sqrt{r^2+R^2-2rR\cos\theta}，则d(y^2)=2ydy=2rR\sin\theta  d\theta
\\&\dots 带入化简得到交叠积分：I=e^{-\frac{R}{a}}\bigg[1+\frac{R}{a}+\frac{1}{3}(\frac{R}{a})^2\bigg]，归一化因子|A|^2=\frac{1}{2(1+I)}
\\&\begin{cases}
(-\frac{\hbar^2}{2m}\nabla^2-\frac{e^2}{4\pi\varepsilon_0}\frac{1}{r_1})\psi_0(r_1)=E_1\psi_0(r_1)
\\
H\psi=[-\frac{\hbar^2}{2m}\nabla^2-\frac{e^2}{4\pi\varepsilon_0}(\frac{1}{r_1}+\frac{1}{r_2})]\cdot A[\psi_0(r_1)+\psi_0(r_2)]=E_1\psi-A\frac{e^2}{4\pi\varepsilon_0}[\frac{1}{r_2}\psi_0(r_1)+\frac{1}{r_1}\psi_0(r_2)]
\end{cases}
\\&\Rightarrow \Braket H=E_1-2|A|^2\frac{e^2}{4\pi\varepsilon_0}\bigg[\Braket{\psi_0(r_1)|\frac{1}{r_2}|\psi_0(r_1)}+\Braket{\psi_0(r_1)|\frac{1}{r_1}|\psi_0(r_2)}\bigg]
\\&\begin{cases}
直接积分：&D=a\Braket{\psi_0(r_1)|\frac{1}{r_2}|\psi_0(r_1)}=\frac{a}{R}-(1+\frac{a}{R})e^{-\frac{2R}{a}}\\
交换积分：&X=a\Braket{\psi_0(r_1)|\frac{1}{r_1}|\psi_0(r_2)}=(1+\frac{R}{a})e^{-\frac{R}{a}}
\end{cases}
\\&\Rightarrow \Braket H=[1+2\frac{D+X}{1+I}]E_1(电子能量),此外有质子间排斥势能：V_{pp}=\frac{e^2}{4\pi\varepsilon_0}\frac{1}{R}=-\frac{2a}{R}E_1
\\&束缚态存在，能量小于一个中性原子加自由质子能量
\end{align}
$$

- 氢分子
(海特勒-伦敦法)

### 利兹变分法

### WKB近似

## 含时微扰论
（量子动力学）

### 二能级系统

- 微扰体系

	- 

$$
\begin{align} &假设无微扰哈密顿量H^0只有两个正交归一本征态\begin{cases}
H^0\psi_a=E_a\psi_a\\ H^0\psi_b=E_b\psi_b
\end{cases}
\\&一般态：\begin{cases}
\Psi(0)=c_a\psi_a+c_b\psi_b\\
\Psi(t)=c_a\psi_a e^{-\frac{i}{\hbar}E_a t}+c_b\psi_b e^{-\frac{i}{\hbar}E_b t}
\end{cases}
\\&加入含时微扰H'(t),波函数仍为线性组合形式，问题即求解c_a(t)和c_b(t)
\\&\Psi(t)=c_a(t)\psi_a e^{-\frac{i}{\hbar}E_a t}+c_b(t)\psi_b e^{-\frac{i}{\hbar}E_b t},\begin{cases}
H\Psi=i\hbar\frac{\partial \Psi}{\partial t}\\ H=H^0+H'(t)
\end{cases}
\\&
\Rightarrow \begin{cases}
c_a[(H^0+H')\psi_a]e^{-\frac{i}{\hbar}E_a t}+c_b[(H^0+H')\psi_a]e^{-\frac{i}{\hbar}E_b t}\\
=i\hbar[\frac{d c_a}{dt}\psi_a e^{-\frac{iE_a t}{\hbar}}+\frac{d c_b}{dt}\psi_b e^{-\frac{iE_b t}{\hbar}}+c_a\psi_a(-\frac{iE_a}{\hbar})e^{-\frac{iE_a t}{\hbar}}+c_b\psi_b(-\frac{iE_b}{\hbar})e^{-\frac{iE_b t}{\hbar}}]
\end{cases}
\\&\Rightarrow
c_a[H'\psi_a]e^{-\frac{iE_a t}{\hbar}}+c_b[H'\psi_a]e^{-\frac{iE_b t}{\hbar}}
=i\hbar[\frac{d c_a}{dt}\psi_a e^{-\frac{iE_a t}{\hbar}}+\frac{d c_b}{dt}\psi_b e^{-\frac{iE_b t}{\hbar}}]
\\&标准技巧：与\psi_a做内积，利用\psi_a和\psi_b正交归一性，并定义H'_{ij}=\Braket{\psi_i|H'|\psi_j}=(H'_{ji})^*
\\&\Rightarrow c_a\Braket{\psi_a|H'|\psi_a}e^{-\frac{iE_a t}{\hbar}}+c_b\Braket{\psi_a|H'|\psi_b}e^{-\frac{iE_b t}{\hbar}}=i\hbar\frac{d c_a}{dt}e^{-\frac{iE_a t}{\hbar}}
\\&
\Rightarrow \begin{cases}
\frac{d c_a}{dt}=-\frac{i}{\hbar}[c_aH'_{aa}+c_bH'_{ab}e^{-\frac{i(E_b-E_a) t}{\hbar}}]\\
\frac{d c_b}{dt}=-\frac{i}{\hbar}[c_bH'_{bb}+c_aH'_{ba}e^{\frac{i(E_b-E_a) t}{\hbar}}]
\end{cases}
,与含时薛定谔方程完全等价
\\&若H'矩阵对角元为零:H'_{aa}=H'_{bb}=0\Rightarrow
\begin{cases}
\frac{d c_a}{dt}=-\frac{i}{\hbar}H'_{ab} e^{-i\omega_0 t}c_b\\
\frac{d c_b}{dt}=-\frac{i}{\hbar}H'_{ba} e^{i\omega_0 t}c_a
\end{cases},其中\omega_0=\frac{E_b-E_a}{\hbar}
\\\\&若没有假定H'_{aa}=H'_{bb}=0\cdots

\end{align}
$$

- 含时微扰理论

	- 

$$
\begin{align} &假设微扰H'很小，E_a\ge E_b，可以用迭代近似法求解含时系数
\\&若粒子在初始时刻处于能量较低态：c_a(0)=1,c_b(0)=0
\\&没有微扰，粒子将永远处于零级态：c_a^{(0)}(t)=1,c_b^{(0)}(t)=0
\\&一级修正代入零级近似值：\begin{cases}
\frac{d c_a^{(1)}}{dt}=0&\rightarrow c_a^{(1)}(t)=1\\
\frac{d c_b^{(1)}}{dt}=-\frac{i}{\hbar}H'_{ba} e^{i\omega_0 t}&\rightarrow
c_b^{(1)}(t)=-\frac{i}{\hbar}\int_0^t H'_{ba}(t')e^{i\omega_0 t'}dt'
\end{cases}
\\&二级修正代入一级近似值：
\begin{cases}
\frac{d c_a^{(2)}}{dt}=-\frac{i}{\hbar}H'_{ab} e^{-i\omega_0 t}(-\frac{i}{\hbar})\int_0^t H'_{ba}(t')e^{i\omega_0 t'}dt' \quad\rightarrow\\
c_a^{(2)}(t)=1-\frac{1}{\hbar^2}\int_0^t H'_{ab}(t')e^{-i\omega_0 t'}
[\int_0^{t'} H'_{ba}(t'')e^{i\omega_0 t''}dt'']dt'\\
c_b^{(2)}(t)=c_b^{(1)}(t)
\end{cases}
\\&严格解的系数满足|c_a^{(1)}(t)|^2+|c_b^{(1)}(t)|^2=1


\end{align}
$$

- 正弦微扰（周期微扰）

	- 

$$
\begin{align} &假设微扰对时间依赖关系具有正弦形式： H'(r,t)=V(r)\cos(\omega t)
\\&则有H'_{ab}=V_{ab}(\cos\omega t),V_{ab}=\Braket{\psi_a|V|psi_b}(假设矩阵对角元为0,且仅讨论一级近似，略去标记)
\\&对一级近似：c_b(t)=-\frac{i}{\hbar}V_{ab}\int_0^t \cos(\omega t')e^{i\omega_0 t'}dt'=-\frac{iV_{ab}}{2\hbar}\int_0^t [e^{i(\omega_0+\omega) t'}+e^{i(\omega_0-\omega) t'}]dt'
\\&\qquad\qquad =-\frac{V_{ab}}{2\hbar}\bigg[\frac{e^{i(\omega_0+\omega) t}-1}{\omega_0+\omega}+\frac{e^{i(\omega_0-\omega) t}-1}{\omega_0-\omega}\bigg]
\\&驱动频率\omega和跃迁频率\omega_0非常接近时(\omega_0+\omega\gg |\omega_0-\omega|),方括号第二项主要作用
\\&其他频率的微扰导致的跃迁概率非常小，可以忽略，故限制不大，舍去第一项
\\&跃迁概率：一个粒子初始处在态\psi_a，经过时间t后发现它处在态\psi_b的概率：
\\&\quad \color{orangered}
P_{a\rightarrow b}(t)=|c_b(t)|^2=\frac{|V_{ab}|^2}{\hbar^2}\frac{\sin^2[\frac{\omega_0-\omega}{2}t]}{(\omega_0-\omega)^2}
\\&只有时间t微扰（小量）时结果可信
\end{align}
$$

### 原子辐射

- 光与物质相互作用

	- 

$$
\begin{align} &\begin{cases}
假设波长远大于原子直径，忽略场的空间变化；
\\假设振荡周期比电荷在原子中运动时间长得多，可以使用静电场理论
\\假设光是单色的，极化方向沿z轴
\\假设原子核很重且固定不动
\end{cases}
\\&原子在电磁波中主要与电场作用，处于正弦电场\boldsymbol E=E_0\cos(\omega t)\hat k
\\&微扰哈密顿量：H'=-qE_0z\cos(\omega t)，\begin{cases}
矩阵元H'_{ba}=-\mathbb p E_0\cos(\omega t),
\\偶极矩\mathbb p =q\Braket{\Psi_b|z|\Psi_a}
\\V_{ba}=-\mathbb p  E_0
\end{cases}
\\&通常\psi是z的奇、偶函数，z|\psi|^2
总为奇函数，对空间积分为0
\\&符合H'对角矩阵元为0的假设，故光与物质相互作用可由振荡微扰描述

\end{align}
$$

- 吸收，受激辐射和自发辐射

	- 

$$
\begin{align} &光与原子作用三种方式：吸收，受激辐射和自发辐射
\\&原子从低能态\psi_a受单色光照射跃迁到高能态\psi_b概率：P_{a\rightarrow b}(t)=\bigg(\frac{|\mathbb p|E_0}{\hbar}\bigg)^2
\frac{\sin^2[\frac{\omega_0-\omega}{2}t]}{(\omega_0-\omega)^2}
\\&原子在该过程吸收一个光子：E_b-E_a=\hbar\omega_0。从高能态向低能态跃迁(受激辐射)概率相同
\\&激光原理：绝大多数处于高能态的原子受激辐射产生光放大的连锁反应
\\&自发辐射：高能态自发跃迁，是衰变的原理，机制是基态电磁场零点能产生的微扰


\end{align}
$$

- 非相干微扰

	- 

$$
\begin{align} &电磁波能量密度：u=\frac{1}{2}\varepsilon_0 E_0^2，单色光跃迁概率：P_{b\rightarrow a}(t)=\frac{2u}{\varepsilon_0 \hbar^2}|\mathbb p|^2
\frac{\sin^2(\frac{\omega_0-\omega}{2}t)}{(\omega_0-\omega)^2}
\\&体系一般处于具有完整频谱的电磁波场，此时u\rightarrow \rho(\omega) d\omega ，\rho(\omega)为能量密度
\\&假设不同频率的微扰彼此独立，总跃迁概率为各个跃迁概率之和，即非相干微扰
\\&P_{b\rightarrow a}(t)=\frac{2}{\varepsilon_0 \hbar^2}|\mathbb p|^2\int_0^{+\infty}\rho(\omega)
\frac{\sin^2(\frac{\omega_0-\omega}{2}t)}{(\omega_0-\omega)^2} d\omega
\approx
\frac{2}{\varepsilon_0 \hbar^2}|\mathbb p|^2\rho(\omega_0)\int_0^{+\infty}
\frac{\sin^2(\frac{\omega_0-\omega}{2}t)}{(\omega_0-\omega)^2} d\omega
\\&令x=\frac{\omega_0-\omega}{2}t,积分上下限扩展为x=\pm \infty(扩展区积分基本为0)，\int_{-\infty}^{\infty}\frac{\sin^2 x}{x^2}=\pi
\\&\Rightarrow 
P_{b\rightarrow a}(t)=\frac{\pi|\mathbb p|^2}{\varepsilon_0 \hbar^2}\rho(\omega_0) t,跃迁概率和时间成正比,跃迁速率R_{b\rightarrow a}(t)=\frac{dP}{dt}=\frac{\pi|\mathbb p|^2}{\varepsilon_0 \hbar^2}\rho(\omega_0) 为常量
\\\\&设不同方向入射光对场的能量贡献相同，对所有极化和入射方向求平均：\mathbb p=q\Braket{\psi_b|\boldsymbol r|\psi_a}
\\&\Rightarrow \mathbb p\cdot\hat n=\mathbb p\cos\theta，|\mathbb p\cdot\hat n|^2_{ave}=\frac{1}{4\pi}\int |\mathbb p|^2\cos^2\theta\sin\theta d\theta d\phi=\frac{1}{3}|\mathbb p|^2
\\&从所有方向入射的非相干、非极化光作用下跃迁速率：R_{b\rightarrow a}(t)=\frac{\pi|\mathbb p|^2}{3\varepsilon_0 \hbar^2}\rho(\omega_0)
\\&此处|\mathbb p|^2为两个态之间矩阵元，\rho(\omega_0)是\omega_0处场的能量密度
\\&跃迁速率与微扰势矩阵元平方成正比，与跃迁频率下的微扰强度成正比。费米黄金定则\dots
\end{align}
$$

- 爱因斯坦辐射理论

	- 

$$
\begin{align} &低能量\psi_a态粒子数N_a，高能量\psi_b态粒子数N_b，A为自发辐射速率
\\&\begin{cases}
自发辐射，单位时间离开高能态粒子数N_bA
\\受激辐射，单位时间离开高能态粒子数N_bB_{ba}\rho(\omega_0)
\\辐射吸收，单位时间跃迁至高能态粒子数N_aB_{ab}\rho(\omega_0)

\end{cases}
\\&\Rightarrow \frac{dN_b}{dt}=-N_bA-N_bB_{ba}\rho(\omega_0)+N_aB_{ab}\rho(\omega_0)
\\&\begin{cases}
假设原子与周围场处于热平衡，每个能级粒子数常数，有\frac{dN_b}{dt}=0
\\经典统计中热平衡态符合玻尔兹曼统计：\frac{N_a}{N_b}=\frac{e^{-\frac{E_a}{k_BT}}}{e^{-\frac{E_b}{k_BT}}}=e^{\frac{\hbar\omega_0}{k_BT}}
\\普朗克黑体辐射公式指出热辐射能量密度：\rho(\omega)=\frac{\hbar}{\pi^2 c^3}\frac{\omega^3}{e^{\frac{\hbar\omega_0}{k_BT}}-1}
\end{cases}
\\&\Rightarrow\frac{\hbar}{\pi^2 c^3}\frac{\omega^3}{e^{\frac{\hbar\omega_0}{k_BT}}-1}=
\frac{A}{e^{\frac{\hbar\omega_0}{k_BT}}B_{ab}-B_{ba}}\Rightarrow

B_{ba}=B_{ab}=\frac{\pi|\mathbb p|^2}{3\varepsilon_0 \hbar^2}

\\&根据已知的受激辐射速率可知自发辐射速率\color{orangered}A=\frac{\omega_0^3|\mathbb p|^2}{3\pi\varepsilon_0 \hbar c^3}
\\&只有自发发射时，减少的粒子数：dN_b=-AN_bdt\Rightarrow N_b(t)=N_b(0)e^{-At}
\\&激发态的寿命\tau=\frac{1}{A},若高能态衰变到多个低能态，\tau=\frac{1}{A_1+A_2+\dots}


\end{align}
$$

- 选择定则

	- 通过跃迁和矩阵元计算得到选择定则
……

### 绝热近似

- 绝热定理

	- 

$$
\begin{align} &内部时间T_i，代表系统自身运动；外部时间T_e，代表系统参数明显变化所需时间。
\\&绝热过程：外部条件缓慢变化的过程。绝热过程要求：T_e\gg T_i^1
\\&基本分析方法：先将外部参数视为常量求解问题，在计算的最后允许他们缓慢随时间变化
\\&波恩-奥本海默近似：首先固定核位置，计算电子波函数，以此获得核位置和缓慢运动信息
\\&绝热定理：\begin{cases}
假设哈密顿量从初值H^i逐渐变化到终值H^f,演化过程能谱分立不简并\\
若粒子开始时处在H^i的第n本征态，将演化至H^f的第n本征态（按薛定谔方程）\\
\Psi_n(t)=e^{i\theta_n(t)}e^{i\gamma_n(t)}\Psi_n(t)，仅增加了一对相因子
\end{cases}

\\&证明：\dots 

\end{align}
$$

- 贝瑞相

### 有限时间内的常微扰

