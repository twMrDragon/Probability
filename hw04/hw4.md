# 機率 hw4

## 資工二 111590012 林品緯

### 1.

$A$ = 選到第一疊牌

$B$ = 選到第二疊牌

$E$ = 選中三張紅色牌

$$
\begin{aligned}
P(E)=&P(E \cap A)+P(E\cap B) \\
=&P(E|A)P(A)+P(E|B)P(B) \\
=&\frac{6}{11}\times\frac{5}{10}\times\frac{4}{9}\times\frac{1}{2}+1\times\frac{1}{2} \\
=&\frac{1110}{1980}
\end{aligned}
$$

$$
\begin{aligned}
P(E\cap A)=&P(E|A)P(A) \\
=&\frac{6}{11}\times\frac{5}{10}\times\frac{4}{9}\times\frac{1}{2} \\
=&\frac{120}{1980}
\end{aligned}
$$

$$
\begin{aligned}
\frac{P(E\cap A)}{P(E)} =& \frac{\frac{120}{1980}}{\frac{1110}{1980}} \\
=&\frac{120}{1110} \\
=&0.108
\end{aligned}
$$

Ans:<br>
0.108

### 2.

$E$ = 最後抽到藍色

$$
\begin{aligned}
P(E)=&P(E\cap RRRR)+P(E\cap BRRR)+P(E\cap BBRR)+P(E\cap BBBR) \\
=&P(E|RRRR)P(RRRR)+P(E|BRRR)P(BRRR)+P(E|BBRR)P(BBRR)\\
+&P(E|BBBR)P(BBBR) \\
=&0\times\frac{5}{8}\times\frac{4}{7}\times\frac{3}{6}\times\frac{2}{5}\times C^4_4 \\
+&\frac{1}{4}\times\frac{3}{8}\times\frac{5}{7}\times\frac{4}{6}\times\frac{3}{5}\times C^4_3 \\
+&\frac{2}{4}\times\frac{3}{8}\times\frac{2}{7}\times\frac{5}{6}\times\frac{4}{5}\times C^4_2 \\
+&\frac{3}{4}\times\frac{3}{8}\times\frac{2}{7}\times\frac{1}{6}\times\frac{5}{5}\times C^4_1 \\
=&\frac{0+720+1440+360}{6720} \\
=&\frac{2520}{6720}
\end{aligned}
$$

$$
\begin{aligned}
\frac{P(E\cap BBRR)}{P(E)} =& \frac{\frac{1440}{6720}}{\frac{2520}{6720}} \\
=&\frac{1440}{2520} \\
=&0.571429
\end{aligned}
$$

Ans:<br>
0.571429

### 3.

$A$ = 加總為奇數

$B$ = 第一次骰到 2

(1,2),(1,4),(1,6),
(2,1),(2,3),(2,5),
(3,2),(3,4),(3,6),
(4,1),(4,3),(4,5),
(5,2),(5,4),(5,6),
(6,1),(6,3),(6,5)
$$P(A) = \frac{18}{36}$$

(2,1),(2,2),(2,3),(2,4),(2,5),(2,6),
$$P(B) = \frac{6}{36}$$

$$P(A\cap B)=\frac{3}{36}$$

$$
\begin{aligned}
P(A)P(B)=&\frac{18}{36}\times \frac{6}{36} \\
=&\frac{3}{36}
\end{aligned}
$$

$$P(A \cap B) = P(A)P(B)$$

Ans:<br>
是獨立的

### 4.

$A$ = 目標被導彈 1 擊中

$B$ = 目標被導彈 2 擊中

$C$ = 目標被導彈 3 擊中

$E$ = 目標被擊中至少 1 次

$$
\begin{aligned}
P(E)=&1-P(A^c)P(B^c)P(C^c) \\
=&1-(1-0.7)\times(1-0.8)\times(1-0.9) \\
=&1-0.006 \\
=&0.994
\end{aligned}
$$

Ans:<br>
0.994

### 5.

$S$ = 實驗成功

$F$ = 實驗失敗

$$
\begin{aligned}
0.5904=&1-P(F)^4 \\
P(F)^4=&0.4096 \\
P(F)=&0.8 \\
P(S)=&0.2
\end{aligned}
$$

Ans:<br>
0.2

### 6.

$S$ = 實驗成功

$F$ = 實驗成功

$E$ = 實驗成功至少 1 次

$$
\begin{aligned}
P(E)=&1-P(F)^6 \\
=&1-\left(\frac{5}{6}\right)^6 \\
=&1-0.334897977\\
=&0.665102023
\end{aligned}
$$

Ans:<br>
0.665102023

### 7.

$E$ = 擲到人頭比抽到 A 早出現

$H$ = 硬幣擲到人頭

$A$ = 抽到 A

$$
\begin{aligned}
P(E)=&P(E\cap H)+P(E\cap H^cA)+P(E\cap H^cA^c) \\
=&P(E|H)P(H)+P(E|H^cA)P(H^cA)+P(E|H^cA^c)P(H^cA^c) \\
=&1\times\frac{1}{2}+0\times\frac{1}{2}\times\frac{4}{52}+P(E)\times\frac{1}{2}\times\frac{48}{52} \\
=&\frac{1}{2}+\frac{24}{52}\times P(E)
\end{aligned}
$$

$$\frac{28}{52}\times P(E)=\frac{1}{2}$$
$$P(E)=\frac{26}{28}$$

Ans:<br>
$\frac{26}{28}$
