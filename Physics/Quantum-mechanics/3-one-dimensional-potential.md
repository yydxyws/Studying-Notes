# 一维势场中的粒子

## 无限深方势阱
（束缚态）

### 

$$
\begin{align} &对于宽度为a的势阱:V(x)=\begin{cases}
0,0<x<a
\\\infty,else
\end{cases}.
\\&(1)势场的变化\Delta V有限，波函数及其导数均连续），\\&(2)波函数无穷远处为零
\\&\color {blue} E=\frac{n^2\pi^2\hbar^2}{2ma^2},
\psi_n(x)=\begin{cases}
\sqrt{\frac{2}{a}}\sin(\frac{n\pi x}{a}),&0<x<a
\\\infty,&else
\end{cases}
\\&若|x|\le\frac{a}{2}时V=0，有\psi_n(x)=
\sqrt{\frac{2}{a}}\sin [n\pi(\frac{x}{a}+\frac{1}{2})]

\end{align}
$$

## 自由粒子

### 

$$
\begin{align} &【分析】自由粒子E=T>V(x)=0恒成立,为散射态,令k=\frac{\sqrt{2mE}}{\hbar},\omega=\frac{\hbar k^2}{2m}
\\&\frac{d^2\psi}{d x^2}=-k^2\psi\Rightarrow \psi(x)=Ae^{ikx}+Be^{-ikx}\Rightarrow \psi(x,t)=Ae^{ikx-i\omega t}+Be^{-ikx-i\omega t}
\\&自由粒子波函数类似于行波，一般解为\color{blue}\Psi(x,t)=\frac{1}{\sqrt{2\pi}}\int \phi(k)e^{i(kx-\frac{\hbar k^2}{2m}t)}dk
\\&【说明】一般解仍然为分离变量解的线性组合，但是对n求和变为对k积分
\\&自由粒子的分离变量解不代表物理上可实现的态，没有确定能量
\\&但是对限制k值范围的\phi(k),波函数能够归一化，其表示自由粒子波包(干涉叠加)
\\&自由粒子一般问题是求解\color{blue}\phi(k)=\frac{1}{\sqrt{2\pi}}\int \Psi(x,0)e^{-ikx}dx
\\&【波包】波包运动速度为群速：v_{g}=\frac{d\omega}{dk},定态运动速度为相速：v_p=\frac{\omega}{k}
\\&【高斯波包】粒子的位置分布是高斯分布:|\psi(x)|^2=\frac{1}{\sigma_x\sqrt{2\pi}}e^{-\frac{x^2}{2\sigma_x^2}}
\\&高斯波包即最小不确定波包\sigma_x\sigma_p=\frac{\hbar}{2}，
\\&在坐标表象下：\psi(x)=\frac{1}{(2\pi\sigma_x)^{\frac{1}{4}}}e^{-\frac{x^2}{(2\sigma_x)^2}},动量表象下也是高斯分布
\\&一般解：\Psi(x)=Ae^{-\frac{a}{2\hbar}(x-\braket{x})^2}e^{\frac{i}{\hbar}\braket px}


\end{align}
$$

## 一维谐振子

### 分析法求解

- 厄米多项式

	- 

$$
\begin{align} 量子体系哈密顿算符：&
    \hat{H}=-\frac{\hbar^2}{2m}\frac{\partial^2 }{\partial x^2}+\frac{1}{2}m\omega^2 x^2
\\定态薛定谔方程：&
    -\frac{\hbar^2}{2m}\frac{d^2\psi}{dx^2}+\frac{1}{2}m\omega^2x^2\psi=E\psi 
\\引入无量纲参数：&\color{blue}
    \lambda =\frac{2E}{\hbar \omega},\quad \xi=\alpha x\quad(\alpha=\sqrt{\frac{m\omega}{\hbar}})
 \\方程两边乘\frac{2}{\hbar \omega}，得到：&
    -\frac{1}{(\frac{m\omega}{\hbar})}\frac{d^2\psi(x)}{dx^2}+(\frac{m\omega}{\hbar})x^2\psi(x)=\frac{2E}{\hbar \omega}\psi(x)  
 \\ 量子谐振子标准方程：&
        \psi''(\xi)+(\lambda-\xi^2)\psi(\xi)\quad 
 \\\xi\rightarrow\pm\infty,\lambda<<\xi^2 ：&
          \frac{d^2\psi}{d\xi^2}-\xi^2\psi=0\rightarrow \psi(\xi)=Ae^{-\frac{\xi^2}{2}}+Be^{\frac{\xi^2}{2}}\rightarrow Ae^{-\frac{\xi^2}{2}}
\\方程的渐进形式解：&   \psi(\xi)=e^{-\frac{\xi^2}{2}}H(\xi)
\\厄米方程：&
  \label{emi}  \frac{d^2H}{d\xi^2}-2\xi\frac{dH}{d\xi}+(\lambda-1)H=0
\\厄米方程有限解条件：&
    \lambda-1=2n, n=0,1\dots\rightarrow\color{blue}线性谐振子能量：    E_n=\hbar \omega(n+\frac{1}{2})
\\对应厄米多项式的解：&\color{blue}
    H_n(\xi)=(-1)^n e^{\xi^2}\frac{d^n}{d\xi^n}e^{-\xi^2},\quad n=0,1\dots,H_0=1,H_1=2\xi\dots
\\薛定谔方程的解： &  \color{blue} \psi_n(\xi)=N_ne^{-\frac{\xi^2}{2}}H_n(\xi)\quad \mbox{或}\psi_n(x)=N_n e^{-\frac{\alpha^2x^2}{2}}H_n(\alpha x)
\\对应的归一化因子：&\color{blue}
    N_n=\sqrt{\frac{\alpha}{\sqrt{\pi}2^n n!}}=\big(\frac{m\omega}{\pi\hbar}\big)^{\frac{1}{4}} \frac{1}{\sqrt{2^n n!}}
\\厄米多项式性质：&\frac{d H_n}{d\xi}=2nH_{n-1}(\xi)，H_{n+1}(\xi)=2\xi H_n(\xi)-2nH_{n-1}(\xi)
\\一维谐振子基态：&\color{blue} \psi_0=\sqrt{\frac{\alpha}{\sqrt{\pi}}}e^{-\frac{1}{2}\alpha^2 x^2}
=\big(\frac{m\omega}{\pi\hbar}\big)^{\frac{1}{4}}e^{-\frac{m\omega}{2\hbar}x^2}
\end{align}
$$

- 谐振子能谱

	- 

### 升降算符法求解

- 

$$
\begin{align} 哈密顿算符：&\hat{H}=\frac{1}{2m}(\hat{p}^2+m^2\omega^2\hat{x}^2)=\frac{1}{2m}\big[(m\omega x)^2-(i)^2(-i\hbar\frac{d}{dx})^2\big]
=\frac{1}{2m}\big[(m\omega x+i\hat p)(m\omega x-i\hat p)\big]

\\&令\xi=\sqrt{\frac{m\omega}{\hbar}}x,构造\color{orangered}升降算符\hat{a}_{\pm}=\frac{1}{\sqrt{2mw\hbar}}(m\omega\hat{x}\mp i\hat{p})=\sqrt{\frac{m\omega}{2\hbar}}(x\mp \frac{i\hat p}{m\omega})=\frac{1}{\sqrt 2}(\xi\mp \frac{\partial }{\partial \xi})

\\&\hat a_-\hat a_+=\frac{1}{\omega\hbar}\frac{1}{2m}[\hat p^2+(m\omega \hbar)^2]+\frac{1}{2}=\frac{1}{\hbar\omega} \hat H+\frac{1}{2}\quad\Rightarrow\color{orangered} \hat H=(\hat a_+\hat a_-+\frac{1}{2})\hbar\omega=(\hat N+\frac{1}{2})\hbar\omega

\\ 
\\算符定义：&\begin{cases}
湮灭算符：&\hat a=\hat a_-  =\frac{1}{\sqrt 2}(\xi+ \frac{\partial }{\partial \xi})=
\frac{1}{\sqrt 2}(\alpha x+\frac{1}{\alpha}\frac{\partial }{\partial x})

\\产生算符：&\hat a^+=\hat a_+  =\frac{1}{\sqrt 2}(\xi- \frac{\partial }{\partial \xi})=
\frac{1}{\sqrt 2}(\alpha x-\frac{1}{\alpha}\frac{\partial }{\partial x})
\end{cases}，粒子数算符：\hat N=\hat a_+\hat a_-
   \\阶梯作用：&\color{orangered}\hbar\omega(\hat a_\pm \hat a_\mp\pm\frac{1}{2})\psi=E\psi \rightarrow \begin{cases}
\hat H \hat a_- \psi=(E-\hbar \omega)\hat a_-\psi\\
\hat H \hat a_+ \psi=(E+\hbar \omega)\hat a_+ \psi
\end{cases} ,\qquad递推关系：\begin{cases}
\hat{a}_{+}\psi_{n}=\sqrt{n+1}\psi_{n+1}
\\\hat{a}_{-}\psi_{n}=\sqrt{n}\psi_{n-1}
\end{cases}
 \\对易关系：&\begin{cases}玻色子算符：&
[\hat a_-,\hat a_+]=1 ，[\hat a_-,\hat a_-]=[\hat a_+,\hat a_+]=0\\
费米子算符：&\{\hat a_-,\hat a_+\}=1 ，\{\hat a_-,\hat a_-\}=\{\hat a_+,\hat a_+\}=0
\\共同对易关系：&[\hat a_-,\hat N]=\hat a_-，[\hat a_+,\hat N]=-\hat a_+
\end{cases}
\\最低阶梯：&\hat{a}_{-}\psi_0=0\rightarrow \frac{1}{\sqrt{2m\omega \hbar}}(i\hat p+m\omega x)\psi_0=0\rightarrow\frac{d\psi_0}{dx}=-\frac{m\omega x}{\hbar}\psi_0



\\&积分，归一化，求解，得到基态函数\psi_0=(\frac{m\omega}{\pi\hbar})^{\frac{1}{4}}\cdot e^{-\frac{m\omega}{2\hbar}x^2}和零点能量E_0=\frac{1}{2}\hbar\omega
\\一般态函数：&反复使用产生算符：\psi_n(x)=A_n(\hat a_+)^n\psi_0(x)=\frac{1}{\sqrt{n!}}(\hat a_+)^n\psi_0
  \\ 力学量表示：&\hat x=\sqrt{\frac{\hbar}{2m\omega}}(\hat a_++\hat a_-)=\frac{1}{\sqrt 2 \alpha}(\hat a_++\hat a_-)
,\quad \hat p=i\sqrt{\frac{m\omega\hbar}{2}}(\hat a_+-\hat a_-)=\frac{\alpha \hbar}{\sqrt 2 }(\hat a_+-\hat a_-)
\\\\占有数表象：&以\ket n为基矢的表象，算符的矩阵元\begin{cases}\quad
\Braket{{n'}|\hat a_-|n}=\sqrt{n}\cdot \delta_{n',n-1}\\
\quad \Braket{{n'}|\hat a_+|n}=\sqrt{n+1} \cdot\delta_{n',n+1}
\end{cases}


\end{align}
$$

## δ势阱

### 微积分性质讨论束缚态

- 

$$
\begin{align}   势函数：&  V(x)=-\frac{\hbar^2\Omega}{m}\delta(x)，\Omega是正常数，刻画\delta势阱强度。
\\
{束缚态(E<0):}&
\\
x\ne 0时：&
    \frac{d^2\psi}{dx^2}-k^2\psi=0\quad \rightarrow k=\sqrt{-\frac{2mE}{\hbar^2}},通解\psi(x)=Ae^{kx}+Be^{-kx}
\\&
又\psi(\pm \infty)=0，\psi(x)在x=0处连续，
有    \psi(x)=\begin{cases}
        Ae^{kx}&(x<0)\\ Ae^{-kx}&(x>0)
    \end{cases},
\\跃变条件：&对波函数求导：    \psi'(x)=\begin{cases}
        kAe^{kx}=k\psi(x)&(x<0)\\  -kAe^{-kx}=-k\psi(x)&(x>0)
    \end{cases}
\\&由于\delta(0)\rightarrow\infty,\psi(0)\rightarrow\infty，导数\psi'(x)在x=0不连续. 
\\&   \psi'(0^+)-\psi'(0^-)=-k(A+B)=-2kA\quad[微分角度的不连续行为]
\\&
对方程在[-\varepsilon,\varepsilon](\varepsilon\rightarrow0)积分：    -\frac{\hbar^2}{2m}\int_{-\varepsilon}^{\varepsilon} d  \big[\psi'(x)\big]-\frac{\hbar^2\Omega}{m}\int_{-\varepsilon}^{\varepsilon} \delta(x)\psi(x)d x=E\int_{-\varepsilon}^{\varepsilon} \psi(x)d x
\\&微分中值定理:\int_{-\varepsilon}^{\varepsilon} \psi(x)d x\approx 2\varepsilon\psi(0)\xrightarrow{\varepsilon\rightarrow0}0，\delta 函数性质:\int f(x)\delta(x-0)=f(0)
\\&即    \psi'(0^+)-\psi(0^-)=-2\Omega\psi(0)\quad(\mbox{积分角度的不连续行为})
 \\ &  联立有2kA=2\Omega\psi(0)，\psi(0)=\frac{kA}{\Omega}
    ，又\psi(0)=Ae^{kx}=A，则k=\Omega=\frac{m\alpha}{\hbar^2}
\\
    \delta势阱能量：&E=-\frac{\hbar^2\Omega^2}{2m}=-\frac{m\alpha^2}{2\hbar^2},体系只有一个束缚态。
 \\ 本征函数：&\psi(x)=\sqrt{\Omega}\cdot e^{-\Omega{|x|}}=\frac{\sqrt{m\alpha}}{\hbar}\cdot e^{-\frac{m\alpha}{\hbar^2}|x|}
\end{align}
$$

### 散射态物理意义与波包

- 

$$
\begin{align}   势函数：&  V(x)=-\frac{\hbar^2\Omega}{m}\delta(x)，\Omega是正常数，刻画\delta势阱强度。
\\散射态(E>0)：&\frac{d^2\psi}{dx^2}-k^2\psi=0\quad \rightarrow k=\sqrt{\frac{2mE}{\hbar^2}}
\\通解：&\psi(x)=\begin{cases}
Ae^{ikx}+Be^{-ikx},x<0\\
Ce^{ikx}+De^{-ikx},x>0
\end{cases}
,\psi'(x)=
\begin{cases}
ik(Ae^{ikx}-Be^{-ikx}),x<0\\
ik(Ce^{ikx}-De^{-ikx}),x>0
\end{cases}
\\性质分析：&\psi(x)连续，\psi(0)=A+B=B+C
\\&\psi'(x)跃变，有\psi'(\varepsilon)-\psi'(-\varepsilon)=-2\Omega\psi(0)，令\beta=\frac{m\alpha}{\hbar^2 k}
\\&即ik(C-D-A+B)=-2\Omega(A+B)\rightarrow C-D-A+B=2i\beta (A+B)
\\物理意义：&假定从左方入射，ABCD为入射、反射、透射波振幅及0，A为自由变量
\\&C=\frac{1}{1-i\beta}A，B=\frac{i\beta}{1-i\beta}A
\\&反射系数：R=\frac{|B|^2}{|A|^2}=\frac{1}{\frac{2\hbar^2 E}{m\alpha^2}+1}，透射系数：T=\frac{|C|^2}{|A|^2}=\frac{1}{\frac{m\alpha^2}{2\hbar^2 E}+1}
\\&以上散射波不能实现归一化，需要构造定态解的线性组合，表示波包

\end{align}
$$

## 一维方势垒
和一维方势阱

### 

$$
\begin{align} &能量 E 的粒子正方向射向方势垒：V(x)=\left\{\begin{array}{lc}{V_{0} }&{ 0<x<a}\\{0 }&x<0或x>a
\end{array}\right.
\\&入射波振幅取1，k^2=\frac{2mE}{\hbar^2},k_0^2=\frac{2m}{\hbar^2}(V_0-E),
\left\{\begin{array}{lc}
\psi_I={e^{ikx}+Re^{-ikx}}&x<0
\\\psi_{III}=Se^{ikx}&{x>a}\end{array}\right.
\\0<E<V_0：&势垒穿透，\psi_{II}=Ae^{gx}+Be^{-gx}(0<x<a)

\\&波函数和导函数连续，利用RS消去AB：\begin{cases}
1+R\frac{k_0-ik}{k_0+ik}=Se^{ika-k_0a}\\
1+R\frac{k_0+ik}{k_0-ik}=Se^{ika+k_0a}
\end{cases}
\\&\begin{cases}
透射系数：T_r=|S|^2=\frac{4k_0^2k^2}{(k^2+k_0^2)^2\sinh^2(k_0a)+4k_0^2k^2}\\
反射系数：R_e=|R|^2=\frac{(k^2+k_0^2)^2\sinh^2(k_0a)}{(k^2+k_0^2)^2\sinh^2(k_0a)+4k_0^2k^2}
\end{cases}
\\&\begin{cases}趋肤效应：a\Rightarrow \infty,S=0,R=1,定义趋肤深度\frac{|\psi(d)|^2}{|\psi(0)|^2}=\frac{1}{e},有d=\frac{1}{2g}=\frac{\hbar}{2\sqrt{2m(V_0-E)}}
\\共振穿透：S=1,R=0,粒子能量符合势垒虚能级形成驻波共振，完全穿透而不损失能量

\\隧穿效应：粒子能穿透比它动能更高的势垒.实例：\alpha衰变，热核聚变，STM.\end{cases}

\\E>V_0>0：&势垒散射，\psi_{II}=Ae^{igx}+Be^{-igx}(0<x<a),
\\&\begin{cases}
透射系数：T_r=\frac{|S|^2}{|D|^2}=\frac{4k_0^2k^2}{(k^2-k_0^2)^2\sin^2(k_0a)+4k_0^2k^2}\\
反射系数：R_e=\frac{|R|^2}{|D|^2}=\frac{(k^2-k_0^2)^2\sin^2(k_0a)}{(k^2-k_0^2)^2\sin^2(k_0a)+4k_0^2k^2}
\end{cases}



\end{align}
$$

### 

$$
\begin{align} &能量 E 的粒子正方向射向方势阱 ：V(x)=\left\{\begin{array}{lc}{V_{0} }&{ -a<x<a}\\{0 }&x<-a或x>a
\end{array}\right.
\\&k^2=\frac{2mE}{\hbar^2},k_0^2=\frac{2m}{\hbar^2}(V_0-E),

\\V_0<E<0：&势阱束缚,\left\{\begin{array}{lc}
\psi_I=Ae^{-kx}&x>a\\
\psi_{II}=C\sin k_0x+D\cos k_0 x&-a<x<a
\\\psi_{III}=Be^{kx}&{x<-a}\end{array}\right.
\\&\begin{cases}
偶宇称态\psi(x)=\left\{\begin{array}{lc}
Ae^{-kx}&x>a\\
D\cos k_0 x&0<x<a
\\\psi(-x)&{x<0}\end{array}\right.利用边界条件得\begin{cases}
k=k_0\tan(k_0a)\\
k^2+k_0^2=\frac{2mV_0}{\hbar^2}
\end{cases}
\\
奇宇称态\psi(x)=\left\{\begin{array}{lc}
Ae^{-kx}&x>a\\
C\sin k_0 x&0<x<a
\\-\psi(-x)&{x<0}\end{array}\right.利用边界条件得\begin{cases}
-k=k_0\cot(k_0a)\\
k^2+k_0^2=\frac{2mV_0}{\hbar^2}
\end{cases}
\\利用k与k_0方程组关系可计算D、F。至少存在一个偶宇称基态
\end{cases}
\\V_0<0<E：&势阱散射,\left\{\begin{array}{lc}
\psi_I=Ae^{-ikx}+Be^{-ikx}&x<-a\\
\psi_{II}=C\sin k_0x+D\cos k_0 x&-a<x<a
\\\psi_{III}=Ee^{ikx}&{x>a}\end{array}\right.
\\&利用边界条件可计算散射系数和透射系数，以及共振透射条件


\end{align}
$$

