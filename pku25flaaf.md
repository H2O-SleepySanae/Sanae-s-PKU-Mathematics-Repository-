苗苗困了 SMES PKU 25F LA-A1 Final

# 1.
(i) 矩阵的特征值和特征向量.

由$$\begin{align*}|\lambda I - A| &= \begin{vmatrix} \lambda - 3 & -2 & 1 \\ 2 & \lambda + 2 & -2 \\ -3 & -6 & \lambda + 1 \end{vmatrix}= \begin{vmatrix} \lambda - 3 & 0 & 1 \\ 2 & \lambda - 2 & -2 \\ -3 & 2(\lambda-2) & \lambda + 1 \end{vmatrix}= \begin{vmatrix} \lambda - 3 & 0 & 1 \\ 2 & \lambda - 2 & -2 \\ -7 & 0 & \lambda + 5 \end{vmatrix} \\&= (\lambda - 2)(\lambda^2 + 2\lambda - 8) = (\lambda - 2)(\lambda - 2)(\lambda + 4)\end{align*}$$
得，矩阵$A$的特征值为$$\lambda_1 = 2, \quad \lambda_2 = 2, \quad \lambda_3 = -4.$$分别求解线性方程组$(A-\lambda_iI)x=0$，可求得原矩阵的特征向量.记方程组$Px=0$的解集为$\mathrm{Nul}~P$,则

$$
\begin{aligned}
\mathrm{Nul}~(A - 2I) &= \mathrm{Nul}~\left(\begin{matrix} 1 & 2 & -1 \\ -2 & -4 & 2 \\ 3 & 6 & -3 \end{matrix}\right) = \left<\begin{pmatrix} 2 \\ -1 \\ 0 \end{pmatrix}, \begin{pmatrix} 1 \\ 0 \\ 1 \end{pmatrix}\right>,\\
\mathrm{Nul}~(A + 4I) &= \mathrm{Nul}~\left(\begin{matrix} 7 & 2 & -1 \\ -2 & 2 & 2 \\ 3 & 6 & 3 \end{matrix}\right) = \mathrm{Nul}~\left(\begin{matrix} 1 & 2 & 1 \\ 0 & 3 & 2 \\ 0 & 0 & 0 \end{matrix}\right) = \left<\begin{pmatrix} 1 \\ -2 \\ 3 \end{pmatrix}\right>.
\end{aligned}$$

(ii) 矩阵是否可对角化

将三个向量写入矩阵
$$
T = \begin{pmatrix} 2 & 1 & 1 \\ -1 & 0 & -2 \\ 0 & 1 & 3 \end{pmatrix},$$
则因为
$$|T| = 2\begin{vmatrix} 0 & -2 \\ 1 & 3 \end{vmatrix} + \begin{vmatrix} 1 & 1 \\ 1 & 3 \end{vmatrix} = \begin{vmatrix} 0 & -4 \\ 1 & 3 \end{vmatrix} + \begin{vmatrix} 1 & 1 \\ 1 & 3 \end{vmatrix} = \begin{vmatrix} 1 & -3 \\1&3\end{vmatrix} \neq 0,$$故前面三个特征向量确实线性无关，因此$A$可对角化，且$T$为所求可逆矩阵，此时$$T^{-1}AT=\begin{pmatrix} 2&0&0 \\ 0&2&0 \\ 0&0&-4 \end{pmatrix}.$$

# 2.
(i) 将方程记作$Ax=0$，其中$A=\left( \begin{matrix}
	1&		0&		-1&		-1\\
	0&		1&		0&		-1\\
\end{matrix} \right) $，则$A$的解空间的基为$\{(1,0,1,0)^\mathrm{T},(1,1,0,1)^\mathrm{T}\}=\{s_1,s_2\}$.对这组基标准正交化，可得$A$的解空间的标准正交基:$$\begin{aligned}q_1&=\frac{s_1}{|s_1|}=\frac{1}{\sqrt{2}}(1,0,1,0)^{\mathrm{T}},\\s_2'&=s_2-\frac{(q_1,s_2)}{(q_1,q_1)}q_1=(1,1,0,1)^\mathrm{T}-\frac12 (1,0,1,0)^\mathrm{T} = \frac12 (1,2,-1,2)^\mathrm{T},\\q_2&=\frac{s_2'}{|s_2'|}=\frac{1}{\sqrt{10}}(1,2,-1,2)^\mathrm{T}.\end{aligned}$$
(ii) 由于线性方程组的解空间与列向量构成的线性空间正交，故列空间正任意一个向量都与解空间每个向量正交.由于$A$的两行线性无关，它们构成$A$的列空间的一组基，因此所求向量可由它们线性组合而得：$$a=(x,y,-x,-x-y)^\mathrm{T},\qquad x,y\in\mathbb{R}.$$

# 3.
本题考查正交投影的定义.最开始的做法是写出$W$和$W^\perp$的标准正交基，虽然也算对了，但显然麻烦得多.最好的做法是先考虑正交投影的定义.

先求$W$的标准正交基：$$W=\left<q_1,q_2\right>=\left<\frac{1}{\sqrt{2}}(1,0,1,0)^\mathrm{T},\frac{1}{\sqrt{22}}(1,4,-1,2)^\mathrm{T}\right>.$$
(i) 由题意有$$A\alpha=\frac{(q_1,\alpha)}{(q_1,q_1)}q_1+\frac{(q_2,\alpha)}{(q_2,q_2)}q_2.$$对$\alpha$取单位矩阵的各列$e^i$，则$A$的第$i$列为$$A^i=\frac{(q_1,e^i)}{(q_1,q_1)}q_1+\frac{(q_2,e^i)}{(q_2,q_2)}q_2,$$故$$A=\left( \begin{matrix}
	q_1&		q_2\\
\end{matrix} \right) \left( \begin{matrix}
	q_1^\mathrm{T}\\
	q_2^\mathrm{T}\\
\end{matrix} \right)I=q_1q_1^\mathrm{T}+q_2q_2^\mathrm{T}=\frac{1}{11}\left( \begin{matrix}
	6&		2&		5&		1\\
	2&		8&		-2&		4\\
	5&		-2&		6&		-1\\
	1&		4&		-1&		2\\
\end{matrix} \right).$$
另外的推理过程：在$\mathbb{R}^4$空间上一定找得到$q_3$和$q_4$，使得$\{q_i\}_{i=1}^4$为标准正交基，设$Q$的各列为$q_i$，则有$AQ=Q~\mathrm{diag}\{1,1,0,0\}.$考虑到$Q$是正交矩阵，我们完成了对$A$的正交对角化，它的谱分解形式就是$A=q_1q_1^\mathrm T+q_2q_2^\mathrm T.$

(ii) 由正交分解定理（请确认大家使用的课本），对任意向量$\beta$，都可以唯一地分解为$W$和$W^\perp$中的向量$A\beta\in W$和$(\beta - A\beta)\in W^\perp$.考虑到$\beta \rightarrow B\beta$定义了一个线性变换，故该矩阵对$\beta$的作用应为$$B\beta = A\beta - (\beta - A\beta)=(2A-I)\beta,$$由$\beta$的任意性，$$B=2A-I=\frac{1}{11}\left( \begin{matrix}
	1&		4&		10&		2\\
	4&		5&		-4&		8\\
	10&		-4&		1&		-2\\
	2&		8&		-2&		7\\
\end{matrix} \right).$$
由定义方式，符合要求的线性变换应该是唯一的，但严谨起见，验证$B$的正交性.因为$BB^\mathrm{T}=(2A-I)^2=4A^2-4A+I$，而$$A^2=\left( \begin{matrix}
	q_1&		q_2\\
\end{matrix} \right) \left( \begin{matrix}
	q_1^\mathrm{T}\\
	q_2^\mathrm{T}\\
\end{matrix} \right)\left( \begin{matrix}
	q_1&		q_2\\
\end{matrix} \right) \left( \begin{matrix}
	q_1^\mathrm{T}\\
	q_2^\mathrm{T}\\
\end{matrix} \right)=A,$$故$BB^\mathrm{T}=I$，$B$一定是正交的.

# 4.
(i) 计算奇异值

$A$的奇异值是矩阵$$A^\mathrm{T}A=\left( \begin{matrix}	1&		0\\	1&		2\\	0&		1\\\end{matrix} \right) \left( \begin{matrix}	1&		1&		0\\	0&		2&		1\\\end{matrix} \right) =\left( \begin{matrix}	1&		1&		0\\	1&		5&		2\\	0&		2&		1\\\end{matrix} \right) =\Lambda $$的三个特征值中，前两大特征值的正平方根.又因为
$$|\lambda I-\Lambda| = \left| \begin{matrix}	\lambda -1&		-1&		0\\	-1&		\lambda -5&		-2\\	0&		-2&		\lambda -1\\\end{matrix} \right|=(\lambda -1)\left| \begin{matrix}	\lambda -5&		-2\\	-2&		\lambda -1\\\end{matrix} \right|+\left| \begin{matrix}	-1&		-2\\	0&		\lambda -1\\\end{matrix} \right|=\lambda (\lambda -1)(\lambda -6),$$
故$\Lambda$的特征值为$$\lambda _1=6,\quad\lambda _2=1,\quad\lambda _3=0.$$故$A$的奇异值为
$$\sigma _1=\sqrt{6},\quad\sigma _2=1.$$

(ii) 求正交矩阵

先对$A^\mathrm{T}A$对角化，即求正交矩阵$V$，使得$$A^\mathrm{T}AV=V\left( \begin{matrix}	6&		&		\\	&		1&		\\	&		&		0\\\end{matrix} \right). $$
因为
$$
\begin{aligned}
\mathrm{Nul}~\left( A^\mathrm{T}A-6I \right) &=\mathrm{Nul}~\left( \begin{matrix}
	-5&		1&		0\\
	1&		-1&		2\\
	0&		2&		-5\\
\end{matrix} \right) =\left< \left( \begin{matrix}
	1\\
	5\\
	2\\
\end{matrix} \right) \right> ,\\
\mathrm{Nul}~(A^\mathrm{T}A-I)&=\mathrm{Nul}~\left( \begin{matrix}
	0&		1&		0\\
	1&		4&		2\\
	0&		2&		0\\
\end{matrix}  \right) =\left< \left( \begin{matrix}
	2\\
	0\\
	-1\\
\end{matrix} \right) \right> ,\\
\mathrm{Nul}~(A^\mathrm{T}A)&=\left< \left( \begin{matrix}
	1\\
	-1\\
	2\\
\end{matrix} \right) \right>,\\
\end{aligned}
$$
故$V$可取$$V=\left( \begin{matrix}
	\frac{1}{\sqrt{30}}&		\frac{2}{\sqrt{3}}&		\frac{1}{\sqrt{6}}\\
	\frac{5}{\sqrt{30}}&		0&		-\frac{1}{\sqrt{6}}\\
	\frac{2}{\sqrt{30}}&		-\frac{1}{\sqrt{5}}&		\frac{2}{\sqrt{6}}\\
\end{matrix} \right).$$


根据奇异值分解的计算过程，只需要再计算$AV$，并对所得结果归一化，即得到所求的正交矩阵.因为
$$
AV =\left( \begin{matrix}
	\frac{6}{\sqrt{50}}&		\frac{2}{\sqrt{5}}&		0\\
	\frac{12}{\sqrt{30}}&		-\frac{1}{\sqrt{5}}&		0\\
\end{matrix} \right) =\left( \begin{matrix}
	\frac{1}{\sqrt{5}}&		\frac{2}{\sqrt{5}}\\
	\frac{2}{\sqrt{5}}&		-\frac{1}{\sqrt{5}}\\
\end{matrix} \right) \left( \begin{matrix}
	\sqrt{6}&		&		\\
	&		1&		0\\
\end{matrix} \right),
$$
所以取$$Q=V,P=\left( \begin{matrix}
	\frac{1}{\sqrt{5}}&		\frac{2}{\sqrt{5}}\\
	\frac{2}{\sqrt{5}}&		-\frac{1}{\sqrt{5}}\\
\end{matrix} \right)$$即可.
# 5.

*据说是数值方法的结论，我不太了解.但是化简$f(x)$用到了经典的行列式降阶技巧，可能还是要掌握一下的.*

(i)对于对称矩阵$A$，存在正交矩阵$P$，使得$PAP^\mathrm{T}=\mathrm{diag}\{\lambda_1,\lambda_2,\cdots,\lambda_n\}=D$，这里$D$是可逆的.

对于$f(x)$，有下面关系成立$$\begin{aligned}
f(x)=\left|\begin{matrix}A&x\\x^\mathrm{T}&a|x|^2\end{matrix}\right|&=
\left|\begin{matrix}P&0\\0&1\end{matrix}\right|
\left|\begin{matrix}A&x\\x^\mathrm{T}&a|x|^2\end{matrix}\right|
\left|\begin{matrix}P^\mathrm{T}&0\\0&1\end{matrix}\right|\\&=
\left|\begin{matrix}D&Px\\(Px)^\mathrm{T}&a|x|^2\end{matrix}\right|\\&=
\left|\begin{matrix}I&0\\-(Px)^\mathrm{T}D^{-1}&1\end{matrix}\right|
\left|\begin{matrix}D&Px\\(Px)^\mathrm{T}&a|x|^2\end{matrix}\right|\\&=
\left|\begin{matrix}D&Px\\0&a|x|^2-(Px)^\mathrm{T}D^{-1}(Px)\end{matrix}\right|,
\end{aligned}$$

令$Px=y$，则$y^\mathrm{T}y=1\Leftrightarrow|x|^2=|y|^2,$ $$f(x)=\prod_{i=1}^n\lambda_i\sum_{i=1}^n\left[\left(a-\frac{1}{\lambda_i}\right)y_i^2\right].$$据此给出$f(x)$的一个标准型.

(ii)$\max_{|x|=1}f(x)$和$\min_{|x|=1}f(x)$分别为二次型$f(x)$的最大和最小特征值.由于$\lambda_1\leqslant\lambda_2\leqslant\cdots\leqslant\lambda_n$，故$a-\frac{1}{\lambda_n}\leqslant a-\frac{1}{\lambda_{n-1}}\leqslant \cdots\leqslant a-\frac{1}{\lambda_1}$，故$$\max_{|x|=1}f(x)=\prod_{i=1}^n\lambda_i\sum_{i=1}^n\left(a-\frac{1}{\lambda_1}\right),\min_{|x|=1}f(x)=\prod_{i=1}^n\lambda_i\sum_{i=1}^n\left(a-\frac{1}{\lambda_n}\right).$$

(iii)若二次型的最小值为正，则二次型正定，这等价于$a>\frac{1}{\lambda_n}$；
若二次型的最大值为负，则二次型负定，这等价于$a<\frac{1}{\lambda_1}$；
其余情况下二次型不定，这等价于$\frac{1}{\lambda_1}\leqslant a\leqslant\frac{1}{\lambda_n}$.

# 6.

*这个其实是极分解的弱化结论，它的直接意义是任何一个连续体的变形行为，都可以分解为一个轴向拉伸和旋转（有时包括镜像）对连续体的先后作用.这里直接引用奇异值分解的结论证明之.*

任意方阵$A$都存在奇异值分解$A=U\Sigma V^\mathrm{T}$，其中$U,V$为正交矩阵，$\Sigma$为对角矩阵,因此$A$可以分解为$$A=U\Sigma V^T=U\Sigma U^\mathrm{T} U V^\mathrm{T}.$$令$$U\Sigma U^\mathrm{T}=S,U V^\mathrm{T}=Q,$$则容易验证$S$是对称矩阵，$Q$是正交矩阵，因而可逆.于是原题得证.

# 7.

由于$A$是正定矩阵，故存在正交矩阵$P$和对角矩阵$D$使得$A=P^\mathrm{T}DP$.定义$D$的平方根$R$为$D$的各个元素改写为其正平方根，则$D$和$R$都是对角矩阵且$R^2=D$.于是，因为相等，或者在左乘某个矩阵的同时右乘它的逆，下面矩阵相似：$$AB = P^\mathrm{T}DPB \sim DPBP^\mathrm{T}=RRPBP^\mathrm{T}\sim RPBP^\mathrm{T}R=RPBP^\mathrm{T}R^\mathrm{T}=RPB(RP)^\mathrm{T}.$$

注意到：

1. 正定矩阵$B$和$RPB(RP)^\mathrm{T}$合同，因而$B$和$RPB(RP)^\mathrm{T}$具有相同的正惯性指数，$RPB(RP)^\mathrm{T}$的特征值都是正实数;

2. $AB$和$RPB(RP)^\mathrm{T}$相似，因而$AB$和$RPB(RP)^\mathrm{T}$的特征值相同，二者的特征值也都是正实数.

于是原题得证.

# 8.

设$A^\mathrm{T}A=B^\mathrm{T}B=S$，则存在正交矩阵$P$和对角矩阵$D=\mathrm{diag}\{d_1,\cdots,d_r,0\cdots,0\}$（其中$r$为$S$的秩；由于$S$正定，$d_i>0$，据此可定义$D$的平方根$R$）使得$S=PDP^\mathrm{T}$，于是$(AP)^\mathrm{T}(AP)=(BP)^\mathrm{T}(BP)=D$.考虑$BP$的第$i$列$b'_i$，则有：

1. $|b'_i|=\begin{cases}\sqrt{d_i},i\leqslant r,\\0,i>r,\end{cases}~~$进而有$b'_i=0(i>r).$

2. $\left\{\frac{b'_i}{|b'_i|}\right\}_{i=1}^{r}$构成$\mathbb{R}^n$中某个子空间的一组标准正交基，且可扩充为$\mathbb{R}^n$的一组标准正交基.据此定义正交矩阵$Q=\left(\begin{matrix}Q_r&Q_{n-r}\end{matrix}\right)$，其前$r$列为$\frac{b'_i}{|b'_i|}(i=1,\cdots,r)$，后$(n-r)$列只需要和前$r$列正交.

故$$BP=\left(\begin{matrix}b'_1&\cdots&b'_r&0&\cdots&0\end{matrix}\right)=\left(\begin{matrix}Q_r&Q_{n-r}\end{matrix}\right)R\Leftrightarrow B=QRP^\mathrm{T}.$$于是我们为$B$找到了奇异值分解.由前面的构造过程可知，$A$的构造过程是类似的，其中：

1. 因为$D$的对角化过程提供了$P$，我们仍然考虑$AP$的各列，因此在$A$的奇异值分解$A=U\Sigma V^\mathrm{T}$中，取$V=P,\Sigma=R$没有问题；

2. 因为对$B$作奇异值分解的过程中构造的$Q$依赖于$B$的形式，因此$A$中根据$AP$定义的正交矩阵应与$B$的不同.

因此，存在可能异于$Q$的正交矩阵$S$，使得$A=SRP^\mathrm{T}$.

因此，$$A=SRP^\mathrm{T}=A=SQ^\mathrm{T}
QRP^\mathrm{T}=(SQ^\mathrm{T})B,$$其中$SQ^\mathrm{T}$是正交矩阵.