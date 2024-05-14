# 機率 hw7

## 資工二 111590012 林品緯

### 1.

#### (a)

$$
\begin{aligned}
\int_{0}^{\infty}ce^{-3x} dx =& 1 \\
c\left[-\frac{e^{-3x}}{3}\right]^{\infty}_{0}  =& 1 \\
c(0-(-\frac{1}{3})) =& 1 \\
c =& 3
\end{aligned}
$$

Ans:

$c=3$

#### (b)

$$
\begin{aligned}
\int_{0}^{0.5}3e^{-3x}dx =& \left[-e^{-3x}\right]^{0.5}_ {0} \\
=&-(e^{-1.5}-1) \\
=&0.77686984
\end{aligned}
$$

Ans:

0.77686984

### 2.

#### (a)

$$
\begin{aligned}
f(x) =& F'(x) \\
=& (1-\frac{16}{x^2})' \\
=& \frac{32}{x^{3}}
\end{aligned}
$$

Ans:

$$
f(x)=
\begin{cases}
\frac{32}{x^{3}} & x\geq 4 \\
0 & \text{otherwise}
\end{cases}
$$

#### (b)

At most 50 hours:

$$
\begin{aligned}
F(5) =&1-\frac{16}{25} \\
=&0.36
\end{aligned}
$$

At least 60 hours:

$$
\begin{aligned}
1-F(6) =&1-(1-\frac{16}{36}) \\
=&1-0.555555556 \\
=&0.444444444
\end{aligned}
$$

Between 50 and 70 hours:

$$
\begin{aligned}
F(7)-F(5) =&1-\frac{16}{49}-1+\frac{16}{25} \\
=&0.673469388-0.36 \\
=&0.313469388
\end{aligned}
$$

Between 10 and 35 hours:

$$
\begin{aligned}
F(3.5)-F(1) = 0
\end{aligned}
$$

Ans:

At most 50 hours:<br>0.36

At least 60 hours:<br>0.444444444

Between 50 and 70 hours:<br>0.313469388

Between 10 and 35 hours:<br>0

### 3.

Ans:

$Y=X^3:$

$$
\begin{aligned}
G(y) =& G(Y\leq y) \\
=&G(X^3 \leq y) \\
=&G(X\leq \sqrt[3]{y})
\end{aligned}
$$

$$
\begin{aligned}
G(y) =& \int_{-2}^{\sqrt[3]{y}} \frac{1}{4} dx \\
=&\left[\frac{1}{4}x\right]^{\sqrt[3]{y}}_{-2}\\
=&\frac{\sqrt[3]{t}}{4}+\frac{1}{2}
\end{aligned}
$$

$$
G(y)=
\begin{cases}
0 & y\lt-8 \\
\frac{\sqrt[3]{t}}{4}+\frac{1}{2} & -8\leq y\lt 8 \\
1 & y\geq 8
\end{cases}
$$

$$
\begin{aligned}
g(y) =& G'(y) \\
=&\frac{y^{\frac{-2}{3}}}{12}
\end{aligned}
$$

Ans:

$$
g(y)=
\begin{cases}
\frac{y^{\frac{-2}{3}}}{12} & -8\leq y\lt 8 \\
0 & \text{otherwise}
\end{cases}
$$

$Z=X^4:$

$$
\begin{aligned}
H(z) =& H(Z\leq z) \\
=& H(X^4 \leq z) \\
=& H(-\sqrt[4]{z} \leq X \leq \sqrt[4]{z})
\end{aligned}
$$

$$
\begin{aligned}
H(z) =& \int_{-\sqrt[4]{z}}^{\sqrt[4]{z}}\frac{1}{4} dx \\
=&\left[\frac{1}{4}x\right]^{\sqrt[4]{z}}_{-\sqrt[4]{z}} \\
=&\frac{\sqrt[4]{z}}{4}+\frac{\sqrt[4]{z}}{4} \\
=&\frac{\sqrt[4]{z}}{2}
\end{aligned}
$$

$$
H(z) =
\begin{cases}
0 & z\lt 0\\
\frac{\sqrt[4]{z}}{2} & 0\leq z \lt 16 \\
1 & z\geq 16 \\
\end{cases}
$$

$$
\begin{aligned}
h(z) =& H'(z) \\
=&\frac{z^{-\frac{3}{4}}}{8}
\end{aligned}
$$

Ans:

$$
h(z) =
\begin{cases}
\frac{z^{-\frac{3}{4}}}{8} & 0\leq z \lt 16 \\
0 & \text{otherwise} \\
\end{cases}
$$

### 4.

$$
\begin{aligned}
G(Y) =& G(Y \leq y) \\
=& G(\sqrt[3]{X^2} \leq y) \\
=& G(X \leq y^{\frac{3}{2}})
\end{aligned}
$$

$$
\begin{aligned}
G(y) =& \int_{0}^{y^{\frac{3}{2}}} \lambda e^{-\lambda x} dx \\
=& \left[-e^{-\lambda x}\right]^{y^{\frac{3}{2}}}_{0} \\
=& -e^{-\lambda y^{\frac{3}{2}}}+1
\end{aligned}
$$

$$
\begin{aligned}
g(y) =& G'(y) \\
=& (-e^{-\lambda y^{\frac{3}{2}}}+1)' \\
=&\lambda \frac{3}{2}y^{\frac{1}{2}}e^{-\lambda y^{\frac{3}{2}}}
\end{aligned}
$$

Ans:

$$
g(y)=
\begin{cases}
\lambda \frac{3}{2}y^{\frac{1}{2}}e^{-\lambda y^{\frac{3}{2}}} & y \geq 0\\
0 & \text{otherwise}\\
\end{cases}
$$

### 5.

$$
\begin{aligned}
\int_{-\infty}^{\infty} e^x3e^{-3x}dx =& \int_{0}^{\infty} e^x3e^{-2x}dx \\
=&\left[-\frac{3}{2}e^{-2x}\right]^{\infty}_{0} \\
=&0-(-\frac{3}{2}) \\
=&\frac{3}{2}
\end{aligned}
$$

Ans:

$\frac{3}{2}$

### 6.

$$
\begin{aligned}
Var(X) = E(X^2)-E(X)^2
\end{aligned}
$$

$$
\begin{aligned}
E(X)=&\int_{-\infty}^{0}x\frac{1}{2}e^{-|x|} dx+\int_{0}^{\infty} x\frac{1}{2}e^{-|x|}dx \\
=&\int_{-\infty}^{0}x\frac{1}{2}e^{x}dx+\int_{0}^{\infty} x\frac{1}{2}e^{-x}dx \\
=&\frac{1}{2}\left[xe^x-e^x\right]^{0}_{-\infty}-\frac{1}{2}\left[-xe^{-x}-e^{-x}\right]^{\infty}_{0} \\
=&-\frac{1}{2}+\frac{1}{2} \\
=&0
\end{aligned}
$$

$$
\begin{aligned}
\int x\frac{1}{2}e^{x}dx =& \frac{1}{2}(xe^x-\int e^x dx)\\
=&\frac{1}{2}(xe^x-e^x)
\end{aligned}
$$

$$
\begin{aligned}
\int x\frac{1}{2}e^{-x}dx =& \frac{1}{2}(-xe^{-x}-\int -e^{-x} dx)\\
=&\frac{1}{2}(-xe^{-x}-e^{-x})
\end{aligned}
$$

$$
\begin{aligned}
E(X^2) =& \int_{-\infty}^{\infty}x^2\frac{1}{2}e^{-|x|} dx \\
=&\int_{0}^{\infty}x^2e^{-x}dx \\
=&\left[-x^2e^{-x}-\int-2xe^{-x}dx \right]^{\infty}_{0}\\
=&\left[-x^2e^{-x}+2\int xe^{-x} \right]^{\infty}_{0} \\
=&\left[-x^2e^{-x}+2(-xe^{-x}-\int -e^{-x}) \right]^{\infty}_{0} \\
=&\left[-x^2e^{-x}+2(-xe^{-x}-e^{-x}) \right]^{\infty}_{0} \\
=&\left[-x^2e^{-x}-2xe^{-x}-2e^{-x}\right]^{\infty}_{0} \\
=&\left[-(x^2+2x+2)e^{-x}\right]^{\infty}_{0} \\
=&2
\end{aligned}
$$

$$
\begin{aligned}
Var(X)=&2-0^2 \\
=& 2
\end{aligned}
$$

Ans:

2
