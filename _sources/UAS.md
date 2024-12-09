---
title: UAS

---

### No 1. Tentukan $(P\implies Q)$ & $(R\implies S)$
||No| P| Q | R|S |$P\implies Q$  |$R\implies S$|Hasilnya|
|--|--|---|--|--|--|--|--|--|
|1| True | True | False | False|T| T | T|
|2| False| True | True | False |T|F |F|
|3| False| True | True | True  |T|T |T|
|4| True | False|  False| False |F| T |T|
|5| False| True | False| True  |T| T |F|
|6| True | False|  True | False |F| F |T|
|7| False| False| True  | True  |T| T |T|
|8| True | True | False | False |T| T |T|


### No 2. 
1. Hitung Closeness Centrality :  G
2. Hitung Betweness Centrality :  F
 
### Jawaban no 1:
![](https://cdn.mathpix.com/snip/images/Wp9V_FkhgYUYVXbOhqzRJZY_wUOC6yC1PXnKJ3Y7VjY.original.fullsize.png)

- $$C_C\left(v_i\right)=\left[\frac{1}{n-1} \sum_{j \neq i}^n g\left(v_i, v_j\right)\right]^{-1}=\frac{n-1}{\sum_{j \neq i}^n g\left(v_i, v_j\right)}$$

$G - A = 6$
$G - B = 5$
$G - C = 4$
$G - D = 3$
$G - E = 2$
$G - F = 1$
$Total = 21$
 
- $Cc(G)=\frac{n-1}{\sum_{j \neq i}^n g\left(v_i, v_j\right)} =\frac{7-1}{\sum_{j \neq i}^n g\left(v_i, v_j\right)}= \frac{6}{21}$ = 0,2857$

### Jawaban no 2:
 $$
C_B\left(v_i\right)=\sum_{v_s \neq v_i \neq v_t \in V, s<t} \frac{\sigma_{s t}\left(v_i\right)}{\sigma_{s t}}
$$
