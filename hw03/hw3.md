# 機率 hw3

## 資工二 111590012 林品緯

### 1.

總共有 :

$$
\begin{aligned}
C^{20}_6 = 38760
\end{aligned}
$$

沒有一組鞋子的數量 :

$$
\begin{aligned}
C^{10}_6 \times 2^6 =& 210\times 64 \\
                    =& 13440
\end{aligned}
$$

沒有一組鞋子的機率 :

$$
\begin{aligned}
P =& \frac{13440}{38760} \\
  =& 0.34675
\end{aligned}
$$

Ans:<br>
0.34675

剛好一組鞋子的數量 :

$$
\begin{aligned}
C^{10}_1 \times C^{9}_4 \times 2^4 =& 10 \times 126\times 32 \\
                                   =& 20160
\end{aligned}
$$

剛好一組鞋子的機率 :

$$
\begin{aligned}
P =& \frac{20160}{38760} \\
  =& 0.520
\end{aligned}
$$

Ans:<br>
0.520

### 2.

coefficient of $x^2y^3z^2$ :

$$
\begin{aligned}
&2^2\times(-1)^3\times 3^2\times \frac{7!}{2!\times 3!\times 2!} \\
                   =&4\times(-1)\times 9\times 210 \\
                   =&-7560
\end{aligned}
$$

Ans:<br>
-7560

### 3.

總共有 :

$$
\begin{aligned}
C^9_3 \times C^8_4 =& 84 \times 70 \\
                   =& 5880
\end{aligned}
$$

選到兩個不合女生 :

$$
\begin{aligned}
C^9_3 \times C^6_2 =& 84 \times 15 \\
                   =& 1260
\end{aligned}
$$

沒有選到兩個不合的女生 :

$$
\begin{aligned}
5880-1260=4620
\end{aligned}
$$

Ans:<br>
4620

### 4.

總共有 :

$$
\begin{aligned}
6^6=46656
\end{aligned}
$$

包含兩個 6 的數量 :

$$
\begin{aligned}
C^6_2 \times 5^4 =& \frac{6!}{2!\times4!}\times 625 \\
                 =&15 \times 625 \\
                 =& 9375
\end{aligned}
$$

包含兩個 6 的機率為:

$$
\begin{aligned}
P=&\frac{9375}{46656} \\
 =&0.201
\end{aligned}
$$

Ans:<br>
0.201

### 5

假設我們有 A、B 兩個集合，A 集合裡有 n 個元素，B 集合裡有 m 個元素。從兩個集合取出 r 個元素有 $\binom{m+n}{r}ab$ 種情況。當我們從集合 A 取出 r 個元素，從集合 B 取出 0 個元素的情況，即 $\binom{m}{0}\binom{n}{r}$ 。當我們從集合 A 取出 r-1 個元素，從集合 B 取出 1 個元素的情況，即 $\binom{m}{1}\binom{n}{r-1}$ 。一直到當我們從集合 A 取出 0 個元素，從集合 B 取出 r 個元素的情況，即 $C^m_rC^n_0$ 。全部加總即為我們從 A、B 集合取出 r 個元素的情況，即 $\binom{n+m}{r}=\sum^r_{i=0}\binom{m}{i}\binom{n}{r-i}$。

### 6.

總共有 :

$$
\begin{aligned}
C^{12}_{7} = 792
\end{aligned}
$$

兩顆黃球都被取出來的數量 :

$$
\begin{aligned}
C^{10}_{5} = 252
\end{aligned}
$$

至少一顆黃球在箱子裡的機率 :

$$
\begin{aligned}
P=& 1-\frac{252}{792} \\
 =& 0.682
\end{aligned}
$$

Ans:<br>
0.682

### 7.

$$
\begin{aligned}
P(D_1D_2D_3D_4) =& P(D_1)P(D_2|D_1)P(D_3|D_1D_2)P(D_4|D_1D_2D_3) \\
                =& \frac{8}{20} \times \frac{7}{19} \times \frac{6}{18} \times \frac{5}{17} \\
                =& 0.014447884
\end{aligned}
$$

Ans:<br>
0.014447884

$$
\begin{aligned}
 &P(D_1D_2D_3 \cup D_1D_2N_3 \cup D_1N_2D_3 \cup N_1D_2D_3) \\
=&P(D_1D_2D_3)+P(D_1D_2N_3)+P(D_1N_2D_3)+P(N_1D_2D_3) \\
=&P(D_1)P(D_2|D_1)P(D_3|D_1D_2) \\
 &+P(D_1)P(D_2|D_1)P(N_3|D_1D_2) \\
 &+P(D_1)P(N_2|D_1)P(D_3|D_1N_2) \\
 &+P(N_1)P(D_2|N_1)P(D_3|N_1D_2) \\
=&\frac{8}{20}\times\frac{7}{19}\times\frac{6}{18}+\frac{8}{20}\times\frac{7}{19}\times\frac{12}{18}+\frac{8}{20}\times\frac{12}{19}\times\frac{7}{18}+\frac{12}{20}\times\frac{8}{19}\times\frac{7}{18} \\
=&0.343859649
\end{aligned}
$$

Ans:<br>
0.343859649

### 8.

$E$ = 第 10 抽是紅心情況

$F$ = 前 9 抽出現 3 張紅心的情況

$$
\begin{aligned}
P(F) =& \frac{C^{13}_3\times C^{39}_6}{C^{52}_9}
\end{aligned}
$$

$$
\begin{aligned}
P(E|F) =& \frac{10}{43}
\end{aligned}
$$

$$
\begin{aligned}
P(FE) =& P(F)P(E|F) \\
      =& \frac{C^{13}_3\times C^{39}_6}{C^{52}_9} \times \frac{10}{43} \\
      =& 0.058982854
\end{aligned}
$$

Ans:<br>
0.058982854

### 9.

$D$ = 有駕駛證

$M$ = 男生

$W$ = 女生

$$
\begin{aligned}
P(D) =& P(D|M)P(M)+P(D|W)P(W) \\
     =& 0.2 \times 0.4 + 0.16 \times 0.6 \\
     =& 0.08+0.096 \\
     =& 0.176
\end{aligned}
$$

Ans:<br>
0.176

### 10.

$E$ = 抽到黑桃

$L$ = 遺失的是黑桃

$$
\begin{aligned}
P(E) =& P(EL)+P(EL^c) \\
     =& P(E|L)P(L)+P(E|L^c)P(L^c) \\
     =& \frac{12}{51}\times\frac{13}{52}+\frac{13}{51}\times\frac{39}{52} \\
     =& 0.25
\end{aligned}
$$

Ans:<br>
0.25

### 11.

$N$ = 新的球

$O$ = 舊的球

$$
\begin{aligned}
P(N) =& P(N_1N_2N_3N_4N_5N_6)+(N_1N_2O_3N_4N_5N_6)+(N_1O_2N_3N_4N_5N_6)+(O_1N_2N_3N_4N_5N_6) \\
+&(N_1O_2O_3N_4N_5N_6)+(O_1O_2N_3N_4N_5N_6)+(O_1N_2O_3N_4N_5N_6)+(O_1O_2O_3N_4N_5N_6) \\
=&P(N_1)P(N_2|N_1)P(N_3|N_1N_2)P(N_4|N_1N_2N_3)P(N_5|N_1N_2N_3N_4)P(N_6|N_1N_2N_3N_4N_5) \\
+&P(N_1)P(N_2|N_1)P(O_3|N_1N_2)P(N_4|N_1N_2O_3)P(N_5|N_1N_2O_3N_4)P(N_6|N_1N_2O_3N_4N_5) \\
+&P(N_1)P(O_2|N_1)P(N_3|N_1O_2)P(N_4|N_1O_2N_3)P(N_5|N_1O_2N_3N_4)P(N_6|N_1O_2N_3N_4N_5) \\
+&P(O_1)P(N_2|O_1)P(N_3|O_1N_2)P(N_4|O_1N_2N_3)P(N_5|O_1N_2N_3N_4)P(N_6|O_1N_2N_3N_4N_5) \\
+&P(N_1)P(O_2|N_1)P(O_3|N_1O_2)P(N_4|N_1O_2O_3)P(N_5|N_1O_2O_3N_4)P(N_6|N_1O_2O_3N_4N_5) \\
+&P(O_1)P(O_2|O_1)P(N_3|O_1O_2)P(N_4|O_1O_2N_3)P(N_5|O_1O_2N_3N_4)P(N_6|O_1O_2N_3N_4N_5) \\
+&P(O_1)P(N_2|O_1)P(O_3|O_1N_2)P(N_4|O_1N_2O_3)P(N_5|O_1N_2O_3N_4)P(N_6|O_1N_2O_3N_4N_5) \\
+&P(O_1)P(O_2|O_1)P(O_3|O_1O_2)P(N_4|O_1O_2O_3)P(N_5|O_1O_2O_3N_4)P(N_6|O_1O_2O_3N_4N_5) \\
=&\frac{8}{18}\times\frac{7}{17}\times\frac{6}{16}\times\frac{5}{18}\times\frac{4}{17}\times\frac{3}{16} \\
+&\frac{8}{18}\times\frac{7}{17}\times\frac{10}{16}\times\frac{6}{18}\times\frac{5}{17}\times\frac{4}{16} \\
+&\frac{8}{18}\times\frac{10}{17}\times\frac{7}{16}\times\frac{6}{18}\times\frac{5}{17}\times\frac{4}{16} \\
+&\frac{10}{18}\times\frac{8}{17}\times\frac{7}{16}\times\frac{6}{18}\times\frac{5}{17}\times\frac{4}{16} \\
+&\frac{8}{18}\times\frac{10}{17}\times\frac{9}{16}\times\frac{7}{18}\times\frac{6}{17}\times\frac{5}{16} \\
+&\frac{10}{18}\times\frac{9}{17}\times\frac{8}{16}\times\frac{7}{18}\times\frac{6}{17}\times\frac{5}{16} \\
+&\frac{10}{18}\times\frac{8}{17}\times\frac{9}{16}\times\frac{7}{18}\times\frac{6}{17}\times\frac{5}{16} \\
+&\frac{10}{18}\times\frac{9}{17}\times\frac{8}{16}\times\frac{8}{18}\times\frac{7}{17}\times\frac{6}{16} \\
=& 0.038266532
\end{aligned}
$$

Ans:<br>
0.038266532
