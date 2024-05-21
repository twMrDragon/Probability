# 機率 hw8

## 資工二 111590012 林品緯

### 1.

$$
\begin{aligned}
15\times\frac{1}{4} = 3.75
\end{aligned}
$$

Ans:

3.75

### 2.

$$
\begin{aligned}
\int_{\frac{k}{3}}^{\frac{2k}{3}}p(x)dx =& \int_{\frac{k}{3}}^{\frac{2k}{3}}\frac{1}{k}dx \\
=&\left[\frac{x}{k}\right]_{\frac{k}{3}}^{\frac{2k}{3}} \\
=&\frac{2}{3}-\frac{1}{3} \\
=&\frac{1}{3}
\end{aligned}
$$

Ans:

$\frac{1}{3}$

### 3.

$$
\begin{aligned}
G(t) =& P(Y\leq t) \\
=& P(-\ln{(1-x)} \leq t) \\
=& P(x \leq 1-e^{-t})
\end{aligned}
$$

| x   | y        |
| --- | -------- |
| 0   | 0        |
| 1   | $\infty$ |

$$
\begin{aligned}
G(t) =& \int_{0}^{1-e^{-t}} 1 dx \\
=&\left[x \right]_{0}^{1-e^{-t}} \\
=&1-e^{-t}
\end{aligned}
$$

$$
G(t)=
\begin{cases}
1-e^{-t} &  t\geq 0\\
0 & \text{otherwise} \\
\end{cases}
$$

$$
\begin{aligned}
g(t) =& G'(t) \\
=& e^{-t}
\end{aligned}
$$

Ans:

$$
g(t)=
\begin{cases}
e^{-t} &  t\geq 0\\
0 & \text{otherwise} \\
\end{cases}
$$

### 4.

$$
\begin{aligned}
P(x \lt Z \lt x+\alpha) =& P(x+\alpha)-P(x) \\
=&\Phi(x+\alpha)-\Phi(x) \\
=& \frac{1}{\sqrt{2\pi}}\int_{-\infty}^{x+\alpha}e^{-\frac{z^2}{2}}dz-\frac{1}{\sqrt{2\pi}}\int_{-\infty}^{x}e^{-\frac{z^2}{2}}dz \\
=&\frac{1}{\sqrt{2\pi}}\int_{x}^{x+\alpha}e^{-\frac{z^2}{2}}dz
\end{aligned} \\
$$

$$
P'(x \lt Z \lt x+\alpha) = \frac{1}{\sqrt{2\pi}}\left[e^{-\frac{(x+\alpha)^2}{2}}-e^{-\frac{(x)^2}{2}}\right] = 0 \\
$$

$$
e^{-\frac{(x+\alpha)^2}{2}}=e^{-\frac{(x)^2}{2}}
$$

$$
x^2+2x\alpha+\alpha^2 = x^2
$$

$$
2x\alpha+\alpha^2=0
$$

$$
\alpha(2x+\alpha) = 0
$$

$$
x=-\frac{\alpha}{2}
$$

Ans:

$x=-\frac{\alpha}{2}$

### 5.

$\mu = 67$

$\sigma^2 = 64$

$\sigma = 8$

$$
\begin{aligned}
A =& 1-\Phi(\frac{90-67}{8}) \\
=& 1-\Phi(2.875) \\
=& 1-0.9979 \\
=& 0.0021
\end{aligned}
$$

$$
\begin{aligned}
B =& \Phi(\frac{90-67}{8}) - \Phi(\frac{80-67}{8}) \\
=& \Phi(2.875)-\Phi(1.625) \\
=& 0.9979-0.9479 \\
=& 0.0500
\end{aligned}
$$

$$
\begin{aligned}
C =& \Phi(\frac{80-67}{8}) - \Phi(\frac{70-67}{8}) \\
=& \Phi(1.625)-\Phi(0.375) \\
=& 0.9479-0.6461 \\
=& 0.3018
\end{aligned}
$$

$$
\begin{aligned}
D =& \Phi(\frac{70-67}{8}) - \Phi(\frac{60-67}{8}) \\
=& \Phi(0.375)-\Phi(-0.875) \\
=& 0.6461-0.1907\\
=& 0.4554
\end{aligned}
$$

$$
\begin{aligned}
F =& \Phi(\frac{60-67}{8}) \\
=& \Phi(-0.875) \\
=& 0.1907
\end{aligned}
$$

Ans:

| Grade | percent |
| ----- | ------- |
| A     | 0.21%   |
| B     | 5%      |
| C     | 30.18%  |
| D     | 45.54%  |
| F     | 19.07%  |

### 6.

$$
\begin{aligned}
P(|X-\mu| \gt k\sigma) =& P(X-\mu \gt k\sigma)+P(X-\mu \lt -k\sigma) \\
=& P(\frac{X-\mu}{\sigma} \gt k)+P(\frac{X-\mu}{\sigma} \lt -k) \\
=&1-\Phi(k)+\Phi(-k)
\end{aligned}
$$

Ans:

Does not depend on $\mu$ or $\sigma$

### 7.

$$
\begin{aligned}
G(t) =& P(Y \leq t) \\
=& P(\sqrt{|x|} \leq t) \\
=& P(-t^2 \leq x \leq t^2) \\
=& \frac{1}{\sqrt{2\pi}}\int_{-t^2}^{t^2}e^{-\frac{x^2}{2}}dx
\end{aligned}
$$

$$
\begin{aligned}
g(t) =& \frac{1}{\sqrt{2\pi}}\left[e^{-\frac{t^4}{2}}\times (2t-(-2t)) \right] \\
=& \frac{4t}{\sqrt{2\pi}}e^{-\frac{t^4}{2}}
\end{aligned}
$$

Ans:

$$
g(t)=
\begin{cases}
\frac{4t}{\sqrt{2\pi}}e^{-\frac{t^4}{2}} & t \geq 0 \\
0 & \text{otherwise}
\end{cases}
$$

### 8.

$E(x)=\frac{1}{\lambda}$

$Var(x)=\frac{1}{\lambda^2}$

$\sigma_x=\frac{1}{\lambda}$

$$
\begin{aligned}
P(|X-E(X)| \gt 2\sigma_x) =& P(X-E(X) \gt 2\sigma_x)+ P(X-E(X) \lt -2\sigma_x) \\
=&P(\frac{2}{\lambda}+\frac{1}{\lambda})+P(-\frac{2}{\lambda}+\frac{1}{\lambda}) \\
=&P(\frac{3}{\lambda}) + P(-\frac{1}{\lambda}) \\
=&P(\frac{3}{\lambda}) \\
=&1-\int_{0}^{\frac{3}{\lambda}}\lambda e^{-\lambda x}dx \\
=&1+\left[e^{-\lambda x} \right]_{0}^{\frac{3}{\lambda}} \\
=&1+(e^{-3}-1) \\
=&e^{-3}
\end{aligned}
$$

Ans:

$e^{-3}$

### 9.

$$
\begin{aligned}
P(\lfloor X \rfloor = n) =& P(n \leq X \lt n+1) \\
=&\int_{n}^{n+1}\lambda  e^{-\lambda x}dx \\
=&\left[-e^{-\lambda x} \right]_{n}^{n+1} \\
=&-e^{-\lambda (n+1)}+e^{-\lambda n} \\
=&(e^{^{-\lambda}})^{n}(1-e^{^{-\lambda}})
\end{aligned}
$$

Ans:

$p=1-e^{-\lambda}$
