# 機率 hw6

## 資工二 111590012 林品緯

### 1.

$$
\begin{aligned}
P=&\binom{6}{3}\times\left(\frac{2}{12}\right)^3\times\left(\frac{10}{12}\right)^3 \\
=&0.053583676
\end{aligned}
$$

Ans:

0.053583676

### 2.

$$
\begin{aligned}
k\leq&(n+1)p \\
k\leq&11*0.45\\
k\leq&4.95
\end{aligned}
$$

$$
\begin{aligned}
p=&\binom{10}{4}\times0.45^4\times0.55^6 \\
=&0.238366647
\end{aligned}
$$

Ans:

$k=4$

$p=0.238366647$

### 3.

當 parity check 發收偶數位錯誤時不會檢查出錯誤。

$$
\begin{aligned}
P=&\sum^{4}_{n=1}\binom{8}{2n}\times(1-0.999)^{2n}\times(0.999)^{8-2n} \\
=&0.0000278325
\end{aligned}
$$

Ans:

0.0000278325

### 4.

$$
\begin{aligned}
\lambda=&80\times0.025 \\
=&2
\end{aligned}
$$

$$
\begin{aligned}
P(X\geq 2)=&1-P(X=0)-P(X=1)\\
=&1-\frac{e^{-2}\times2^0}{0!}-\frac{e^{-2}\times2^1}{1!}\\
=&0.59399415
\end{aligned}
$$

Ans:

0.59399415

### 5.

$$
\begin{aligned}
\lambda=&\frac{3}{10}\times 35 \\
=&10.5
\end{aligned}
$$

$$
\begin{aligned}
P(X=10)=&\frac{e^{-10.5}\times10.5^{10}}{10!} \\
=&0.123605529
\end{aligned}
$$

$$
\begin{aligned}
[P(X=10)]^2=&0.123605529^{2} \\
=&0.015278327
\end{aligned}
$$

Ans:

0.015278327

### 6.

$$
\begin{aligned}
P(X=1)=&P(X=3) \\
\frac{e^{-\lambda}\times\lambda^1}{1!}=&\frac{e^{-\lambda}\times\lambda^3}{3!} \\
6=&\lambda^2\\
\lambda=&\sqrt{6}
\end{aligned}
$$

$$
\begin{aligned}
P(X=5)=&\frac{e^{-\sqrt{6}}\times\sqrt{6}^5}{5!}\\
=&0.063444941
\end{aligned}
$$

Ans:

0.063444941

### 7.

$$
\begin{aligned}
P=&\binom{7}{2}\times0.2^3\times0.8^5 \\
=&0.05505024
\end{aligned}
$$

Ans:

0.05505024

### 8.

Ans:

$p^{n-1}$

### 9.

最後一個是第 10 個老年人。在第 10 個老人以前，會有 9 個老人和 x 個非老人。

$$
\begin{aligned}
P=&\binom{x+9}{9}\times0.15^{10}\times0.85^{x}
\end{aligned}
$$

Ans:

$$
P=
\begin{cases}
\binom{x+9}{9}\times0.15^{10}\times0.85^{x} & x\geq0 \\
0 & \text{otherwise}
\end{cases}
$$

### 10.

$$
\begin{aligned}
P_n = \frac{\binom{50}{4}\times\binom{N-50}{46}}{\binom{N}{50}}
\end{aligned}
$$

$$
\begin{aligned}
P_{n+1} =& \frac{\binom{50}{4}\times\binom{N+1-50}{46}}{\binom{N+1}{50}} \\
=& \frac{\binom{50}{4}\times\binom{N-49}{46}}{\binom{N+1}{50}}
\end{aligned}
$$

$$
\begin{aligned}
P_{n-1} =& \frac{\binom{50}{4}\times\binom{N-1-50}{46}}{\binom{N-1}{50}} \\
=&\frac{\binom{50}{4}\times\binom{N-51}{46}}{\binom{N-1}{50}}
\end{aligned}
$$

$$
\begin{aligned}
\frac{P_n}{P_{n+1}}=&\frac{\binom{50}{4}\times\binom{N-50}{46}}{\binom{N}{50}}\times\frac{\binom{N+1}{50}}{\binom{50}{4}\times\binom{N-49}{46}} \\
=&\frac{(N-50)!}{46!\times(N-96)!}\times\frac{50!(N-50)!}{N!}\times\frac{(N+1)!}{50!(N-49)!}\times\frac{46!\times(N-95)!}{(N-49)!} \\
=&\frac{(N+1)\times(N-95)}{(N-49)\times(N-49)} \\
\end{aligned}
$$

$$
\begin{aligned}
\frac{P_n}{P_{n+1}}\geq& 1 \\
\frac{(N+1)\times(N-95)}{(N-49)\times(N-49)}\geq& 1 \\
N^2-94N-95\geq& N^2-98N+2401 \\
4N\geq&2496 \\
N\geq& 624
\end{aligned}
$$

$$
\begin{aligned}
\frac{P_n}{P_{n-1}}=&\frac{\binom{50}{4}\times\binom{N-50}{46}}{\binom{N}{50}}\times\frac{\binom{N-1}{50}}{\binom{50}{4}\times\binom{N-51}{46}} \\
=&\frac{(N-50)!}{46!\times(N-96)!}\times\frac{50!(N-50)!}{N!}\times\frac{(N-1)!}{50!(N-51)!}\times\frac{46!\times(N-97)!}{(N-51)!} \\
=&\frac{(N-50)\times(N-50)}{N\times(N-96)} \\
\end{aligned}
$$

$$
\begin{aligned}
\frac{P_n}{P_{n-1}}\geq& 1 \\
\frac{(N-50)\times(N-50)}{N\times(N-96)}\geq& 1 \\
N^2-100N+2500\geq& N^2-96N \\
2500\geq&4N \\
625\geq&N
\end{aligned}
$$

$625\geq N \geq 624$

Ans:

$N= 624$ or $625$
