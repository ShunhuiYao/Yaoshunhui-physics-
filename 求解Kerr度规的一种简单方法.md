我们将用一种特殊的参数化方法求解一类Einstein方程的真空解,其中,我们会将Kerr解和schwarzschild解用统一的参数化方法表示出来。
基本假设

g_{\mu\nu}=\eta_{\mu\nu}-2ml_{\mu}l_\nu 
其中， \eta_{\mu\nu}=diag\{1,-1,-1,-1\} 是平直的时空背景， m 为一个实参数
而 l_{\mu} 时空中的一个类光向量场，其满足
l_{\nu}l_{\mu}\eta^{\mu\nu}=0 
我们的基本假设仅仅是
R_{\mu\nu}(\mathbf x,m)=0 对于任意的 m 恒成立，也就是说,我们要求解的是一个用参数 m 标记的解族。所以只需要将Ricci 张量展开为关于 m 的多项式函数，令每一阶的系数都为零就可以了。
首先，可以证明度规的逆变张量 g^{\mu\nu}=\eta^{\mu\nu}+2ml^\mu l^\nu 
注意其中，我们定义 l^\mu \equiv\eta^{\mu\nu}l_\nu 
不过，也可以证明， l^\mu=(g^{\mu\nu}-2ml^\mu l^\nu)l_\nu=g^{\mu\nu}l_\nu 
所以在这种定义之下， l_\mu 在弯曲时空中也是类光矢量场，也就是说我们的构造是自洽的。
下面来计算Ricci张量的分量
化简场方程

先计算联络系数：
\Gamma^{i}_{jk}= -2m\{l^i\partial_{(j}l_{k)}+l_{(k}\partial_{j)}l^i-l_{(j}\partial^il_{k)}\}+2m^2\{l^il^\rho\partial_\rho(l_jl_k)\} 
根据Ricci张量的定义列出Einstein方程
0=R_{\mu\nu}=-\partial_\mu\partial_\nu\log\sqrt{-g}+\Gamma^{i}_{\mu\nu}\partial_i\log\sqrt{-g}+\partial_i\Gamma^i_{\mu\nu}-\Gamma^i_{\mu j}\Gamma^j_{\nu i} 
易知： \partial_i\log\sqrt{-g}=0，所以可以化简得
\partial_i\Gamma^i_{jk}=\Gamma^i_{j \rho}\Gamma^{\rho}_{k i}
依照假设，我们可以两边按照 m 的幂次展开，各阶展开系数对应相等：
\mathcal O(m) :
\partial_i\{l^i\partial_{(j}l_{k)}+l_{(k}\partial_{j)}l^i-l_{(j}\partial^il_{k)}\}=0 
\mathcal O(m^2) :
\begin{align} &\partial_i\{l^il^\rho\partial_\rho(l_jl_k)\}\\=&2\{l^i\partial_{(j}l_{\rho)}+l_{(j}\partial_{\rho)}l^i-l_{(j}\partial^il_{\rho)}\}\{l^\rho\partial_{(k}l_{i)}+l_{(k}\partial_{i)}l^\rho-l_{(k}\partial^\rho l_{i)}\}\end{align} 
\mathcal O(m^3) :
\{l^il^\sigma\partial_\sigma(l_jl_\rho)\}\{l^\rho\partial_{(k}l_{i)}+l_{(k}\partial_{i)}l^\rho-l_{(k}\partial^\rho l_{i)}\}+(j\leftrightarrow k)=0 
\mathcal O(m^4):
\{l^il^\sigma\partial_\sigma(l_jl_\rho)\}\{l^\rho l^\sigma\partial_\sigma(l_kl_i)\}=0 
我们发现， \mathcal O(m^4) 是个恒等式，所以只需要考虑前三个方程就可以了
为了化简这些方程，我们定义：
-\nabla_\mu l^\mu= \ell=-\partial_\mu l^\mu ; 
l^\beta\nabla_\beta l^\alpha=l^\beta\partial_\beta l^\alpha=\mathcal A ^\alpha 
易知： \mathcal A_\mathcal \alpha A^\alpha=0, \mathcal A^\alpha l_\alpha=0
可以推出 \mathcal A\parallel l 
所以可以定义标量场 \mathcal D 
-l^\beta\nabla_\beta l^\alpha=-l^\beta\partial_\beta l^\alpha=\mathcal D l^\alpha 
从而易看出 \mathcal O(m^3) 也是一个恒等式
因而可以化简原方程组为
\mathcal O(m): 
-\square( l_{j}l_k)=\partial_j(\ell+\mathcal D)l_k+\partial_k(\ell+\mathcal D)l_j 
当 l^\mu 满足 \mathcal O(m) 阶的方程时， O(m^2) 阶方程是自动成立的
LHS=(2\mathcal D\ell-2l^\mu\partial_\mu\mathcal D+4\mathcal D^2)l_jl_k 
RHS=\{3\mathcal D^2+(\partial^\rho l^i )\partial_i l_\rho+l^\rho\square l_\rho)\}l_jl_k 
我们可以同时用 l^j 和 \mathcal O(m) 方程的两边进行缩并，得到：
l^\rho\square l_\rho= -l^\mu\partial_\mu(\ell+\mathcal D)+(\ell+\mathcal D)\mathcal D 
又因为
(\partial^\rho l^i )\partial_i l_\rho=-\partial_\mu(\mathcal D l^\mu)+l^\mu\partial_\mu\ell=l^\mu\partial_\mu(\ell-\mathcal D)+\mathcal D\ell 
所以自然可以得到
RHS=LHS 
所以我们惊喜地发现，对于这类特殊的度规
 g_{\mu\nu}=\eta_{\mu\nu}-2ml_\mu l_\nu 
只需要将场方程方程 R_{\mu\nu}(\mathbf x,m)=0 展开到 m 的一阶，就可以保证以后各阶的方程都自动地成立。 

而一阶的方程是如下的波动方程：
-\square( l_{j}l_k)=\partial_j(\ell+\mathcal D)l_k+\partial_k(\ell+\mathcal D)l_j
波动方程的稳态解

我们要求引力场是稳态的，所以 l^\mu 不显含时间，所以方程可以化简为三维空间中的Laplace型方程。
\Delta(l_j l_k)=\partial_j(\ell+\mathcal D)l_k+\partial_k(\ell+\mathcal D)l_j （j,k=0,1,2,3） 
设 l_\mu=\lambda(1,n_1,n_2,n_3)，其中 \overset{\rightharpoonup}{n} 为单位矢量， \lambda 为标量
则原方程等价于方程组：
\Delta(\lambda^2)=0 
\Delta(\lambda^2 n_j)= \partial_j(\lambda\ell+\lambda\mathcal D) 
\Delta(\lambda^2n_jn_k)=\partial_j\{(\ell+\mathcal D)\lambda n_k\}+\partial_k\{(\ell+\mathcal D)\lambda n_j\} ， j,k=1,2,3 
最后一个方程可以用前两个方程化简为：
\lambda\nabla n_j\cdot\nabla n_k=(\ell+\mathcal D)\partial_{(j}n_{k)} 
定义 M_{ij}=\partial_jn_i, p=\frac{2\lambda}{\ell+\mathcal D} 则：
 pMM^T=M+M^T 
这里用一个因式分解的Trick:
(1-pM)(1-pM^T)=1 
这说明， U=1-pM 满足 UU^T=U^TU=1 ,即， U\in O(3) 
在群论中，我们知道，三维空间的转动群中的任何一个元素必然可以写成绕着一个轴转动的形式，其中，转动轴就是本征值 1 对应的本征矢量方向，
我们又发现
U\mathbf n =\mathbf n 
所以转动轴恰好就是 \mathbf n，又设转动角度为 \chi 
由定轴转动的Rodrigues公式，可以用 (\mathbf n,\chi) 两个参数来重写转动矩阵
U_{ij}=\cos\chi\delta_{ij}+(1-\cos\chi)n_{i}n{_j}+\sin\chi\epsilon_{\alpha ji}n_\alpha (对重复指标求和)
所以
\partial_in_j=\frac{1}{p}(1-\cos\chi)(\delta_{ij}-n_in_j)-\frac{1}{p}\sin\chi\varepsilon_{\alpha ij}n_\alpha 
我们还可以更为简单地参数化上面的表达式
\partial_in_j=\alpha(\delta_{ij}-n_in_j)-\beta\varepsilon_{ijk}n_k 
其中， \alpha=\frac{\ell+\mathcal D}{2\lambda}(1-\cos\chi);\beta=\frac{\ell+\mathcal D}{2\lambda}(\sin\chi) 
两边同时对 i,j 缩并得
\mathbf{div}n=2\alpha 
两边同时斜对称化得
\mathbf{curl} \ \mathbf n=-2\beta\mathbf n 
又由同时缩并以 \partial_i,并利用  \mathbf n\cdot\nabla\mathbf n=0知
\Delta\mathbf n=\nabla\alpha-2(\alpha^2+\beta^2)\mathbf n-\mathbf {(n}\cdot\nabla\alpha)\mathbf n+\nabla\beta\times\mathbf n 
又因为： \nabla\times(\nabla\times\mathbf n)=\nabla(\nabla\cdot\mathbf n)-\Delta\mathbf n 故：
\Delta \mathbf n=\nabla\times(2\beta\mathbf n)+\nabla(2\alpha)=-4\beta^2\mathbf n+2\nabla\beta\times\mathbf n+2\nabla\alpha 
两个式子对比得
\nabla\alpha=-\nabla\beta\times\mathbf n-2(\alpha^2-\beta^2)\mathbf n-(\mathbf n\cdot\nabla\alpha)\mathbf n
\mathbf n\cdot\nabla\alpha=\beta^2-\alpha^2
\nabla\alpha=\mathbf n\times\nabla\beta+(\beta^2-\alpha^2)\mathbf n 
两边同时用 \mathbf n 叉乘得
\nabla\beta=-\mathbf n\times \nabla\alpha+(\mathbf n\cdot\nabla\beta)\mathbf n 
又因为
\mathbf{curl} \ \mathbf n=-2\beta\mathbf n
\nabla\beta\cdot\mathbf n=-2\alpha\beta 
整理得：
\nabla\beta=-\mathbf n\times \nabla\alpha-2\alpha\beta\mathbf n\\ \nabla\alpha=\mathbf n\times\nabla\beta+(\beta^2-\alpha^2)\mathbf n 
我们引入一个复变量
\gamma:=\alpha+i\beta ，并定义： \gamma^{-1}:=\omega 
则有
\nabla\gamma=-i\mathbf n\times\nabla\gamma-\gamma^2\mathbf n 
所以
\begin{align}\Delta\gamma=&2i\beta\mathbf n\cdot\nabla\gamma-2\gamma\nabla\gamma\cdot\mathbf n-2\alpha\gamma^2=2\gamma^3-2\gamma^3=0 \end{align} 
(\nabla\omega)^2=1 
提取出 l_\mu 的解

我们将证明，上面的两个方程可以完全地代替原来的波动方程，也就是只要根据边界条件定出 \gamma 和 \omega 
就可以完全地定出波动方程的解 l_\mu=\lambda(1,\mathbf n) 来
首先
\nabla\omega=-i\mathbf n\times\nabla\omega+\mathbf n 
而
\nabla\omega\times\nabla\omega^*=i(1+\nabla\omega\cdot\nabla\omega^*)\mathbf n-i(\nabla\omega+\nabla\omega^*) 
所以
\mathbf n=\frac{\nabla\omega+\nabla\omega^*-i\nabla\omega\times\nabla\omega^*}{1+\nabla\omega\cdot\nabla\omega^*} 
下面证明, \lambda^2=\alpha 是 l_\mu标量部分的解
只需要证明
\Delta\lambda^2=\Delta\alpha=\Delta\gamma=0
\Delta(\alpha n_j)=\partial_j(\lambda\ell+\lambda\mathcal D)
 第一个式子不言自明，主要证明第二个式子
\Delta(\lambda^2 n_j)=\Delta(\alpha n_j)=2\nabla\alpha\cdot\nabla n_j+\alpha\Delta n_j 
根据上面的推导，可以知道
\Delta n_j=-2(\alpha^2+\beta^2) n_j 
2\nabla\alpha\cdot\nabla n_j=\partial_j(\alpha^2+\beta^2)+2\alpha(\beta^2+\alpha^2)n_j
所以
\Delta(\alpha n_j)=\partial_j(\alpha^2+\beta^2) 
又因为： \alpha^2+\beta^2=\frac{(\ell+\mathcal D)^2}{2\lambda^2}(1-\cos\chi)=\frac{\ell+\mathcal D}{\lambda}\alpha=\lambda\ell+\lambda\mathcal D
这样就证明了 \lambda=\sqrt{\alpha}给出了解的标量部分
schwarzschild解


根据上面的论述，场方程等价于求解一个Laplace方程
\Delta\gamma=0 \quad (\nabla\omega)^2=1 
考虑一个最简单的球对称基本解
\gamma=(x^2+y^2+z^2)^{-\frac{1}{2}} 
从而定出
\mathbf{n}=(\frac{x}{r},\frac{y}{r},\frac{z}{r}) , \lambda=\frac{1}{\sqrt r} 
故场方程的一个球对称解为
ds^2=(dx^0)^2-dx^2-dy^2-dz^2-\frac{2m}{r}(dx^0+\frac{x}{r}dx+\frac{y}{r}dy +\frac{z}{r}dz)^2 
 x=r\sin\theta\cos\varphi ,y=r\sin\theta\cos\varphi ,z=r\cos\theta 
则
ds^2=(1-\frac{2m}{r})(dx^0)^2-(1+\frac{2m}{r})dr^2-\frac{4m}{r}drdx^0-r^2d\Omega^2 
这就是用Eddington坐标描述的schwarzschild解
进一步地，令
t=x^0-2m\log(|\frac{r}{2m}-1|) 既可以得到schwarzschild度规
ds^2=(1-\frac{2m}{r})dt^2-(1-\frac{2m}{r})^{-1}dr^2-r^2d\Omega^2 
从schwarzschild解到Kerr解

仿照上面的解法，我们发现，只需要对点源的 \gamma 进行虚平移就可以得到轴对称的调和函数解 \gamma 
即
\gamma\to(x^2+y^2+(z-ia)^2)^{-\frac{1}{2}}
其中 a 为一个实参数
很容易看出，这样的平移后， \gamma 仍是Laplace方程的解
定义椭球坐标(\rho,\sigma)： 
\omega=(r^2-a^2-2iaz)^\frac{1}{2}=\rho+i\sigma 
可以证明 \rho 满足
\frac{x^2}{\rho^2+a^2}+\frac{y^2}{\rho^2+a^2}+\frac{z^2}{\rho^2}=1 , \sigma=\frac{-az}{\rho} 
则此时，
\gamma=\frac{\rho-i\sigma}{\rho^2+\sigma^2} 
\nabla\omega=\frac{\mathbf r-ia\mathbf e_z}{\omega} 
\mathbf n=\frac{\rho\mathbf{r-a\sigma\mathbf{e_z}}+ay\mathbf e_x-ax\mathbf e_y}{a^2+\rho^2} 
这样我们就得到了轴对称的线元
ds^2=(dx^0)^2-dx^2-dy^2-dz^2-\frac{2m\rho^3}{\rho^4+z^2a^2}(dx^0+\frac{\rho xdx+\rho ydy}{a^2+\rho^2}+\frac{ aydx-axdy}{\rho^2+a^2}+\frac{zdz}{\rho})^2\\ 定义极坐标 (\theta,\varphi) 
\cos\theta=\frac{z}{\rho}\quad x+iy=(\rho-ia)e^{i\varphi}\sin\theta 
并且定义 u=x^0+\rho 
则度规可以写为
ds^2=(1-\frac{2m\rho}{\rho^2+a^2\cos^2\theta})du^2-(\rho^2+a^2\cos^2\theta)d\theta^2\\-[(\rho^2+a^2)\sin^2\theta+\frac{2m\rho a^2\sin^4\theta}{\rho^2+a^2\cos^2\theta}]d\varphi^2-2dud\rho-\\-\frac{4m\rho a\sin^2\theta}{\rho^2+a^2\cos^2\theta}dud\varphi-2a\sin^2\theta d\rho d\varphi 
可以通过坐标变换重新定义角度和时间参数
t=u-A(\rho)\quad \varphi'=\varphi-B(\rho) 
便可以消去交叉项 dud\rho \quad d\varphi d\rho 
得到Kerr度规为：
ds^2=(1-\frac{2m\rho}{\rho^2+a^2\cos^2\theta})dt^2-(\rho^2+a^2\cos^2\theta)d\theta^2\\-\frac{\rho^2+a^2\cos^2\theta}{\rho^2+a^2-2m\rho}d\rho^2-[(\rho^2+a^2)\sin^2\theta+\frac{2m\rho a^2\sin^4\theta}{\rho^2+a^2\cos^2\theta}]d\varphi^2\\-\frac{4m\rho a\sin^2\theta}{\rho^2+a^2\cos^2\theta}dtd\varphi 
参考文献
[1]Introduction to General Relativity ,  Ronald B. Adler 


















