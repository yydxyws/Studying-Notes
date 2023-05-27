# 中心力场

## 三维库伦势

### 球对称势与分离变量法

- 

$$
\begin{align} 1.&三维直角坐标系：-\frac{\hbar^2}{2m}\nabla^2\psi+V\psi=E\psi,\quad \Psi(r,t)=\sum c_n\psi_n(r)e^{-\frac{i}{\hbar}E_n t}
\\2.&球坐标系与分离变量：设解的形式\psi(r,\theta,\phi)=R(r)Y(\theta,\phi)
\\&\nabla^2=\frac{1}{r^2}\frac{\partial }{\partial r}\bigg(r^2\frac{\partial }{\partial r}\bigg)+\frac{1}{r^2\sin \theta}\frac{\partial }{\partial \theta}\bigg(\sin\theta\frac{\partial }{\partial \theta}\bigg)+\frac{1}{r^2\sin^2\theta}\frac{\partial ^2}{\partial \phi^2}
\\\Rightarrow&-\frac{\hbar^2}{2m}\bigg[\frac{Y}{r^2}\frac{d}{dr}\bigg(r^2\frac{dR}{dr}\bigg)+

\frac{R}{r^2\sin \theta}\frac{\partial}{\partial\theta}\bigg(\sin\theta\frac{\partial Y}{\partial\theta}\bigg)+\frac{R}{r^2\sin^2\theta}\frac{\partial^2Y}{\partial\phi^2}\bigg]+VRY=ERY
\\\Rightarrow&\begin{cases}
径向方程&\big[\frac{1}{R}\frac{d}{dr}\big(r^2\frac{dR}{dr}\big)-\frac{2mr^2}{\hbar^2}(V-E)\big]=\lambda=l(l+1)\\
角向方程&\frac{1}{Y}\big[\frac{1}{\sin \theta}\frac{\partial}{\partial\theta}\big(\sin\theta\frac{\partial Y}{\partial\theta}\big)+\frac{1}{\sin^2\theta}\frac{\partial^2Y}{\partial\phi^2}\big]=-\lambda=-l(l+1)
\end{cases}

\end{align}
$$

### 角向波函数与角向解

- 

$$
\begin{align} &\sin \theta\frac{\partial}{\partial\theta}\big(\sin\theta\frac{\partial Y}{\partial\theta}\big)+\frac{\partial^2Y}{\partial\phi^2}=-l(l+1)\sin^2\theta Y,分离变量Y(\theta,\phi)=\Theta(\theta)\Phi(\phi)
\\&方位角函数：\frac{1}{\Phi}\frac{d^2\Phi}{d\Phi^2}=-m^2\rightarrow \Phi(\phi)=e^{im\phi},且\Phi(\phi+2\pi)=\Phi(\phi)\rightarrow m=0,\pm 1\dots
\\&俯仰角函数：\sin \theta\frac{d}{d\theta}\big(\sin\theta\frac{d\Theta}{d\theta}\big)+[l(l+1)\sin^2\theta -m^2]\Theta=0\rightarrow \Theta(\theta)=AP_l^m(\cos\theta)
\\&关联勒让德函数：P_l^m(x)=(1-x^2)^{\frac{|m|}{2}}\big(\frac{d}{dx}\big)^{|m|}P_l(x)
\\&勒让德多项式（罗德里格公式）：P_l(x)=\frac{1}{l!2^l}\big(\frac{d}{dx}\big)^{l}(x^2-1)^l,\quad P_0=1,P_1=x\dots
\\&为使罗德里格公式有意义，要求l为非负整数；关联勒让德函数非零要求|m|<l
\\&归一化条件：\int_0^\infty |R|^2r^2dr=1,\int_0^{2\pi}\int_0^\pi |Y|^2\sin\theta d\theta d\phi=1
\\&归一化的角向波函数：Y_l^m(\theta,\phi)=\varepsilon\sqrt{\frac{(2l+1)(l-|m|)!}{4\pi (l+|m|)!}} e^{im\phi}P_l^m(\cos\theta),\varepsilon=\begin{cases}
(-1)^m&m\ge 0\\
1 &m\le 0
\end{cases}
\\&角量子数：l，磁量子数：m，Y_0^0=\frac{1}{2\sqrt\pi}，Y_1^0=(\frac{3}{4\pi})^{\frac{1}{2}}\cos\theta\dots

\end{align}
$$
- 连带勒让德函数与球谐函数

### 径向波函数与合流超几何函数

- 

$$
\begin{align} &\frac{d}{dr}\big(r^2\frac{dR}{dr}\big)-\frac{2mr^2}{\hbar^2}(V-E)R=l(l+1)R，令u(r)=rR(r)
\\&径向方程：-\frac{\hbar^2}{2m}\frac{d^2u}{dr^2}+\big[V+\frac{\hbar^2}{2m}\frac{l(l+1)}{r^2}\big]u=Eu,有效势含有离心项\frac{2mr^2}{\hbar^2}\frac{l(l+1)}{r^2}
\\&指定势为V(r)=\begin{cases}
0&r<a\\\infty &r>a
\end{cases}\quad\Rightarrow \frac{d^2u}{dr^2}=\big[\frac{l(l+1)}{r^2}-k^2\big]u,k^2=\frac{2mE}{\hbar^2}
\\&对l=0：u(r)=A\sin(kr)+B\cos(kr),\begin{cases}
满足r\rightarrow 0存在条件：B=0
\\满足边界条件u(a)=0：ka=n\pi
\end{cases}
\\&\qquad 得到E_{n0}=\frac{n^2\pi^2\hbar^2}{2ma^2},\psi_{n00}=\frac{1}{\sqrt{2a\pi}}\frac{\sin(\frac{n\pi r}{a})}{r}
\\&对l任意：u(r)=Ar\cdot j_l(kr)+Br\cdot n_l(kr),\begin{cases}
j_l(x)=(-x)^l\big(\frac{1}{x}\frac{d}{dx}\big)^l\frac{\sin x}{x}(球贝塞尔函数)\\
n_l(x)=-(-x)^l\big(\frac{1}{x}\frac{d}{dx}\big)^l\frac{\cos x}{x}(球诺依曼函数)
\end{cases}
\\&\qquad \begin{cases}
满足x=0存在：B=0，R(r)=A \cdot j_l(kr)\\
满足边界条件：j_l(ka)=0,k=\frac{\beta_{Nl}}{a},\beta_{Nl}为l阶贝塞尔函数的第N个零点
\end{cases}
\\&\qquad E_{nl}=\frac{\hbar^2}{2ma^2}\beta_{nl}^2，\psi_{nlm}(r,\theta,\phi)=A_{nl}\cdot j_l(\frac{r\beta_{Nl}}{a}) \cdot Y_l^m(\theta,\phi)
\\&每个l对应2l+1个m，每个(nl)能级2l+1重简并

\end{align}
$$
- 无限深球形势阱

### 束缚态与束缚态幂次对应关系

### 自由粒子

### 三维谐振子

## 氢原子

### 氢原子的波函数

- 

$$
\begin{align} &E<0：以质子为原点应用质心坐标系，势能V(r)=-\frac{e^2}{4\pi\varepsilon_0}\frac{1}{r}
\\&(质子不在原点时分离变量解仍可分离出下式)
\\&-\frac{\hbar^2}{2m}\frac{d^2u}{dr^2}+\big[-\frac{e^2}{4\pi\varepsilon_0}\frac{1}{r}+\frac{\hbar^2}{2m}\frac{l(l+1)}{r^2}\big]u=Eu，令\kappa=-\frac{2mE}{\hbar^2}，
\\&引入\rho=\kappa r,\rho_0=\frac{me^2}{2\pi\varepsilon_0 \hbar^2\kappa}
\Rightarrow \frac{d^2 u}{d\rho^2}=[1-\frac{\rho_0}{\rho}+\frac{l(l+1)}{\rho^2}]u
\\&渐近试探\begin{cases}
\rho\rightarrow \infty，常数项主导：\frac{d^2u}{d\rho^2}=u，形式解： u(\rho)=Ae^{-\rho}+be^{\rho}=Ae^{-\rho}
\\
\rho\rightarrow 0,离心项主导:\frac{d^2u}{d\rho^2}=\frac{l(l+1)}{\rho^2}u,形式解: u(\rho)=C\rho^{l+1}+D\rho^{-l}=C\rho^{l+1}(l=0除外)
\end{cases}
\\&将渐进形式解分离出去,令u(\rho)=\rho^{l+1}e^{-\rho}v(\rho),逐阶代入径向方程求导并化简
\\&得\rho\frac{d^2 v}{d \rho^2}+2(l+1-\rho)\frac{dv}{d\rho}+[\rho_0-2(l+1)]v=0[广义拉盖尔方程]
\\&令v(\rho)=\sum_{j=0}^{+\infty} c_j\rho_j
,逐次求导，令同幂次项系数相等，得c_{j+1}=\frac{2(j+l+1)-\rho_0}{(j+1)(j+2l+2)}c_j
\\&令级数中断，c_{j+1}=0。定义主量子数n=j_{max}+l+1,此时\rho=2n

\end{align}
$$
- 

$$
\begin{align} &经典力学结论\begin{cases}
束缚态E<0：经典椭圆轨道，对应原子中电子运动\\
临界态E=0：经典抛物线轨道，对应电子电离\\
散射态E>0：经典双曲线轨道，对应卢瑟福散射
\end{cases}

\\&E=-\frac{\hbar^2\kappa^2}{2m}=-\frac{me^4}{8\pi^2\varepsilon_0^2\hbar^2\rho_0^2}=-\bigg[\frac{m}{2\hbar^2}\big(\frac{e^2}{4\pi\varepsilon_0}\big)^2\bigg]\frac{1}{n^2}=\frac{E_1}{n^2}【玻尔公式】
\\&\kappa=\big(\frac{me^2}{4\pi\varepsilon_0\hbar^2}\big)\frac{1}{n}=\frac{1}{an},玻尔半径：a=\frac{4\pi\varepsilon_0\hbar^2}{me^2},则\rho=\frac{r}{an}
\\\\&氢原子空间波函数\psi_{nlm}(r,\theta,\phi)=R_{nl}(r)Y_l^m(\theta,\phi),
\\& \begin{cases}
R_{nl}(r)=\frac{1}{r}\rho^{l+1} e^{-\rho} v(\rho),\rho=\kappa r,u=Rr\\
v(\rho)是最高幂次为j_{max}=n-l-1的多项式，c_{j+1}=\frac{2(j+l+1-n)}{(j+1)(j+2l+2)}c_j\\
关联拉盖尔多项式:L_{q-p}^p(x)=(-1)^p(\frac{d}{dx})^p L_q(x),L_q(x)=e^x(\frac{d}{dx})^q(e^{-x}x^q)
\end{cases}
\\&能级E_n的总简并度d(n)=\sum_{l=0}^{n-1}(2l+1)=n^2
\\&氢原子基态：\boldsymbol{\color{red}\psi_{100}=R_{10}(r)Y_0^0=\frac{2}{a^{3/2}}e^{-\frac{r}{a}}\cdot\frac{1}{\sqrt{4\pi}}=\frac{1}{\sqrt{\pi a^3}}\cdot e^{-\frac{r}{a}}}
\\&归一化氢原子波函数：\psi_{nlm}=\sqrt{\big(\frac{2}{na}\big)^3\frac{(n-l-1)!}{2n[(n+l)!]^3}}\cdot e^{-\frac{r}{na}}\cdot \big(\frac{2r}{na}\big)^l\cdot\big[L_{n-l-1}^{2l+1}(\frac{2r}{na})\big]\cdot Y_l^m(\theta,\phi)
\\&径向概率密度：W_{nl}(r)dr=|R_{nl}(r)|^2r^2dr
\\&角向概率密度：W_{lm}(\theta,\phi)d\Omega=|Y_{lm}(\theta,\phi)|^2d\Omega
\end{align}
$$

### 氢原子和类氢离子光谱

- 氢原子能级图
- 

$$
\begin{align} &氢原子能谱E_n=-\frac{\mu e^4}{2\hbar^2}\frac{1}{n^2}=-\frac{e^2}{2a}\frac{1}{n^2},a=\frac{\hbar^2}{\mu e^2},n=1,2,3...
\\&类氢离子能谱E_n=-\frac{\mu e^4}{2\hbar^2}\frac{Z^2}{n^2}=-\frac{e^2}{2a}\frac{Z^2}{n^2},a=\frac{\hbar^2}{\mu e^2},n=1,2,3...这里的Z即原子核所带正电荷数.
\\&类氢离子势场V(r)=-\frac{Ze^2}{r}中，定态波函数\psi_{nlm}(r)=R_{nl}(r)Y_{lm}(\theta,\varphi)
\\&R_{nl}(r)=N_{nl}e^{-\frac{Zr}{na}}(\frac{2Zr}{na})^lF(l+1-n,2l+2,\frac{2Zr}{na})
N_{nl}=\frac{2}{a^{3/2}n^2(2l+1)!}\sqrt{\frac{(n+l)!}{(n-l-1)!}},n=1,2,3...
\\&其中a是波尔半径，F是合流超几何函数，基态时(n=1),R_{10}=\frac{2}{a^{3/2}}e^{-r/a}
\\&氢原子光谱里德伯公式：\frac{1}{\lambda}=R(\frac{1}{n_i^2}-\frac{1}{n_f^2}),里德伯常量R=\frac{m}{4\pi c\hbar^3}(\frac{e^2}{4\pi\varepsilon_0})^2

\end{align}
$$

### 二维中心力场

- 二维无限深圆方势阱
- 二维各向同性谐振子
- 二维氢原子和类氢离子

## 角动量理论

### 本征值与本征函数

- 升降算符法

	- 本征值

		- 

$$
\begin{align} &角动量基本对易关系：[L_x,L_y]=i\hbar L_z,\quad[L^2,L_x]=0,\quad[L^2,\boldsymbol L]=0
\\&\begin{cases}
L^2f=\lambda f\\ L_z f=\mu f
\end{cases},\color{orangered}，构造升降算符:\begin{cases}
升阶：L_+=L_x+ iL_y,\\ 降阶：L_-=L_x- iL_y
\end{cases}
\\&L_\pm L_\mp=L^2-L_z^2\mp i(i\hbar L_z)\rightarrow L^2=L_\pm L_\mp +L_z^2\mp \hbar L_z
\\&对易关系：[L_z,L_\pm]=[L_z,L_x]\pm i[L_z,L_y]=i\hbar L_y\pm i(-i\hbar L_x)=\pm \hbar L_\pm
\\&\qquad\qquad  [L^2,L_\pm]=[L^2,L_x]\pm i[L^2,L_y]=0
\\& f和L_\pm f都是L^2本征值为\lambda的本征函数：L^2(L_\pm f)=\lambda L_\pm f
\\&\color{orangered}L_\pm f是L_z本征值为\mu\pm\hbar的本征函数：\begin{cases}
L_z(L_+ f)=(\mu+\hbar)L_+f\\
L_z(L_-f)=(\mu-\hbar)L_-f
\end{cases}
\\&\begin{cases}
最高阶梯f_t:&\begin{cases}L_+f_t=0 ,本征值: l\hbar,\quad
\begin{cases}
L_zf_t=\hbar lf_t\\L^2 f_t=\lambda f_t
\end{cases}\\
L^2 f_t=(L_-L_++L_z^2+\hbar L_z)f_t= l(l+1)\hbar^2f_t
\end{cases}
\\
最低阶梯f_b:&\begin{cases}L_-f_b=0 ,
本征值:\bar l\hbar,\quad
\begin{cases}
L_zf_b=\hbar \bar lf_b\\L^2 f_b=\lambda f_b
\end{cases}\\
L^2 f_b=(L_+L_-+L_z^2-\hbar L_z)f_b= \bar l(\bar l-1)\hbar^2f_b
\end{cases}
\end{cases}
\\&综上，有\begin{cases}
\lambda=l(l+1)\hbar^2\\
\lambda=\bar l(\bar l-1)\hbar^2
\end{cases},两者表示同一个量，有\bar l=-l
\\&L_z本征值显然为m\hbar,-l升阶N次为l阶,l=\frac{N}{2}为整数或半整数
\\&\color{orangered}角动量本征方程：\begin{cases}
L^2f_l^m=l(l+1)\hbar^2 f_l^m &,l=0,\frac{1}{2},1,\frac{3}{2}\cdots\\
L_z f_l^m=m\hbar f_l^m&,
m=-l,-l+1,\dots,l-1,l
\end{cases}
\\&L_\pm f_l^m=A_l^m f_l^{m\pm 1}\rightarrow A_l^m=\sqrt{l(l+1)-m(m\pm 1)}\hbar
\end{align}
$$

	- 本征函数

		- 

$$
\begin{align} 
&\begin{cases}
\boldsymbol L=\frac{\hbar}{i}(\boldsymbol r\times\nabla),\\
\nabla=\hat r\frac{\partial }{\partial r}+\hat \theta\frac{1}{r}\frac{\partial }{\partial \theta}+\hat\phi\frac{1}{r\sin\theta}\frac{\partial }{\partial \phi},
\end{cases}
\Rightarrow
\begin{cases}
\boldsymbol r=\hat r r\\
\hat r\times \hat r=0\\
\hat r\times \hat \theta=\hat\phi\\
\hat r\times \hat \phi=-\hat\theta
\end{cases}
\Rightarrow \boldsymbol L=-i\hbar\bigg(\hat\phi\frac{\partial }{\partial \theta} -\hat\theta\frac{1}{\sin\theta}\frac{\partial }{\partial \phi}\bigg)
\\&\begin{cases}
\hat r=(\sin\theta\cos\phi)\hat i+(\sin\theta\sin\phi)\hat j+(\cos\theta)\hat k
\\
\hat\theta=(\cos\theta\cos\phi)\hat i+(\cos\theta\sin\phi)\hat j-(\sin\theta)\hat k
\\
\hat\phi=-(\sin\phi)\hat i+(\cos\phi)\hat j
\end{cases}
\Rightarrow 
\begin{cases}
L_x=-i\hbar(-\sin\phi\frac{\partial }{\partial \theta}-\cos\phi\cot\theta\frac{\partial }{\partial \phi})
\\
L_y=-i\hbar(\cos\phi\frac{\partial }{\partial \theta}-\sin\phi\cot\theta\frac{\partial }{\partial \phi})
\\
L_z=-i\hbar \frac{\partial }{\partial \phi}
\end{cases}
\\&\Rightarrow L_\pm=\pm\hbar e^{\pm i\phi}\bigg(\frac{\partial }{\partial \theta}\pm i\cot\theta \frac{\partial }{\partial \phi}\bigg)
\Rightarrow L_+L_-=-\hbar^2 \bigg(\frac{\partial^2 }{\partial \theta^2}+ \cot\theta \frac{\partial }{\partial \theta}+\cot^2\theta \frac{\partial^2 }{\partial \phi^2}+i\frac{\partial }{\partial \phi}\bigg)
\\&\Rightarrow L^2=-\hbar^2\bigg[\frac{1}{\sin\theta} \frac{\partial }{\partial \theta}\bigg(\sin\theta \frac{\partial }{\partial \theta}\bigg)+\frac{1}{\sin^2\theta} \frac{\partial ^2}{\partial \phi^2}\bigg]
\\&\begin{cases}
角向方程：L^2f_l^m=-\hbar^2\bigg[\frac{1}{\sin\theta} \frac{\partial }{\partial \theta}\bigg(\sin\theta \frac{\partial }{\partial \theta}\bigg)+\frac{1}{\sin^2\theta} \frac{\partial ^2}{\partial \phi^2}\bigg]f_l^m=l(l+1)\hbar^2f_l^m\\
方位角方程：L_zf_l^m=-i\hbar \frac{\partial ^2}{\partial \phi^2}f_l^m=m\hbar f_l^m

\end{cases}
\\&根据氢原子计算结果知，本征函数为球谐函数Y_l^m(\theta,\phi)
\\&注意：角动量代数理论中，l可以是半整数。分离变量理论中，l只能是整数值
\end{align}
$$

- 分析法

	- 动量和坐标算符代入，求导，化简

### 角动量普遍性质

### 角动量的本征值与矩阵表述

### 总角动量本征态求解

