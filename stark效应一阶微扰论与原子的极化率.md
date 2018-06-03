前一段时间,有朋友问怎样估计一个原子的极化率或者介电常数,我马上意识到这就是熟悉的stark效应,可以算作一道量子力学的微扰论的习题了.

首先,极化是指,原先呈现电中性的系统,例如一个处于基态的氢原子,在外场的作用下,正负电荷的中心发生偏离,系统被诱导出一个偶极矩的过程,其中,在外场为微扰的情况下,可看做是材料对外场的**线性**的响应,也就是说,精确到第一阶,有

![\mathbf{P}=\chi \mathbf{E} +\mathcal{O}(\mathbf{|E|}^2)](https://www.zhihu.com/equation?tex=%5Cmathbf%7BP%7D%3D%5Cchi+%5Cmathbf%7BE%7D+%2B%5Cmathcal%7BO%7D%28%5Cmathbf%7B%7CE%7C%7D%5E2%29)

在一般的线性介质中, ![\chi](https://www.zhihu.com/equation?tex=%5Cchi) 是一个张量,而在各向同性的系统中, ![\chi](https://www.zhihu.com/equation?tex=%5Cchi) 就是一个标量,称为极化率.

对于一个氢原子系统来说,在外加静电场的作用下,本征态发生的微扰叫做stark效应.发生stark效应后,氢原子的基态就带有了极性,也就是说,它被诱导产生了一个不为零的偶极矩,

所以我们就可以用量子力学中的微扰论来计算这个偶极矩的大小,从而计算出极化率.

------

## **一阶微扰论:**

在量子力学中,如果哈密顿受到修正 ,![\lambda](https://www.zhihu.com/equation?tex=%5Clambda) 为一个耦合常数,是小量

![H(\lambda)=H+\lambda V](https://www.zhihu.com/equation?tex=H%28%5Clambda%29%3DH%2B%5Clambda+V)

则,**基态**的本征值和本征函数都会受到扰动,扰动的强度由 ![\lambda](https://www.zhihu.com/equation?tex=%5Clambda) 决定

![H\psi=E\psi\to H(\lambda)\psi(\lambda)=E(\lambda)\psi(\lambda)](https://www.zhihu.com/equation?tex=H%5Cpsi%3DE%5Cpsi%5Cto+H%28%5Clambda%29%5Cpsi%28%5Clambda%29%3DE%28%5Clambda%29%5Cpsi%28%5Clambda%29)

两边同时展开到 ![\lambda](https://www.zhihu.com/equation?tex=%5Clambda) 的一阶项得到

![(H+\lambda V)(\psi+\lambda\psi^{(1)}+\mathcal{O}(\lambda^2))=(E+\lambda E^{(1)}+\mathcal{O}(\lambda^2))(\psi+\lambda\psi^{(1)}+\mathcal{O}(\lambda^2))](https://www.zhihu.com/equation?tex=%28H%2B%5Clambda+V%29%28%5Cpsi%2B%5Clambda%5Cpsi%5E%7B%281%29%7D%2B%5Cmathcal%7BO%7D%28%5Clambda%5E2%29%29%3D%28E%2B%5Clambda+E%5E%7B%281%29%7D%2B%5Cmathcal%7BO%7D%28%5Clambda%5E2%29%29%28%5Cpsi%2B%5Clambda%5Cpsi%5E%7B%281%29%7D%2B%5Cmathcal%7BO%7D%28%5Clambda%5E2%29%29)

对比系数得到

![V\psi+H\psi^{(1)}=E\psi^{(1)}+E^{(1)}\psi](https://www.zhihu.com/equation?tex=V%5Cpsi%2BH%5Cpsi%5E%7B%281%29%7D%3DE%5Cpsi%5E%7B%281%29%7D%2BE%5E%7B%281%29%7D%5Cpsi)

而由Hellmann–Feynman 定理

![E^{(1)}=\frac{\partial E(\lambda)}{\partial\lambda}=\langle\psi|\frac{\partial H(\lambda)}{\partial \lambda}|\psi\rangle=\langle\psi|V|\psi\rangle](https://www.zhihu.com/equation?tex=E%5E%7B%281%29%7D%3D%5Cfrac%7B%5Cpartial+E%28%5Clambda%29%7D%7B%5Cpartial%5Clambda%7D%3D%5Clangle%5Cpsi%7C%5Cfrac%7B%5Cpartial+H%28%5Clambda%29%7D%7B%5Cpartial+%5Clambda%7D%7C%5Cpsi%5Crangle%3D%5Clangle%5Cpsi%7CV%7C%5Cpsi%5Crangle)

所以只需要解方程

![(E-H)\psi^{(1)}=(V-E^{(1)})\psi](https://www.zhihu.com/equation?tex=%28E-H%29%5Cpsi%5E%7B%281%29%7D%3D%28V-E%5E%7B%281%29%7D%29%5Cpsi)

就可得到 ![\psi^{(1)}](https://www.zhihu.com/equation?tex=%5Cpsi%5E%7B%281%29%7D)

**这里要注意,这是一个非齐次的线性偏微分方程, ![\psi^{(1)}](https://www.zhihu.com/equation?tex=%5Cpsi%5E%7B%281%29%7D)具有一个自由性,可以相差一个齐次方程的解** **,但是,若将微扰后的波函数作归一化的约束:**

![\langle\psi|\psi\rangle=1;\langle\psi+\lambda\psi^{(1)}|\psi+\lambda\psi^{(1)}\rangle +\mathcal{O}(\lambda^2)=1 \implies \langle\psi|\psi^{(1)}\rangle=0](https://www.zhihu.com/equation?tex=%5Clangle%5Cpsi%7C%5Cpsi%5Crangle%3D1%3B%5Clangle%5Cpsi%2B%5Clambda%5Cpsi%5E%7B%281%29%7D%7C%5Cpsi%2B%5Clambda%5Cpsi%5E%7B%281%29%7D%5Crangle+%2B%5Cmathcal%7BO%7D%28%5Clambda%5E2%29%3D1+%5Cimplies+%5Clangle%5Cpsi%7C%5Cpsi%5E%7B%281%29%7D%5Crangle%3D0)

**则方程的解就是唯一的.**

根据偶极矩的定义

![\mathbf{P}=\int\rho(\mathbf{r})\mathbf {r}d^3\mathbf{r}=-e\langle\psi(\lambda)|\mathbf{r}|\psi(\lambda)\rangle=-\lambda\cdot2e\langle\psi|\mathbf{r}|\psi^{(1)}\rangle+\mathcal{O}(\lambda^2)](https://www.zhihu.com/equation?tex=%5Cmathbf%7BP%7D%3D%5Cint%5Crho%28%5Cmathbf%7Br%7D%29%5Cmathbf+%7Br%7Dd%5E3%5Cmathbf%7Br%7D%3D-e%5Clangle%5Cpsi%28%5Clambda%29%7C%5Cmathbf%7Br%7D%7C%5Cpsi%28%5Clambda%29%5Crangle%3D-%5Clambda%5Ccdot2e%5Clangle%5Cpsi%7C%5Cmathbf%7Br%7D%7C%5Cpsi%5E%7B%281%29%7D%5Crangle%2B%5Cmathcal%7BO%7D%28%5Clambda%5E2%29)

注意到,由于氢原子基态的对称性,零级微扰必然为零.

------

## **求解微扰方程**

在数学物理中,格林函数法在是处理非齐次方程的直接解法.

对于非齐次方程

![(E-H)\psi^{(1)}=(V-E^{(1)})\psi](https://www.zhihu.com/equation?tex=%28E-H%29%5Cpsi%5E%7B%281%29%7D%3D%28V-E%5E%7B%281%29%7D%29%5Cpsi)

定义**广义**格林算符为:

![G(E)=\sum_{\{n\neq1,l,m\}} \frac{|{n,l,m}\rangle\langle n,l,m|}{E-E_n+i\epsilon}- |\psi\rangle\langle\psi|](https://www.zhihu.com/equation?tex=G%28E%29%3D%5Csum_%7B%5C%7Bn%5Cneq1%2Cl%2Cm%5C%7D%7D+%5Cfrac%7B%7C%7Bn%2Cl%2Cm%7D%5Crangle%5Clangle+n%2Cl%2Cm%7C%7D%7BE-E_n%2Bi%5Cepsilon%7D-+%7C%5Cpsi%5Crangle%5Clangle%5Cpsi%7C)

其中, ![\psi:=|1,0,0\rangle](https://www.zhihu.com/equation?tex=%5Cpsi%3A%3D%7C1%2C0%2C0%5Crangle) 是系统的基态, ![E=E_1](https://www.zhihu.com/equation?tex=E%3DE_1)

可以形式化的表示出方程的一个**特解**,

![\psi^{(1)}=G(E)(V-E^{(1)})\psi](https://www.zhihu.com/equation?tex=%5Cpsi%5E%7B%281%29%7D%3DG%28E%29%28V-E%5E%7B%281%29%7D%29%5Cpsi)

在约束条件 ![\langle\psi|\psi^{(1)}\rangle=0](https://www.zhihu.com/equation?tex=%5Clangle%5Cpsi%7C%5Cpsi%5E%7B%281%29%7D%5Crangle%3D0) ,之下,这也唯一解

![\begin{eqnarray}\psi^{(1)}(\mathbf{r})=&\sum_{n\neq1}\frac{1}{E-E_n} \sum_l \sum_{m=-l}^l\psi_{n,l,m}(\mathbf{r})\int_{ \mathbb{R}^3}\psi_{n,l,m}^*(\mathbf{r}')V(\mathbf{r'})\psi_{100}(\mathbf{r'})d^3\mathbf{r'} \end{eqnarray}](https://www.zhihu.com/equation?tex=%5Cbegin%7Beqnarray%7D%5Cpsi%5E%7B%281%29%7D%28%5Cmathbf%7Br%7D%29%3D%26%5Csum_%7Bn%5Cneq1%7D%5Cfrac%7B1%7D%7BE-E_n%7D+%5Csum_l+%5Csum_%7Bm%3D-l%7D%5El%5Cpsi_%7Bn%2Cl%2Cm%7D%28%5Cmathbf%7Br%7D%29%5Cint_%7B+%5Cmathbb%7BR%7D%5E3%7D%5Cpsi_%7Bn%2Cl%2Cm%7D%5E%2A%28%5Cmathbf%7Br%7D%27%29V%28%5Cmathbf%7Br%27%7D%29%5Cpsi_%7B100%7D%28%5Cmathbf%7Br%27%7D%29d%5E3%5Cmathbf%7Br%27%7D+%5Cend%7Beqnarray%7D)

在本问题中,受到外场作用,势能的微扰为:

![\lambda V=e\mathbf{E\cdot r}](https://www.zhihu.com/equation?tex=%5Clambda+V%3De%5Cmathbf%7BE%5Ccdot+r%7D)

其中, ![\mathbf{E}](https://www.zhihu.com/equation?tex=%5Cmathbf%7BE%7D) 为外加的电场,

我们知道,基态时,系统的能量为

![E=E_1=-\frac{e^2}{2\rho_0}](https://www.zhihu.com/equation?tex=E%3DE_1%3D-%5Cfrac%7Be%5E2%7D%7B2%5Crho_0%7D) ,其中, ![\rho_0=\frac{\hbar^2}{\mu e^2}](https://www.zhihu.com/equation?tex=%5Crho_0%3D%5Cfrac%7B%5Chbar%5E2%7D%7B%5Cmu+e%5E2%7D) 为Bohr 半径.

所以可以用 ![\lambda=\frac{e\rho_0\mathbf{|E|}}{2E}=\frac{\rho_0^2}{e}\mathbf{|E|}](https://www.zhihu.com/equation?tex=%5Clambda%3D%5Cfrac%7Be%5Crho_0%5Cmathbf%7B%7CE%7C%7D%7D%7B2E%7D%3D%5Cfrac%7B%5Crho_0%5E2%7D%7Be%7D%5Cmathbf%7B%7CE%7C%7D) 作为表征耦合强度的无量纲参数,

这样一来,![V=\frac{e^2\mathbf{E\cdot r}}{\rho_0^2|\mathbf E|}](https://www.zhihu.com/equation?tex=V%3D%5Cfrac%7Be%5E2%5Cmathbf%7BE%5Ccdot+r%7D%7D%7B%5Crho_0%5E2%7C%5Cmathbf+E%7C%7D)

我们不妨先计算一下积分

![\begin{eqnarray}\sum_{l} \sum_{m=-l}^l\psi_{n,l,m}(\mathbf r)\int_{ \mathbb{R}^3}\psi_{n,l,m}^*(\mathbf{r}')\mathbf{r'}\psi_{100}(\mathbf{r'})d^3\mathbf{r'}\\ \end{eqnarray}](https://www.zhihu.com/equation?tex=%5Cbegin%7Beqnarray%7D%5Csum_%7Bl%7D+%5Csum_%7Bm%3D-l%7D%5El%5Cpsi_%7Bn%2Cl%2Cm%7D%28%5Cmathbf+r%29%5Cint_%7B+%5Cmathbb%7BR%7D%5E3%7D%5Cpsi_%7Bn%2Cl%2Cm%7D%5E%2A%28%5Cmathbf%7Br%7D%27%29%5Cmathbf%7Br%27%7D%5Cpsi_%7B100%7D%28%5Cmathbf%7Br%27%7D%29d%5E3%5Cmathbf%7Br%27%7D%5C%5C+%5Cend%7Beqnarray%7D)

由Wigner-Eckart定理,这个积分含有不可约张量算符的矩阵元

![\langle n,l,m|\mathbf{r}|1,0,0\rangle](https://www.zhihu.com/equation?tex=%5Clangle+n%2Cl%2Cm%7C%5Cmathbf%7Br%7D%7C1%2C0%2C0%5Crangle)

所以,有"选择定则": 只有![l=1](https://www.zhihu.com/equation?tex=l%3D1) 矩阵元才不为零

所以积分为:

![\begin{align} =&\frac{1}{\sqrt{4\pi}}R_{n,1}(r)\int\sum_{m=-1}^{+1} Y_{1,m}(\mathbf n)Y_{1,m}^*(\mathbf{n}')\mathbf{n'}(\mathbf{r'})d\Omega'\int_0^\infty r'^2 dr'R_{n,1}(r')R_{1,0}(r')r'\\=&\frac{\mathbf{n}}{\sqrt{4\pi}}R_{n,1}(r)\int_0^\infty r'^2 dr'R_{n,1}(r')R_{1,0}(r')r' \end{align}](https://www.zhihu.com/equation?tex=%5Cbegin%7Balign%7D+%3D%26%5Cfrac%7B1%7D%7B%5Csqrt%7B4%5Cpi%7D%7DR_%7Bn%2C1%7D%28r%29%5Cint%5Csum_%7Bm%3D-1%7D%5E%7B%2B1%7D+Y_%7B1%2Cm%7D%28%5Cmathbf+n%29Y_%7B1%2Cm%7D%5E%2A%28%5Cmathbf%7Bn%7D%27%29%5Cmathbf%7Bn%27%7D%28%5Cmathbf%7Br%27%7D%29d%5COmega%27%5Cint_0%5E%5Cinfty+r%27%5E2+dr%27R_%7Bn%2C1%7D%28r%27%29R_%7B1%2C0%7D%28r%27%29r%27%5C%5C%3D%26%5Cfrac%7B%5Cmathbf%7Bn%7D%7D%7B%5Csqrt%7B4%5Cpi%7D%7DR_%7Bn%2C1%7D%28r%29%5Cint_0%5E%5Cinfty+r%27%5E2+dr%27R_%7Bn%2C1%7D%28r%27%29R_%7B1%2C0%7D%28r%27%29r%27+%5Cend%7Balign%7D)

其中, ![\mathbf{n}:=\frac{\mathbf{r}}{r}](https://www.zhihu.com/equation?tex=%5Cmathbf%7Bn%7D%3A%3D%5Cfrac%7B%5Cmathbf%7Br%7D%7D%7Br%7D) 为方向矢量.

所以

![\begin{eqnarray}\psi^{(1)}(\mathbf{r})=&\sum_{n\neq1}\frac{1}{E-E_n} \sum_l \sum_{m=-l}^l\psi_{n,l,m}(\mathbf{r})\int_{ \mathbb{R}^3}\psi_{n,l,m}^*(\mathbf{r}')V(\mathbf{r'})\psi_{100}(\mathbf{r'})d^3\mathbf{r'}\\=&-\frac{1}{\sqrt{4\pi}}\frac{\mathbf{n}\cdot\mathbf{E}}{|\mathbf{E}|}\sum_{n\neq1}\frac{n^2}{n^2-1} R_{n,1}(r)\int_0^\infty r'^2 dr'R_{n,1}(r')R_{1,0}(r')r' \end{eqnarray}](https://www.zhihu.com/equation?tex=%5Cbegin%7Beqnarray%7D%5Cpsi%5E%7B%281%29%7D%28%5Cmathbf%7Br%7D%29%3D%26%5Csum_%7Bn%5Cneq1%7D%5Cfrac%7B1%7D%7BE-E_n%7D+%5Csum_l+%5Csum_%7Bm%3D-l%7D%5El%5Cpsi_%7Bn%2Cl%2Cm%7D%28%5Cmathbf%7Br%7D%29%5Cint_%7B+%5Cmathbb%7BR%7D%5E3%7D%5Cpsi_%7Bn%2Cl%2Cm%7D%5E%2A%28%5Cmathbf%7Br%7D%27%29V%28%5Cmathbf%7Br%27%7D%29%5Cpsi_%7B100%7D%28%5Cmathbf%7Br%27%7D%29d%5E3%5Cmathbf%7Br%27%7D%5C%5C%3D%26-%5Cfrac%7B1%7D%7B%5Csqrt%7B4%5Cpi%7D%7D%5Cfrac%7B%5Cmathbf%7Bn%7D%5Ccdot%5Cmathbf%7BE%7D%7D%7B%7C%5Cmathbf%7BE%7D%7C%7D%5Csum_%7Bn%5Cneq1%7D%5Cfrac%7Bn%5E2%7D%7Bn%5E2-1%7D+R_%7Bn%2C1%7D%28r%29%5Cint_0%5E%5Cinfty+r%27%5E2+dr%27R_%7Bn%2C1%7D%28r%27%29R_%7B1%2C0%7D%28r%27%29r%27+%5Cend%7Beqnarray%7D)

我们发现,这里陷入了一个无穷求和的困境,

**但是我们从这个复杂的形式中看出, ![\psi^{(1)}](https://www.zhihu.com/equation?tex=%5Cpsi%5E%7B%281%29%7D) 是可以分离变数的.**

所以不妨设 ![\psi^{(1)}(\mathbf{r})=\frac{\mathbf{E\cdot n}}{|\mathbf{E}|}\cdot u(r)](https://www.zhihu.com/equation?tex=%5Cpsi%5E%7B%281%29%7D%28%5Cmathbf%7Br%7D%29%3D%5Cfrac%7B%5Cmathbf%7BE%5Ccdot+n%7D%7D%7B%7C%5Cmathbf%7BE%7D%7C%7D%5Ccdot+u%28r%29),

直接带到原方程中,分离变数法得以下径向方程,(这里进行了代换 ![r\to{\rho_0}r](https://www.zhihu.com/equation?tex=r%5Cto%7B%5Crho_0%7Dr) )

![\{-\frac{1}{r^2}\frac{d}{dr}r^2\frac{d}{dr}+\frac{2}{r^2}-\frac{2}{r}+1\}u(r)=-\frac{1}{\sqrt{\pi}}re^{-r}](https://www.zhihu.com/equation?tex=%5C%7B-%5Cfrac%7B1%7D%7Br%5E2%7D%5Cfrac%7Bd%7D%7Bdr%7Dr%5E2%5Cfrac%7Bd%7D%7Bdr%7D%2B%5Cfrac%7B2%7D%7Br%5E2%7D-%5Cfrac%7B2%7D%7Br%7D%2B1%5C%7Du%28r%29%3D-%5Cfrac%7B1%7D%7B%5Csqrt%7B%5Cpi%7D%7Dre%5E%7B-r%7D)

令![u(r)=e^{-r}\xi(r)](https://www.zhihu.com/equation?tex=u%28r%29%3De%5E%7B-r%7D%5Cxi%28r%29),则 ![\xi(r)](https://www.zhihu.com/equation?tex=%5Cxi%28r%29) 满足

![\{-\frac{1}{r^2}\frac{d}{dr}r^2\frac{d}{dr}+\frac{2}{r^2}+2\frac{d}{dr}\}\xi(r)=-\frac{1}{\sqrt{\pi}}r](https://www.zhihu.com/equation?tex=%5C%7B-%5Cfrac%7B1%7D%7Br%5E2%7D%5Cfrac%7Bd%7D%7Bdr%7Dr%5E2%5Cfrac%7Bd%7D%7Bdr%7D%2B%5Cfrac%7B2%7D%7Br%5E2%7D%2B2%5Cfrac%7Bd%7D%7Bdr%7D%5C%7D%5Cxi%28r%29%3D-%5Cfrac%7B1%7D%7B%5Csqrt%7B%5Cpi%7D%7Dr)

可考虑多项式形式的解

![\xi(r)=Ar^2+Br](https://www.zhihu.com/equation?tex=%5Cxi%28r%29%3DAr%5E2%2BBr) ,带入方程中得到

![-6A+2A+4Ar+2B=-\frac{1}{\sqrt{\pi}}r](https://www.zhihu.com/equation?tex=-6A%2B2A%2B4Ar%2B2B%3D-%5Cfrac%7B1%7D%7B%5Csqrt%7B%5Cpi%7D%7Dr)

解得 ![A=-\frac{1}{4}\frac{1}{\sqrt{\pi}},B=-\frac{1}{2}\frac{1}{\sqrt{\pi}}](https://www.zhihu.com/equation?tex=A%3D-%5Cfrac%7B1%7D%7B4%7D%5Cfrac%7B1%7D%7B%5Csqrt%7B%5Cpi%7D%7D%2CB%3D-%5Cfrac%7B1%7D%7B2%7D%5Cfrac%7B1%7D%7B%5Csqrt%7B%5Cpi%7D%7D)

恢复标度 ![r\to\frac{r}{\rho_0}](https://www.zhihu.com/equation?tex=r%5Cto%5Cfrac%7Br%7D%7B%5Crho_0%7D) 得

![\psi^{(1)}=-\frac{1}{\sqrt{\pi\rho_0^3}}(\frac{1}{2}\frac{r}{\rho_0}+\frac{1}{4}\frac{r^2}{\rho_0^2})e^{-{\frac{r}{\rho_0}}}\frac{\mathbf{E\cdot n}}{|\mathbf{E}|}](https://www.zhihu.com/equation?tex=%5Cpsi%5E%7B%281%29%7D%3D-%5Cfrac%7B1%7D%7B%5Csqrt%7B%5Cpi%5Crho_0%5E3%7D%7D%28%5Cfrac%7B1%7D%7B2%7D%5Cfrac%7Br%7D%7B%5Crho_0%7D%2B%5Cfrac%7B1%7D%7B4%7D%5Cfrac%7Br%5E2%7D%7B%5Crho_0%5E2%7D%29e%5E%7B-%7B%5Cfrac%7Br%7D%7B%5Crho_0%7D%7D%7D%5Cfrac%7B%5Cmathbf%7BE%5Ccdot+n%7D%7D%7B%7C%5Cmathbf%7BE%7D%7C%7D)

------

## **极化率的计算**

经过简单的计算可以得到

![\langle\psi|\mathbf{r}|\psi^{(1)}\rangle=-\frac{9}{4}\rho_{0}\frac{\mathbf{E}}{\mathbf{|E|}}](https://www.zhihu.com/equation?tex=%5Clangle%5Cpsi%7C%5Cmathbf%7Br%7D%7C%5Cpsi%5E%7B%281%29%7D%5Crangle%3D-%5Cfrac%7B9%7D%7B4%7D%5Crho_%7B0%7D%5Cfrac%7B%5Cmathbf%7BE%7D%7D%7B%5Cmathbf%7B%7CE%7C%7D%7D)

![\mathbf{P}=-\lambda\cdot2e\langle\psi|\mathbf{r}|\psi^{(1)}\rangle+\mathcal{O}(\lambda^2)= \frac{9}{2}\rho_0^3\mathbf{E}+\mathcal{O}(|\mathbf{E}|^2)](https://www.zhihu.com/equation?tex=%5Cmathbf%7BP%7D%3D-%5Clambda%5Ccdot2e%5Clangle%5Cpsi%7C%5Cmathbf%7Br%7D%7C%5Cpsi%5E%7B%281%29%7D%5Crangle%2B%5Cmathcal%7BO%7D%28%5Clambda%5E2%29%3D+%5Cfrac%7B9%7D%7B2%7D%5Crho_0%5E3%5Cmathbf%7BE%7D%2B%5Cmathcal%7BO%7D%28%7C%5Cmathbf%7BE%7D%7C%5E2%29)

所以

![\mathbf{P}= \frac{9}{2}\rho_0^3\mathbf{E}+\mathcal{O}(|\mathbf{E}|^2)](https://www.zhihu.com/equation?tex=%5Cmathbf%7BP%7D%3D+%5Cfrac%7B9%7D%7B2%7D%5Crho_0%5E3%5Cmathbf%7BE%7D%2B%5Cmathcal%7BO%7D%28%7C%5Cmathbf%7BE%7D%7C%5E2%29)

所以氢原子基态的极化率为

![\chi=\frac{9\rho_0^3}{2}](https://www.zhihu.com/equation?tex=%5Cchi%3D%5Cfrac%7B9%5Crho_0%5E3%7D%7B2%7D)