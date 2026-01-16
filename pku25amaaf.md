苗苗困了 SMES PKU 25F AM-A1 Final

# 1.

(1) 由题目：$$\begin{aligned}\left|\overrightarrow{AB}\times\overrightarrow{AC}\right|&=\left|\begin{matrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\2&a&0\\0&-1&2\end{matrix}\right|=\left(2a,-4,-2\right)=\sqrt{4a^2+16+4}=2\sqrt{6}\Leftrightarrow a=1,\\V_{ABCD}&=\left|\begin{matrix}2&a&0\\0&-1&2\\2&b&1\end{matrix}\right|=-2+4a-4b=2\Leftrightarrow a-b=1,\end{aligned}$$故$$a=1,\qquad b=0.$$

(2) 平面过$\overrightarrow{r_0}=(2,3,4)$点，且一个法向量为$$\overrightarrow{n}=\overrightarrow{AB}\times\overrightarrow{AD}=\left|\begin{matrix}\boldsymbol{i}&\boldsymbol{j}&\boldsymbol{k}\\2&1&0\\2&0&1\end{matrix}\right|=(1,-2,-2),$$故平面方程可由$\overrightarrow{n}\cdot(\overrightarrow{r}-\overrightarrow{r_0})=0$给出，即$$(x-2)-2(y-3)-2(z-4)=0\Leftrightarrow x-2y-3z+12=0.$$

(3)当$\boldsymbol{x}=(1,2,1)$时，由$$\frac{\partial f}{\partial x}=2x+yz=4,\qquad\frac{\partial f}{\partial y}=2y+xz=5,\qquad\frac{\partial f}{\partial x}=2z+xy=4,$$故$$\left.\nabla f\right|_{\boldsymbol{x}=(1,2,1)}=\left(\frac{\partial f}{\partial x},\frac{\partial f}{\partial y},\frac{\partial f}{\partial z}\right)_{\boldsymbol{x}=(1,2,1)}=(4,5,4).$$因为与$\overrightarrow{AB}$同向的方向向量为$\overrightarrow{n_1}=\left(\frac{2}{\sqrt{5}},\frac{1}{\sqrt{5}},0\right)$，所以所求方向导数为$$\left.\frac{\partial f}{\partial n}\right|_{\boldsymbol{x}=(1,2,1)}=\overrightarrow{n_1}\cdot\left.\nabla f\right|_{\boldsymbol{x}=(1,2,1)}=\frac{13}{\sqrt{5}}.$$

# 2.

(1) 由于$\displaystyle \lim_{x\rightarrow 2}\frac{f(2x-2)}{x-2}$存在，$\displaystyle \lim_{x\rightarrow 2}{(x-2)}=2$，且$f(2x-2)$在$2$处有定义，$f(2)=0$一定成立.

又因为$\forall x \in (2,4), f'(x)>0$，所以$f(x)$在$(2,4)$上单调递增，故$\forall x \in [2,4], f(x)\geqslant f(2) = 0$，且$f(x)=0,x\in[2,4],\Leftrightarrow x=2$

(2) 对定义于$[2,4]$的函数$\displaystyle g(y)=6f(y)-y\int_2^4f(x)\mathrm{d}x$在$[2,4]$上积分：$$\int_2^4g(y)\mathrm{d}y=6\int_2^4 f(y)\mathrm{d}y-\int_2^4 y\mathrm{d}y\int_2^4f(x)\mathrm{d}x=(6-6)\int_2^4f(x)\mathrm{d}x=0.$$由于$g(y)$是定义于闭区间上的连续函数，故必存在$\xi\in(2,4)$，使得$\displaystyle g(\xi)=0\Leftrightarrow \frac{6f(\xi)}{\xi}=\int_2^4f(x)\mathrm{d}x.$

(3) 对(2)所证结论等价变形得$$6\cdot\frac{f(\xi)-f(2)}{\xi-2}=\frac{\xi}{\xi-2}\int_2^4f(x)\mathrm{d}x.$$因为$f(x)$在$[2,4]$上连续，在$(2,4)$上可导，故由Lagrange中值定理，对(2)中的$\xi$，存在$\eta\in(2,\xi)\subset(2,4)$（因此自然有$\eta\neq\xi$），使得$$6f'(\eta)=\frac{\xi}{\xi-2}\int_2^4f(x)\mathrm{d}x.$$

# 3.

(1) 易知$$f(x)=\sum_{n=1}^N(-1)^{n-1}\frac{x^n}{n}+o(x^{n})=x-\frac{x^2}{2}+\frac{x^3}{3}-\frac{x^4}{4}+\cdots+o(x^{n}).$$

(2) 用Taylor展开式重写待求极限的表达式：$$\begin{aligned}
\frac{1}{x^2}\left[2(1+x)^{\frac1x}+\mathrm{e}(x-2)\right]
&=\frac{1}{x^2}\left\{2\exp\left[\frac{\ln(1+x)}{x}\right]+\mathrm{e}(x-2)\right\}\\
&=\frac{1}{x^2}\left\{2\exp\left[\frac{x-\frac{x^2}{2}+\frac{x^3}{3}+o(x^3)}{x}\right]+\mathrm{e}(x-2)\right\}\\
&=\frac{1}{x^2}\left\{2\exp\left[1-\frac{x}{2}+\frac{x^2}{3}+o(x^2) \right] +\mathrm{e}(x-2)\right\}\\
&=\frac{1}{x^2}\left\{2\mathrm{e}\exp\left[-\frac{x}{2}+\frac{x^2}{3}+o(x^2) \right] +\mathrm{e}(x-2)\right\}\\
&=\frac{1}{x^2}\left\{2\mathrm{e}\left[1+\left(-\frac{x}{2}+\frac{x^2}{3}\right)+\frac12\left(-\frac{x}{2}+\frac{x^2}{3}\right)^2+o(x^2) \right] +\mathrm{e}(x-2)\right\}\\
&=\frac{1}{x^2}\left\{2\mathrm{e}\left[1-\frac{x}{2}+\frac{x^2}{3}-\frac{x^2}{8}+o(x^2) \right] +\mathrm{e}(x-2)\right\}\\
&=\frac{5\mathrm{e}}{12}+o(1),
\end{aligned}$$
故所求极限$I=\frac{5\mathrm{e}}{12}$.

# 4.

一个关于齐次函数的题目.

(1) 对确定的$x$和$y$，在实数域上定义函数$g(t)=f(tx,ty)-t^2f(x,y)$，则事实上$g(t)$就是常函数$0$，则$$
0=g'(t)=x\left.\frac{\partial f}{\partial x}\right|_{(tx,ty)}+y\left.\frac{\partial f}{\partial y}\right|_{(tx,ty)}-2tf(x,y).$$令上式中$x=1,y=2,t=1$，则$$
0=\left.\frac{\partial f}{\partial x}\right|_{(1,2)}+2\left.\frac{\partial f}{\partial y}\right|_{(1,2)}-2f(1,2)=5+2\left.\frac{\partial f}{\partial y}\right|_{(1,2)}\Leftrightarrow \left.\frac{\partial f}{\partial y}\right|_{(1,2)}=-\frac52.$$

(2) 对于函数$h(t)=\left\{1+f\left(2t-2\sin t+1,\sqrt[3]{1+t^3}+1\right)\right\}^{\frac{1}{\ln(1+t^3)}}$，先计算$\displaystyle \lim_{t\rightarrow 0}{h(t)}$. 然后，考虑L'Hospital法则.

对此，依次考虑下面函数在自变量取零附近的Taylor展开式：$$\begin{aligned}
\delta X(t)=2t-2\sin t&=2t-2\left(t-\frac{1}{6}t^3\right)+o(t^3)=\frac{1}{3}t^3+o(t^3),\\
\delta Y(t)=\sqrt[3]{1+t^3}-1&=1+\frac{1}{3}t^3-1+o(t^3)=\frac{1}{3}t^3+o(t^3),\\
f(2t-2\sin t+1,\sqrt[3]{1+t^3}+1)&=f(1+\delta X,2+\delta Y)\\
&=f(1,2)+f_x(1,2)\delta X+f_y(1,2)\delta Y+o(t^3)\\
&=-\frac52(\delta Y-2\delta X)+o(t^3)\\
&=-\frac52\left(\frac13 t^3-\frac23 t^3\right)+o(t^3)\\
&=\frac56 t^3+o(t^3),\\
\ln h(t) = \frac{\ln\left[1+f\left(2t-2\sin t+1,\sqrt[3]{1+t^3}+1\right)\right]}{{\ln(1+t^3)}}
&=\frac{\ln\left[1+\frac56 t^3+o(t^3)\right]}{\ln(1+t^3)}=\frac56+o(1),
\end{aligned}$$故$\displaystyle \lim_{t\rightarrow 0}{h(t)}=\mathrm{e}^{\frac56}.$考虑到原式的分子和分母在$x\rightarrow 0$时都趋于$0$，由L'Hospital法则，原式等于$\mathrm{e}^{\frac56}.$

# 5.

解偏微分方程？有点意思.

(1) 将$u_{xy}(x,y)=0$看作对$x$固定而以$y$为自变量的一元函数，对$y$积分，则存在函数$f_0(x)$使得$u_x(x,y)=f_0(x)$；再将$u_x(x,y)$看作对$y$固定而以$x$为自变量的一元函数，对$x$积分，则存在函数$f(x)$和$g(y)$，使得$f'(x)=f_0(x)$且$u(x,y)=f(x)+g(y)$.

将$u(x,y)=f(x)+g(y)$中的$x$或$y$固定为$x_0$或$y_0$，可据此定义以$y$或$x$为自变量的一元函数$u(x_0,y)=f(x_0)+g(y)$或$u(x,y_0)=f(x)+g(y_0)$.因为$u(x,y)$是二阶可导的，所以$f(x)$和$g(y)$也是二阶可导的.

(2) 因为
$$\begin{aligned}
	\frac{\partial z}{\partial x}&=\frac{\partial z}{\partial u}\frac{\partial u}{\partial x}=\frac{1}{u}\frac{\partial u}{\partial x}\\
	\frac{\partial ^2z}{\partial x\partial y}&=\frac{\partial}{\partial y}\left( \frac{\partial z}{\partial x} \right) =\frac{\partial}{\partial y}\left( \frac{1}{u}\frac{\partial u}{\partial x} \right) =-\frac{1}{u^2}\frac{\partial u}{\partial x}\frac{\partial u}{\partial y}+\frac{1}{u}\frac{\partial ^2u}{\partial x\partial y}\\
	&=-\frac{1}{u^2}\frac{\partial u}{\partial x}\frac{\partial u}{\partial y}+\frac{1}{u}\left( \frac{1}{u}\frac{\partial u}{\partial x}\frac{\partial u}{\partial y} \right) =0\\
\end{aligned}$$
所以若$z=\ln u(x,y)$，则$\frac{\partial^2 z}{\partial x\partial y}=0$.

(3) 由(2)，若作变量替换$z=\ln u(x,y)$，则
$$\begin{cases}
	\frac{\partial ^2z}{\partial x\partial y}=0,&		(x,y)\in D\\
	\varepsilon (x,0)=-\frac{x^2}{2}+\ln x,&		x\in (0,+\infty ),\\
	\varepsilon (1,y)=-\frac{y^2}{2}-\frac{1}{2},&		y\in (-\infty ,+\infty ).\\
\end{cases}$$
由(1)，存在二阶可导的函数$f(x)$和$g(y)$，使得$$z(x,y)=f(x)+g(y).$$
令$y=0$，则$$z(x,0)=f(x)+g(0)=-\frac{x^2}{2}+\ln x;$$
令$x=1$，则$$\begin{aligned}
z(1,y)&=f(1)+g(y)=-\frac12-\frac{y^2}{2},\\
z(1,0)&=-\frac12=f(1)+g(0).
\end{aligned}$$
据上面四式有$$z(x,y)=-\frac{x^2+y^2+1}{2}+\ln x - f(1) - g(0) = -\frac{x^2+y^2}{2}+\ln x,$$继而$$u(x,y) = \exp z(x,y) = x\exp\left(\frac{x^2+y^2}{2}\right).$$

# 6.
(1) 证明$g(x,y)$在$(0,0)$处取到极值.

只需证明$\nabla g|_{(0,0)}=(0,0)$即可，为此需对$g(x,y)=f(u(x,y),v(x,y))=f(\mathrm{e}^{xy},x^2+y^2)$求导.因为$f(x,y)=1-x-y+o(|\Delta \boldsymbol x|)$，所以在$(x,y)=(1,0)$处，$f_x=f_y=-1$.注意到此时$u(0,0)=1,v(0,0)=0$，因此$(u,v)=(1,0),(x,y)=(0,0)$；并注意区分$\partial_xf$和$\partial_xu$（其他需要区分的偏导类似）：
$$
\begin{aligned}
	\left. \frac{\partial g}{\partial x} \right|_{(x,y)}&=\left. \frac{\partial f}{\partial x} \right|_{(u,v)}\left. \frac{\partial u}{\partial x} \right|_{(x,y)}+\left. \frac{\partial f}{\partial y} \right|_{(u,v)}\left. \frac{\partial v}{\partial x} \right|_{(x,y)}=(-1)(ye^{xy})+(-1)(2x)=0\\
	\left. \frac{\partial g}{\partial y} \right|_{(x,y)}&=\left. \frac{\partial f}{\partial x} \right|_{(u,v)}\left. \frac{\partial u}{\partial y} \right|_{(x,y)}+\left. \frac{\partial f}{\partial y} \right|_{(u,v)}\left. \frac{\partial v}{\partial y} \right|_{(x,y)}=(-1)(xe^{xy})+(-1)(2y)=0\\
\end{aligned}
$$
因此完成证明，$g(x,y)$确实在$(0,0)$处取到极值.

(2) 求极值.

由于$\displaystyle f(1,0)=\lim_{(x,y)\rightarrow (1,0)}f(x,y)=1-1-0=0$且$g(0,0)=f(1,0)=0$，故该极值为$0$.

(3) 判断极值点类型.

在对$g(x,y)$求二阶导之前，为清晰起见，需明确一些符号的具体含义.对于以$(u,v)$为自变量的诸函数$\frac{\partial f}{\partial x},\frac{\partial f}{\partial y}$，后面记作$f_1(u,v),f_2(u,v)$，这两个函数在$(u=1,v=0)$即$(x=0,y=0)$处的一阶导为
$$
\begin{aligned}
	(f_1)_x&=f_{11}u_x+f_{12}v_x=0\\
	(f_2)_x&=f_{21}u_x+f_{22}v_x=0\\
	(f_1)_y&=f_{11}u_y+f_{12}v_y=0\\
	(f_2)_y&=f_{21}u_y+f_{22}v_y=0\\
\end{aligned}
$$
于是，我们开始对$g(x,y)$求二阶导：
$$
\begin{aligned}
	g_{xx}&=\left( f_1u_x+f_2v_x \right) _x=f_{1}u_{xx}+f_{2}v_{xx}=(-1)\left( y^2e^{xy} \right) +(-1)(2)=-2\\
	g_{xy}&=\left( f_1u_x+f_2v_x \right) _y=f_{1}u_{xy}+f_{2}v_{xy}=(-1)\left[ (1+xy)e^{xy} \right] +(-1)(0)=-1\\
	g_{yy}&=\left( f_1u_y+f_2v_y \right) _y=f_{1}u_{yy}+f_{2}v_{yy}=(-1)\left( x^2e^{xy} \right) +(-1)(2)=-2\\
\end{aligned}
$$
据此可得$g(x,y)$在$(x,y)=(0,0)$处的Hessian为$\left(\begin{matrix}-2&-1\\-1&-2\end{matrix}\right)$，它是特征值为$-1$和$-3$的实对称矩阵，因此也是负定矩阵，这说明这个极值点是极大值点.

# 7.

微分几何背景，所给条件和曲率有关.但是本题的求解主要运用隐函数存在定理，表示出隐函数的各阶导数.考虑到隐函数存在定理只能给出局部存在性，故考虑逐渐延拓解的存在范围.事实上，由于条件对称，这个过程容易进行，不过还是需要严格化.

看到$f_y(xy)\neq 0$就能想到隐函数定理，这个条件很有特色，应注意识别.

(1) 必要性显然，但稍加说明为妙.

对任意实数$C\in  I$，若曲线$F(x,y)=C$为直线，则$F(x,y)$为一（经过平移的）线性函数，即$F(x,y)=Ax+By+C'$，且$B\neq 0$.因为
$$
\frac{\partial f}{\partial x}=A,\quad \frac{\partial f}{\partial y}=B,\quad \frac{\partial ^2f}{\partial x\partial y}=\frac{\partial ^2f}{\partial x^2}=\frac{\partial ^2f}{\partial y^2}=0
$$
所以
$$
\left( \frac{\partial f}{\partial y} \right) ^2\frac{\partial ^2f}{\partial x^2}-2\frac{\partial f}{\partial x}\frac{\partial f}{\partial y}\frac{\partial ^2f}{\partial x\partial y}+\left( \frac{\partial f}{\partial x} \right) ^2\frac{\partial ^2f}{\partial y^2}=B^2\cdot 0-2AB\cdot 0+A^2\cdot 0=0
$$

(2) 充分性分下面几步证明.

1. 对任意实数$C\in I$，都存在$(x_0,y_0)$，使得$F(x,y)=f(x,y)-C=0$.在$(x_0,y_0)$处，由于$F(x,y)$满足
	1. $F$在包含$(x_0,y_0)$的区域$D$内连续，
	2. $F(x_0,y_0)=0$，
	3. $F_y(x,y)$在$D$内连续，
	4. $F_y(x_0,y_0)\neq 0$，
	故$\exists \delta > 0$，$\forall x \in \left(x_0-\frac{3\delta}{2},x_0+\frac{3\delta}{2}\right)=I_0$，存在唯一一个定义于$I_0$上的函数$y_0(x)$，使得$F(x,y_0(x))=0,\forall x \in I_0$.
2. 因为$f(x,y)$具有二阶连续偏导数，故具体说来$F_x(x,y)$也是连续函数，故$y_0(x)$在$I_0$上具有连续导函数$y_0'(x)=-\frac{F_x(x,y)}{F_y(x,y)}=-\frac{f_x(x,y)}{f_y(x,y)}$；因为分子和分母都连续可导，故$y_0$也二阶连续可导，且$$\begin{aligned}y_0''(x)&=-\frac{\mathrm{d}}{\mathrm{d}x}\frac{F_x(x,y)}{F_y(x,y)}=-\frac{\mathrm{d}}{\mathrm{d}x}\frac{f_x(x,y_0(x))}{f_y(x,y_0(x))}\\
	&=-\frac{1}{f_{y}^{2}}\left[ \left( \left. \frac{\partial f_x}{\partial z} \right|_{(x,y_0)}+\left. \frac{\partial f_x}{\partial y} \right|_{(x,y_0)}y'_0 \right) f_y-f_x\left( \left. \frac{\partial f_y}{\partial z} \right|_{(x,y_0)}+\left. \frac{\partial f_y}{\partial y} \right|_{(x,y_0)}y'_0 \right) \right]\\
	&=\frac{1}{f_{y}^{2}}\left\{ f_x\left[ f_{xy}+f_{yy}\left( -\frac{f_x}{f_y} \right) \right] -f_y\left[ f_{xx}+f_{xy}\left( -\frac{f_x}{f_y} \right) \right] \right\}\\
	&=\frac{1}{f_{y}^{3}}\left( f_xf_yf_{xy}-f_{x}^{2}f_{yy}-f_{y}^{2}f_{xx}+f_xf_yf_{xy} \right)\\
	&=0\\
\end{aligned}$$
因此，在区间$I_0$上积两次分，即得$y_0(x)=a_0x+m_0$.
3. 下面证明：在区间$I_k=I_0+k\delta(k\in \mathbb{Z})$上，该条件均唯一定义函数$y_k(x)$，且该函数必为线性函数.
	1. 我们只需给出$(k\in \mathbb{Z}^+)$情形的证明过程.
	2. $k=0$已经验证.
	3. 现在假设对于所有的$k=n(n>0)$都得到验证，则以此为基础，取$x=x_0+n\delta$，因为由归纳假设，$y_n$得到定义，则可以取$y=y_n(x_0+n\delta)$，则$(x,y)$点处满足的一切条件都和第1、2步相同，故区间$I_{n+1}$上也唯一定义一个线性函数$y_{k+1}(x)$.
因此，我们证明了在区间$I_k$上该函数都是唯一定义的，且是线性函数，即$y_k(x)=a_kx+m_k$.
4. 又因为对于函数$y_k$和$y_{k+1}$，两函数的定义域有公共区域$J_k=I_k\cup I_{k+1}=\left(x_0+\left(k+\frac12\right)\delta,x_0+\left(k+\frac32\right)\delta\right)$，所以由唯一性，两函数在公共区域的表达式相同，因此$a_k=a,m_k=m$.
5. 因此，在相应条件下，该条件隐式定义了一个
	1. 唯一的
	2. 连续的
	3. 满足$f(x,y)=C$的
	线性函数，即曲线$f(x,y)=C$为直线.