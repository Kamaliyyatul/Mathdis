---
title: UAS

---

# UAS

## No 1. Tentukan $(P\implies Q)$ $\implies$ $(R\implies S)$
|No|P| Q| R | S|$P\implies Q$  | $R\implies S$|Hasilnya|
|--|--|---|--|--|--|--|--|
|1| True | True | False | False|T| T | T|
|2| False| True | True | False |T|F |F|
|3| False| True | True | True  |T|T |T|
|4| True | False|  False| False |F| T |T|
|5| False| True | False| True  |T| T |F|
|6| True | False|  True | False |F| F |T|
|7| False| False| True  | True  |T| T |T|
|8| True | True | False | False |T| T |T|


## No 2. 
1. Hitung Closeness Centrality :  G
2. Hitung Betweness Centrality :  F
 
### Jawaban no 1:
![](https://cdn.mathpix.com/snip/images/Wp9V_FkhgYUYVXbOhqzRJZY_wUOC6yC1PXnKJ3Y7VjY.original.fullsize.png)

- $$C_C\left(v_i\right)=\left[\frac{1}{n-1} \sum_{j \neq i}^n g\left(v_i, v_j\right)\right]^{-1}=\frac{n-1}{\sum_{j \neq i}^n g\left(v_i, v_j\right)}$$

G - A = 6

G - B = 5

G - C = 4

G - D = 3

G - E = 2

G - F = 1

Total = 21
 
$Cc(G)=\frac{n-1}{\sum_{j \neq i}^n g\left(v_i, v_j\right)} =\frac{7-1}{\sum_{j \neq i}^n g\left(v_i, v_j\right)}= \frac{6}{21}$ = $0,2857$

### Jawaban no 2:

Pasangan Node yang melewati F :

Pasangan (A,G) = A, B, C, D, E, F, G

Pasangan (B,G) =  B, C, D, E, F, G

Pasangan (C,G) = C, D, E, F, G

Pasangan (D,G) = D, E, F, G

Pasangan (E,G) = E, F, G

Total ada 5 pasangan yang melewati Node F

Normalisasi Betweenness Centrality :

$$
C_B^{\prime}(F)=\frac{C_B(F)}{(n-1)(n-2) / 2} = \frac{5}{(7-1)(7-2) / 2}= \frac{5}{6*5 / 2} =\frac{5}{15}= 0,3334
$$
