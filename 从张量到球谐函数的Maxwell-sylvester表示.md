**直观的说,球谐函数就是不可约张量的单指标记法,不可约张量的独立分量和球谐函数是对应的**

接下来讨论的就是从表示论的出发建立球谐函数与张量之间的对应关系,同时介绍一种借助张量的分量直接得到球谐函数的表达式的方法.

## **1.从调和函数到转动群的不可约表示**

比较了诸多的资料,对于得到SO(3)的不可约表示,有三种不同的但是殊途同归的切入方式

来源于调和函数. 我们知道,调和函数空间可以荷载转动群的表示,因为调和函数张成的空间在转动群作用下是封闭的. 其中 ![l](https://www.zhihu.com/equation?tex=l) 次的齐次调和多项式空间(下面记为 ![V_l](https://www.zhihu.com/equation?tex=V_l) )正是转动群的 ![2l+1](https://www.zhihu.com/equation?tex=2l%2B1) 维不可约表示空间.

> **![l](https://www.zhihu.com/equation?tex=l) 次的齐次调和多项式空间(下面记为 ![V_l](https://www.zhihu.com/equation?tex=V_l) )的维数为 ![2l+1](https://www.zhihu.com/equation?tex=2l%2B1)** ![\mathbb{P}_l=span\langle x^iy^jz^k|i+j+k=l;i,j,l\in\mathbb{N}\rangle](https://www.zhihu.com/equation?tex=%5Cmathbb%7BP%7D_l%3Dspan%5Clangle+x%5Eiy%5Ejz%5Ek%7Ci%2Bj%2Bk%3Dl%3Bi%2Cj%2Cl%5Cin%5Cmathbb%7BN%7D%5Crangle) 为 ![l](https://www.zhihu.com/equation?tex=l) 次齐次多项式空间
> 容易知道其维数为 ![{l+3-1\choose3-1}={l+2\choose2}](https://www.zhihu.com/equation?tex=%7Bl%2B3-1%5Cchoose3-1%7D%3D%7Bl%2B2%5Cchoose2%7D) 
> 考虑线性映射 ![\Delta:\mathbb{P}_l\to\mathbb{P}_{l-2}](https://www.zhihu.com/equation?tex=%5CDelta%3A%5Cmathbb%7BP%7D_l%5Cto%5Cmathbb%7BP%7D_%7Bl-2%7D) 其中 ![\Delta](https://www.zhihu.com/equation?tex=%5CDelta) 为Laplace算符,
> 这个映射显然是一个满射,所以核空间即 ![V_l](https://www.zhihu.com/equation?tex=V_l) 的维数为 ![{\rm dim V}_l={l+2\choose 2}-{l\choose2}=2l+1](https://www.zhihu.com/equation?tex=%7B%5Crm+dim+V%7D_l%3D%7Bl%2B2%5Cchoose+2%7D-%7Bl%5Cchoose2%7D%3D2l%2B1)

我们也知道, ![l](https://www.zhihu.com/equation?tex=l) 阶的球谐多项式 ![r^lY_{lm}](https://www.zhihu.com/equation?tex=r%5ElY_%7Blm%7D) 共有 ![2l+1](https://www.zhihu.com/equation?tex=2l%2B1) 个, 易验证他们都是调和多项式,且线性无关,

**所以 ![l](https://www.zhihu.com/equation?tex=l) 阶的球谐多项式 ![r^lY_{lm}](https://www.zhihu.com/equation?tex=r%5ElY_%7Blm%7D) 就是 ![V_l](https://www.zhihu.com/equation?tex=V_l) 的一组正交的完备基底.** 使用这组基底,就能构造出转动群的 ![2l+1](https://www.zhihu.com/equation?tex=2l%2B1) 维的不可约酉表示.

从反方向说,使用另外的一组调和多项式基,例如 ![l=2](https://www.zhihu.com/equation?tex=l%3D2) 时, ![\{ xy,yz,xz,x^2-y^2,y^2-z^2\}](https://www.zhihu.com/equation?tex=%5C%7B+xy%2Cyz%2Cxz%2Cx%5E2-y%5E2%2Cy%5E2-z%5E2%5C%7D) ,这些简单的齐次调和多项式基底和球谐多项式基底是等价的,可以做一些线性组合去构造出想要的球谐多项式,这一点十分关键.

## **2.用商表示作为转动群的不可约表示**

上面所说,通过调和多项式,可以得到转动群的不可约表示,下面我们回顾第二种得到转动群不可约表示的方法..

首先,![l](https://www.zhihu.com/equation?tex=l)次齐次多项式空间 ![\mathbb{P}_l](https://www.zhihu.com/equation?tex=%5Cmathbb%7BP%7D_l) 也是转动群的一个表示,但是这个表示不是不可约的,因为可以用一维不可约表示 ![<x^2+y^2+z^2>](https://www.zhihu.com/equation?tex=%3Cx%5E2%2By%5E2%2Bz%5E2%3E) 与 ![\mathbb{P}_{l-2}](https://www.zhihu.com/equation?tex=%5Cmathbb%7BP%7D_%7Bl-2%7D) 的直积构成 ![\mathbb{P}_l](https://www.zhihu.com/equation?tex=%5Cmathbb%7BP%7D_l) 的一个子表示.

所以 ![\mathbb{P}_l](https://www.zhihu.com/equation?tex=%5Cmathbb%7BP%7D_l) 模掉这个子表示才是不可约表示,用多项式的语言,不可约表示是 ![\mathbb{P}_l](https://www.zhihu.com/equation?tex=%5Cmathbb%7BP%7D_l) 模去 ![<x^2+y^2+z^2>](https://www.zhihu.com/equation?tex=%3Cx%5E2%2By%5E2%2Bz%5E2%3E) 生成的理想,而最后得到的商表示的维数也是 ![dim\mathbb{P}_l-dim\mathbb{P}_{l-2}=2l+1](https://www.zhihu.com/equation?tex=dim%5Cmathbb%7BP%7D_l-dim%5Cmathbb%7BP%7D_%7Bl-2%7D%3D2l%2B1)

## 3.**通过张量得到转动群的不可约表示.**

表示论中有如下的定理，如果紧致Lie群是有限维向量空间的上的线性群的一个闭子群,则它的所有不可约表示可以从基本表示的张量积约化出来.最简单的例子就是,SO(3)的基本表示是三维的,而做一次张量积后可以由如下的约化

![\mathbf{3}\otimes\mathbf{3}=\mathbf{1}\oplus\mathbf{3}\oplus\mathbf{5}](https://www.zhihu.com/equation?tex=%5Cmathbf%7B3%7D%5Cotimes%5Cmathbf%7B3%7D%3D%5Cmathbf%7B1%7D%5Coplus%5Cmathbf%7B3%7D%5Coplus%5Cmathbf%7B5%7D)

实际上,只通过全对称张量空间就可以约化出转动群的全部不可约表示了. 做法就是将张量对称无迹部分拿出来就可以了,**这部分对称无迹的张量就是所谓的不可约张量**

> 注意到一个 ![l](https://www.zhihu.com/equation?tex=l) 阶全对称张量的独立分量与 ![l](https://www.zhihu.com/equation?tex=l) 次的齐次多项式基底 ![x^jy^jz^k](https://www.zhihu.com/equation?tex=x%5Ejy%5Ejz%5Ek)是一一对应的,因为你可以用过对称性把不同的分量都给他以统一的指标排列写出来比如说对![T_{ijkl\cdots}=T_{xxxyyyzz}](https://www.zhihu.com/equation?tex=T_%7Bijkl%5Ccdots%7D%3DT_%7Bxxxyyyzz%7D)
> 可以认为下标中的字符串就是一个齐次式,所以从计数的角度说,首先,一个 ![l](https://www.zhihu.com/equation?tex=l) 阶全对称张量的独立分量个数与 ![l](https://www.zhihu.com/equation?tex=l) 次齐次多项式空间 ![\mathbb{P}_l](https://www.zhihu.com/equation?tex=%5Cmathbb%7BP%7D_l) 的维数相等,同样的,要得到无迹张量子空间,需要在对指标两两缩并,所以无迹张量子空间必然满足 ![l\choose2](https://www.zhihu.com/equation?tex=l%5Cchoose2) 个约束方程,所以全对称无迹张量子空间的维数就是 ![2l+1](https://www.zhihu.com/equation?tex=2l%2B1).

## **4.通过多Maxwell-Sylvester表示法来实现三种方式的统一**

**所谓的**Maxwell-Sylvester表示法就是在静电学中我们熟悉的多极矩展开

![\frac{1}{|\mathbf{x-x'}|}=\sum_l\frac{(-1)^l}{l!}\sum_{1\leq k_1,k_2,\cdots k_l\leq3}x'^{k_1}x'^{k_2}\cdots x'^{k_l}\partial_{k_1}\partial_{k_2}\cdots\partial_{k_l}\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cfrac%7B1%7D%7B%7C%5Cmathbf%7Bx-x%27%7D%7C%7D%3D%5Csum_l%5Cfrac%7B%28-1%29%5El%7D%7Bl%21%7D%5Csum_%7B1%5Cleq+k_1%2Ck_2%2C%5Ccdots+k_l%5Cleq3%7Dx%27%5E%7Bk_1%7Dx%27%5E%7Bk_2%7D%5Ccdots+x%27%5E%7Bk_l%7D%5Cpartial_%7Bk_1%7D%5Cpartial_%7Bk_2%7D%5Ccdots%5Cpartial_%7Bk_l%7D%5Cfrac%7B1%7D%7Br%7D)

在空间转动作用下,展开的每一项都是不变的,更具体的说

![\frac{(-1)^l}{l!}\sum_{1\leq k_1,k_2,\cdots k_l\leq3}x'^{k_1}x'^{k_2}\cdots x'^{k_l}\partial_{k_1}\partial_{k_2}\cdots\partial_{k_l}\frac{1}{r}=P_l(\langle\mathbf{n,n'}\rangle)\frac{r'^l}{r^{l+1}}](https://www.zhihu.com/equation?tex=%5Cfrac%7B%28-1%29%5El%7D%7Bl%21%7D%5Csum_%7B1%5Cleq+k_1%2Ck_2%2C%5Ccdots+k_l%5Cleq3%7Dx%27%5E%7Bk_1%7Dx%27%5E%7Bk_2%7D%5Ccdots+x%27%5E%7Bk_l%7D%5Cpartial_%7Bk_1%7D%5Cpartial_%7Bk_2%7D%5Ccdots%5Cpartial_%7Bk_l%7D%5Cfrac%7B1%7D%7Br%7D%3DP_l%28%5Clangle%5Cmathbf%7Bn%2Cn%27%7D%5Crangle%29%5Cfrac%7Br%27%5El%7D%7Br%5E%7Bl%2B1%7D%7D)

是转动不变的

这个不变量就可以看作张量 ![\underbrace{\mathbb{x}\otimes\mathbb{x}\otimes\cdots\mathbb{x}}_{l \text{times}}](https://www.zhihu.com/equation?tex=%5Cunderbrace%7B%5Cmathbb%7Bx%7D%5Cotimes%5Cmathbb%7Bx%7D%5Cotimes%5Ccdots%5Cmathbb%7Bx%7D%7D_%7Bl+%5Ctext%7Btimes%7D%7D) 与张量 ![\underbrace{\nabla\nabla\cdots\nabla}_{l\text{times}}\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cunderbrace%7B%5Cnabla%5Cnabla%5Ccdots%5Cnabla%7D_%7Bl%5Ctext%7Btimes%7D%7D%5Cfrac%7B1%7D%7Br%7D) 之间的一个内积.

下面的主角就是多极矩张量 ![\underbrace{\nabla\nabla\cdots\nabla}_{l\text{times}}\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cunderbrace%7B%5Cnabla%5Cnabla%5Ccdots%5Cnabla%7D_%7Bl%5Ctext%7Btimes%7D%7D%5Cfrac%7B1%7D%7Br%7D)

首先,它是一个仿射张量,可以验证,在仿射(线性)坐标变换之下是协变的.

齐次,它正式上一节提到的全对称Traceless张量,可以验证,对任意两个下标缩并结果均为零

> ![\delta^{\mu\nu}\partial_{k_1}\partial_{k_2}\cdots\partial_{\mu}\partial_{\nu}\cdots\partial_{k_l}\frac{1}{r}=\partial_{k_1}\cdots\partial_{k_j}\cdots\Delta\frac{1}{r}=0](https://www.zhihu.com/equation?tex=%5Cdelta%5E%7B%5Cmu%5Cnu%7D%5Cpartial_%7Bk_1%7D%5Cpartial_%7Bk_2%7D%5Ccdots%5Cpartial_%7B%5Cmu%7D%5Cpartial_%7B%5Cnu%7D%5Ccdots%5Cpartial_%7Bk_l%7D%5Cfrac%7B1%7D%7Br%7D%3D%5Cpartial_%7Bk_1%7D%5Ccdots%5Cpartial_%7Bk_j%7D%5Ccdots%5CDelta%5Cfrac%7B1%7D%7Br%7D%3D0)

所以,这个张量在坐标变换下实现了转动群的一个 ![2l+1](https://www.zhihu.com/equation?tex=2l%2B1) 维的不可约表式.

然后,它的每一个分量都给出了一个调和多项式,

容易验证,

![r^{l+2}\partial_{k_1}\partial_{k_2}\cdots\partial_{k_l}\frac{1}{r}](https://www.zhihu.com/equation?tex=r%5E%7Bl%2B2%7D%5Cpartial_%7Bk_1%7D%5Cpartial_%7Bk_2%7D%5Ccdots%5Cpartial_%7Bk_l%7D%5Cfrac%7B1%7D%7Br%7D) 均是一个调和多项式.

> 定理(Maxwell,Sylvester):多极矩张量的分量中总包含了调和多项式的完备基底.

**这个定理关键的,他告诉我们,多极矩张量的分量可以被用于生成全部的调和多项式.**

一个最简单的例子就是四极矩张量的分量们

![3xy,3yz,3xz,3x^2-r^2,3y^2-r^2,3z^2-r^2](https://www.zhihu.com/equation?tex=3xy%2C3yz%2C3xz%2C3x%5E2-r%5E2%2C3y%5E2-r%5E2%2C3z%5E2-r%5E2)

当然,后面的三个分量是不独立的,所以可以任意删掉一个,构成一个5维的调和多项式空间. 同时也意识到,这个空间,就是转动群的一个五维的不可约表示,这些基函数,可以构成2阶的球谐函数,在量子力学中,把他们都可以叫做2阶不可约张量算符.

最后我们来谈商表示是怎么体现在这个张量中的.

其实很简单, ![\partial_{k_1}\partial_{k_2}\cdots\partial_{k_l}\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cpartial_%7Bk_1%7D%5Cpartial_%7Bk_2%7D%5Ccdots%5Cpartial_%7Bk_l%7D%5Cfrac%7B1%7D%7Br%7D) 的前面部分就是一个常系数导子值的 ![l](https://www.zhihu.com/equation?tex=l) 齐次多项式,他们代表了齐次多项式的原始表示空间,可是当他们作用到 ![\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cfrac%7B1%7D%7Br%7D) 上的时候,自然会产生一个等价关系

![\sum_{\{k\}}\xi^{k_1k_2\cdots k_l}\partial_{k_1}\partial_{k_2}\cdots\partial_{k_l}\sim\sum_{\{j\}}\xi^{j_1j_2\cdots j_l}\partial_{j_1}\partial_{j_2}\cdots\partial_{j_l} \text{when}\\ \sum_{\{k\}}\xi^{k_1k_2\cdots k_l}\partial_{k_1}\partial_{k_2}\cdots\partial_{k_l}-\sum_{\{j\}}\xi^{j_1j_2\cdots j_l}\partial_{j_1}\partial_{j_2}\cdots\partial_{j_l} \in\langle \partial_x^2+\partial_y^2+\partial_z^2\rangle](https://www.zhihu.com/equation?tex=%5Csum_%7B%5C%7Bk%5C%7D%7D%5Cxi%5E%7Bk_1k_2%5Ccdots+k_l%7D%5Cpartial_%7Bk_1%7D%5Cpartial_%7Bk_2%7D%5Ccdots%5Cpartial_%7Bk_l%7D%5Csim%5Csum_%7B%5C%7Bj%5C%7D%7D%5Cxi%5E%7Bj_1j_2%5Ccdots+j_l%7D%5Cpartial_%7Bj_1%7D%5Cpartial_%7Bj_2%7D%5Ccdots%5Cpartial_%7Bj_l%7D+%5Ctext%7Bwhen%7D%5C%5C+%5Csum_%7B%5C%7Bk%5C%7D%7D%5Cxi%5E%7Bk_1k_2%5Ccdots+k_l%7D%5Cpartial_%7Bk_1%7D%5Cpartial_%7Bk_2%7D%5Ccdots%5Cpartial_%7Bk_l%7D-%5Csum_%7B%5C%7Bj%5C%7D%7D%5Cxi%5E%7Bj_1j_2%5Ccdots+j_l%7D%5Cpartial_%7Bj_1%7D%5Cpartial_%7Bj_2%7D%5Ccdots%5Cpartial_%7Bj_l%7D+%5Cin%5Clangle+%5Cpartial_x%5E2%2B%5Cpartial_y%5E2%2B%5Cpartial_z%5E2%5Crangle)

商掉等价关系后的商空间正是商表示.

## **5.Maxwell-Sylvester方法直接生成球谐函数**

前面的所有论证无非是要说明,调和函数,不可约张量两种体系本质上可以统一为多极矩张量

一方面,多极矩张量就是不可约张量,另一方面,它的分量给出了全部相互独立的调和多项式

我们也知道,球谐多项式是一组特殊的调和多项式,且与直接生成的多极矩分量是等价的,也就是说,存在这一个变换,将多极矩分量转换成球谐函数.

**而张量的协变性使得我们想到,球谐多项式空间中的基变换,可以由张量的坐标变换诱导**

若我们引入以下的线性坐标变换

![x^+=\frac{1}{\sqrt 2}(-x+iy)\qquad x^-=\frac{1}{\sqrt 2}(x+iy)\qquad x^0=z](https://www.zhihu.com/equation?tex=x%5E%2B%3D%5Cfrac%7B1%7D%7B%5Csqrt+2%7D%28-x%2Biy%29%5Cqquad+x%5E-%3D%5Cfrac%7B1%7D%7B%5Csqrt+2%7D%28x%2Biy%29%5Cqquad+x%5E0%3Dz)

则多极矩张量在协变规则下,其分量都变成了球谐函数

最明显的是 ![l=1](https://www.zhihu.com/equation?tex=l%3D1) 时,以上的三个新的坐标就是偶极矩张量在新表象下的坐标,而他们就是三个

一阶的球谐函数.

对于一般的多极矩,按照协变规则 ,新的分量必为

![\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5Cfrac%7B1%7D%7Br%7D)

此时的抽象指标 ![m_i](https://www.zhihu.com/equation?tex=m_i) 可以取 ![-1,0,+1](https://www.zhihu.com/equation?tex=-1%2C0%2C%2B1)

我们将证明,这就是球谐函数.

首先在新的坐标系下,并不改变的是调和多项式的本质,必有

![\Delta r^{2l+1} \partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}\frac{1}{r}=0](https://www.zhihu.com/equation?tex=%5CDelta+r%5E%7B2l%2B1%7D+%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5Cfrac%7B1%7D%7Br%7D%3D0)

所以可以推出的是

![\mathbf{L}^2\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}\frac{1}{r}=l(l+1)\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cmathbf%7BL%7D%5E2%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5Cfrac%7B1%7D%7Br%7D%3Dl%28l%2B1%29%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5Cfrac%7B1%7D%7Br%7D)

齐次,让我们在新的坐标系下考虑角动量算符

![L_z=-i(x\partial_y-y\partial_x)=-x^+\partial_++x^-\partial_-](https://www.zhihu.com/equation?tex=L_z%3D-i%28x%5Cpartial_y-y%5Cpartial_x%29%3D-x%5E%2B%5Cpartial_%2B%2Bx%5E-%5Cpartial_-)

可以证明, ![\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5Cfrac%7B1%7D%7Br%7D) 的为角动量算符属于本征值 ![M=\sum_{i=1}^lm_i](https://www.zhihu.com/equation?tex=M%3D%5Csum_%7Bi%3D1%7D%5Elm_i) 的本征函数

由对易子

![[L_z,\partial_m]=-[x^+\partial_+,\partial_m]+[x^-\partial_-,\partial_m]=\delta_{m,+1}\partial_+-\delta_{m,-1}\partial_-=m\partial_m](https://www.zhihu.com/equation?tex=%5BL_z%2C%5Cpartial_m%5D%3D-%5Bx%5E%2B%5Cpartial_%2B%2C%5Cpartial_m%5D%2B%5Bx%5E-%5Cpartial_-%2C%5Cpartial_m%5D%3D%5Cdelta_%7Bm%2C%2B1%7D%5Cpartial_%2B-%5Cdelta_%7Bm%2C-1%7D%5Cpartial_-%3Dm%5Cpartial_m)

所以对易子

![[L_z,\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}]=\sum_i\partial_{m_1}\cdots[L_z,\partial_{m_i}]\cdots\partial_{m_l}=M\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}](https://www.zhihu.com/equation?tex=%5BL_z%2C%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5D%3D%5Csum_i%5Cpartial_%7Bm_1%7D%5Ccdots%5BL_z%2C%5Cpartial_%7Bm_i%7D%5D%5Ccdots%5Cpartial_%7Bm_l%7D%3DM%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D)

又由于 ![L_z\frac{1}{r}=0](https://www.zhihu.com/equation?tex=L_z%5Cfrac%7B1%7D%7Br%7D%3D0)

所以 ![L_z\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}\frac{1}{r}=M\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}\frac{1}{r}](https://www.zhihu.com/equation?tex=L_z%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5Cfrac%7B1%7D%7Br%7D%3DM%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5Cfrac%7B1%7D%7Br%7D)

这样一来, ![\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5Cfrac%7B1%7D%7Br%7D) 就是 ![\{\mathbf{L}^2,L_z\}](https://www.zhihu.com/equation?tex=%5C%7B%5Cmathbf%7BL%7D%5E2%2CL_z%5C%7D) 的共同本征函数,量子数标记为 ![\vert l,M\rangle](https://www.zhihu.com/equation?tex=%5Cvert+l%2CM%5Crangle)

根据球谐函数的定义可以知道, ![\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5Cfrac%7B1%7D%7Br%7D) 在单位球面上的限制必然与球谐函数 ![Y_{l,M}](https://www.zhihu.com/equation?tex=Y_%7Bl%2CM%7D) 只相差一个归一化的系数和相位因子,进一步地,易验证

![(\partial_m)^*=(-1)^m\partial_{-m}](https://www.zhihu.com/equation?tex=%28%5Cpartial_m%29%5E%2A%3D%28-1%29%5Em%5Cpartial_%7B-m%7D)

所以 ![\partial_{m_1}\partial_{m_2}\cdots\partial_{m_l}\frac{1}{r}](https://www.zhihu.com/equation?tex=%5Cpartial_%7Bm_1%7D%5Cpartial_%7Bm_2%7D%5Ccdots%5Cpartial_%7Bm_l%7D%5Cfrac%7B1%7D%7Br%7D) 在相位约定上也和 ![Y_{l,M}](https://www.zhihu.com/equation?tex=Y_%7Bl%2CM%7D)保持了一致.所以我们可以进行归一化后直接写出球谐函数了.

参考文献:

[1]李政道 *物理学中的数学方法*

[2]Methods of Mathematical Physics [Vol 1] - R. Courant, D. Hilbert (Wiley, 1989)

[3] A.И.柯斯特利金 *代数学引论(第三卷)*

[4]I.R.Shafarevich *代数基本概念*

[5]Group Theory in a Nutshell for Physicists-A.Zee