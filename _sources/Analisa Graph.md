---
title: Analisa Graph

---

* ###  Social Network Analysis
Social Network Analysis (SNA) adalah metode untuk mempelajari  hubungan antara individu, kelompok, atau entitas lain dalam suatu jaringan sosial dengan menggunakan teori graf. Implementasi Social Network Analysis yaitu dapat menjelaskan relasi atau hubungan antara aktor melalui visualisasi berbentuk graf. Relasi dalam analisis jaringan sosial dapat diproses dalam bentuk perhitungan yang disebut centrality. centrality adalah ukuran untuk mengetahui seberapa penting atau berpengaruhnya sebuah node dalam jaringan.
* ### Social Network 
Terdapat node yang mewakili orang atau individu atau aktor. 
Relasi  antar objek  dapat dinyatakan dengan link atau edges yang terjadi antara aktor tersebut. Social network terdiri dari banyak aktor yang mempunyai relasi satu sama lain hingga membentuk peta jaringan sosial yang dinyatakan dengan graph.

![original image](https://cdn.mathpix.com/snip/images/2XgBue-ahlsabJv_kV0h96Nlm_emFcgFAkteEwcPeaY.original.fullsize.png)

Table 1.1 : Adjacency Matrix
| Node |1|2|3|4|5|6|7|8|9|
|----- |-|-|-|-|-|-|-|-|-|
|  1   |-|1|1|1|0|0|0|0|0|
|  2   |1|-|1|0|0|0|0|0|0|
|  3   |1|1|-|1|0|0|0|0|0|
|  4   |1|0|1|-|1|1|0|0|0|
|  5   |0|0|0|1|-|1|1|1|0|
|  6   |0|0|0|1|1|-|1|1|0|
|  7   |0|0|0|0|1|1|-|1|1|
|  8   |0|0|0|0|1|1|1|-|0|
|  9   |0|0|0|0|0|0|1|0|-|
* Tidak semua node dalam jaringan adalah penting(aktor)
* Dalam suatu jaringan, mencari node itu sangatlah penting
* Centrality adalah penentuan aktor menggunakan ukuran pada Social Networ Centrality dalam teori graf dan social network, dibagi menjadi empat jenis yaitu : 
1. Degree centrality
2. Betweeness centrality
3. Cloness centrality
4. Eigenvector centrality

* ### Degree Centrality
Degree centrality adalah ukuran sentralitas dalam jaringan yang mengukur seberapa banyak suatu node terhubung dengan node lainnya. 
pentingnya node ditentukan oleh jumlah node yang berdekatan dengan node tersebut : lebih besar derajatnya (degree) maka lebih penting node itu dalam suatu jaringan dan hanya sebagian kecil node yang memiliki derajat tinggi dalam jaringan.
* Degree Centrality:
$$C_D\left(v_i\right)=d_i=\sum_i A_{i j}$$
* Normalisasi Degree Centrality:
 $C_D^{\prime}\left(v_i\right)=d_i /(n-1)$

untuk node 1, degree centrality adalah 3 dan untuk Normalisasi degree centrality adalah 3/(9-1) = 3/8.

* ### Closeness Centrality
Closeness centrality adalah nilai yang menunjukkan seberapa dekat suatu node dengan node yang lain dalam jaringan dengan menghitung rata-rata dari jarak relasi node-node tersebut. Skor closeness centrality mewakili kecepatan dalam penyebaran informasi.
* Average Distance: 
 $D_{\text {avg }}\left(v_i\right)=\frac{1}{n-1} \sum_{j \neq i}^n g\left(v_i, v_j\right)$
*  Closeness Centrality:
$$C_C\left(v_i\right)=\left[\frac{1}{n-1} \sum_{j \neq i}^n g\left(v_i, v_j\right)\right]^{-1}=\frac{n-1}{\sum_{j \neq i}^n g\left(v_i, v_j\right)}$$

* Contoh Closeness Centrality
$$\begin{gathered}
C_C(3)=\frac{9-1}{1+1+1+2+2+3+3+4}=8 / 17=0.47 \\
C_C(4)=\frac{9-1}{1+2+1+1+1+2+2+3}=8 / 13=0.62
\end{gathered}$$
Node 4 lebih central dari node 3

Table 1.2 : Pairwise geodesic distance
| Node |1|2|3|4|5|6|7|8|9|
|------|-|-|-|-|-|-|-|-|-|
|  1   |0|1|1|1|2|2|3|3|4|
|  2   |1|0|1|2|3|3|4|4|5|
|  3   |1|1|0|1|2|2|3|3|4| 
|  4   |1|2|1|0|1|1|2|2|3|
|  5   |2|3|2|1|0|1|1|1|2|
|  6   |2|3|2|1|1|0|1|1|2|
|  7   |3|4|3|2|1|1|0|1|1|
|  8   |3|4|3|2|1|1|1|0|2|
|  9   |4|5|4|3|2|2|1|2|0|

* ### Betweenness Centrality
Betweenness centrality adalah ukuran yang menunjukkan seberapa besar kemampuan suatu node dalam mengendalikan aliran informasi antara node-node lain dalam jaringan.
* Semakin banyak lintasan yang harus melewati persimpangan itu (misal tidak ada jalan alternatif), maka semakin penting arti persimpangan tersebut. Hal ini menandakan seberapa besar suatu node diperlukan sebagai penghubung dalam penyebaran informasi di dalam jaringan.
* Ukuran ini juga dapat digunakan untuk mengidentifikasi boundary spanners, yaitu orang atau node yang berperan sebagai penghubung (jembatan) antara dua komunitas.

* Menghitung jumlah lintasan terpendek yang melewati suatu node
* Node dengan betwenneess tinggi adalah penting dalam komunikasi dan penyebaran informasi
* Betweenness Centrality
$$
C_B\left(v_i\right)=\sum_{v_s \neq v_i \neq v_t \in V, s<t} \frac{\sigma_{s t}\left(v_i\right)}{\sigma_{s t}}
$$
$\sigma_{s t}$ Jumlah lintasan terpendek antara s dan t 
$\sigma_{s t}\left(v_i\right)$ Jumlah lintasan terpendek antara $s$ dan $t$ yang melewati $\mathrm{v}_{\mathrm{i}}$

![original image](https://cdn.mathpix.com/snip/images/2XgBue-ahlsabJv_kV0h96Nlm_emFcgFAkteEwcPeaY.original.fullsize.png)$C_B(4)=15$


|  | *s* = 1 | *s* = 2 | *s* = 3 |
|--|-------- |-------- |-------- |
| *t* = 5 | 1/1 | 2/2 | 1/1 |
| *t* = 6 | 1/1 | 2/2 | 1/1 |
| *t* = 7 | 2/2 | 4/4 | 2/2 |
| *t* = 8 | 2/2 | 4/4 | 2/2 |
| *t* = 9 | 2/2 | 4/4 | 2/2 |

Normalisasi Betweenness Centrality :
$$C_B^{\prime}(i)=\frac{C_B(i)}{(n-1)(n-2) / 2} .$$

* ### Eigenvector centrality
metode untuk mengukur seberapa penting suatu node dalam jaringan berdasarkan koneksi dengan node-node penting lainnya. Metode ini digunakan untuk mencari node yang paling populer atau berpengaruh dalam jaringan sosial.


