---
title: Aljabar Boolean dan Gerbang Logika

---

 **Aljabar Boolean dan Gerbang Logika**
Aljabar boolean adalah struktur aljabar yang menghubunngkan dengan variabel-variabel biner yang hanya meiliki dua nilai, yaitu benar (1) dan salah (0), dan dioperasikan dengan operasi logika seperti and, or, dan not.
**Gerbang Logika**
Gerbang logika adalah memasukkan input yang diproses dan hasilnya dalam tabel kebenaran.
**Operator Biner**
Operator biner adalah jenis bilangan yang hanya bisa terdiri dari dua jenis angka yitu 0 dan 1. Aljabar boolean memiliki dua operator biner:
1.Penjumlahan(+): Digunakan untuk operasi disjungsi (OR).
2.Perkalian(.): Digunakan untuk operasi konjungsi (AND)
**Operator Uner**
Operator uner adalah operasi yang hanya melibatkan satu operand, yaitu satu input.
1.Komplemen ('): Digunakan untuk menghasilkan nilai yang berlawanan dari suatu elemen. Misalnya, jika a=1, maka a=0, dan sebaliknya.
**Aksioma**
Aksioma adalah pernyataan yang diterima sebagai kebenaran dasar tanpa perlu pembuktian dalam suatu sistem logika atau matematika.
Untuk setiap a, b, c ∈ B, berlaku aksioma-aksioma berikut:
* Closure: a + b ∈ B dan a ⋅ b ∈ B.
* Identitas: a + 0 = a dan a ⋅ 1 = a.
* Komutatif: a + b = b + a dan a ⋅ b = b ⋅ a.
* Distributif: a ⋅ (b + c) = (a ⋅ b) + (a ⋅ c) dan a + (b ⋅ c) = (a + b) ⋅ (a + c).
* Komplemen: Untuk setiap a ∈ B, terdapat elemen unik a’ ∈ B sehingga a + a’ = 1 dan a ⋅ a’ = 0
**Tabel Kebenaran untuk Operator Boolean**
A AND Y

| X | Y | XY |
|---|---|----|
| 0 | 0 | 0  |
| 0 | 1 | 0  |
| 1 | 0 | 0  |
| 1 | 1 | 1  |

A OR Y

| X | Y | X+Y |
|---|---|-----|
| 0 | 0 | 0   |
| 0 | 1 | 1   |
| 1 | 0 | 1   |
| 1 | 1 | 1   |

**Boolean Algebra**
Boolean algebra adalah aljabar dimana nilai variabel merupakan nilai kebenaran, benar dan salah, yang biasanya dilambangkan dengan 1 dan 0.

NOT X
| X | $$\overline X$$ |
| -------- | -------- | 
| 0        | 1        | 
| 1        | 0        |

**Berikut adalah fungsi Boolean:**
* Memiliki satu variabel boolean
* Memiliki satu operator boolean
* Memiliki satu input dari himpunan{0,1}.

Tabel kebenaran untuk untuk fungsi Boolean:
 $$F(x,y,z)=x\overline{z}+y$$

| X | Y | Z | $$\overline Z$$| $$X\overline Z$$| $$X\overline Z+Y$$ |
| ----- | -------| -------| ---  |---|---|
| 0 | 0 | 0 | 1 | 0 | 0 |    
| 0 | 0 | 1 | 0 | 0 | 0 |
| 0 | 1 | 0 | 1 | 0 | 1 |
| 0 | 1 | 1 | 0 | 0 | 1 |
| 1 | 0 | 0 | 1 | 1 | 1 |
| 1 | 0 | 1 | 0 | 0 | 0 |
| 1 | 1 | 0 | 1 | 1 | 1 |
| 1 | 1 | 1 | 0 | 0 | 1 |

 $$F(x,y,z)=x{y}+\overline z$$
 
* Sebagian besar identitas Boolean memiliki bentuk AND (perkallian) serta bentuk OR (jumlah). Kami menyajikan identitas kami menggunakan kedua bentuk tersebut. 

| Identity Name | AND Form | OR Form |
| -------- | -------- | ------- |
| Identity Law | $$1x=x$$ | $$0+x=x$$ |   
| Null Law | $$0x=0$$ | $$1+x=1$$ |
| Idempotent Law | $$xx=x$$ | $$x+x=x$$ |
| Inverse Law | $$x\overline x=0$$ | $$x+\overline x=1$$

* Kelompok kedua

| Identity Law | AND Form | OR Form |
| -------- | -------- | -------- |
| Commutative Law | $$xy = yx$$ | $$x+y=y+x$$|
| Associative Law | $$(xy)z=x(yz)$$ |$$(x+y)+z=x+(y+z)$$|
| Distributive Law | $$x+yz=(x+y)(x+z)$$|$$x(y+z)=xy+xz$$|

* Kelompok ketiga 

| Identity Law | AND Form | OR Form |
| -------- | -------- | -------- |
| Absorption Law DeMorgan's Law | $$x(x+y=x$$ $$\overline(xy)=\overline x+\overline y$$|$$x+xy=x$$ $$\overline(x+y)=\overline x\overline y$$ | 
| Double Complement Law | $$\overline(\overline x)=x$$ |
 
* Terkadang, lebih ekonomis membangun sirkuit dengan menggunakan komplemen fungsi dan mengkomplementasi hasilnya dibandingkan mengimplementasikan fungsi secara langsung. Hukum DeMorgan memudahkan penemuan komplemen dari fungsi Boolean, yang menyatakan: 
$$\overline{(xy)}= \overline{x}+ \overline{y} \quad \text{and} \quad \overline{(x+y)}= \overline{x} \overline{y}$$ 

**Logic Gates**
* Fungsi Boolean diimplementasikan dalam sirkuit komputer digital yang disebut gerbang (gates).  
* Gerbang adalah perangkat elektronik yang menghasilkan hasil berdasarkan dua atau lebih nilai input.  
* Dalam kenyataannya, gerbang terdiri dari satu hingga enam transistor, tetapi desainer digital menganggapnya sebagai satu kesatuan.  
* Sirkuit terintegrasi mengandung kumpulan gerbang yang sesuai untuk tujuan tertentu.
* Memiliki tiga gerbang yaitu, AND, OR, dan NOT.
gerbang AND ->  1 AND 0=0
gerbang OR  -> i OR o=1
* Gerbang yang sangat berguna lainnya adalah gerbang eksklusif OR (XOR).  
* Output dari operasi XOR adalah benar hanya ketika nilai-nilai input berbeda.
gerbang XOR  -> 1 XOR 0=1
gerbang XOR  -> 1 XOR 1=0
* NAND dan NOR dua gerbang yang sangat penting. Simbol dan tabel kebenarannya ditunjukkan di sebelah kanan. 

* NAND dan NOR dikenal dengan gerbang universal  karena mereka murah untuk diproduksi dan setiap fungsi Boolean dapat dibangun menggunakan gerbang ini. NAND atau hanya gerbang NOR . 
X NAND Y

| X | Y | X NAND Y |
|---|---| -------- |
| 0 | 0 | 1        |
| 0 | 1 | 1        |
| 1 | 0 | 1        |
|1  | 1 | 0        | 

X NOR Y

| X | Y | X NOR Y|
|---|---|--------|
| 0 | 0 | 1      |
| 0 | 1 | 0      |
| 1 | 0 | 0      |
| 1 | 1 | 0      |

* Gerbang dapat memiliki beberapa  inputs dan dan lebih dari satu output.
* Output kedua dapat disediakan untuk komplemen dari operasi.

**Komponen Digital**
* Hal utama yang perlu diingat adalah bahwa kombinasi gerbang menerapkan fungsi Boolean.
* Rangkaian di bawah ini mengimplementasikan fungsi Boolean :
$F(X,Y,Z) = X+ \overline{Y}Z$

**Combinational Circuits(Sirkuit Kombinasi)**
* Kami telah merancang rangkaian yang mengimplementasikan fungsi Boolean :
$F(X,Y,Z) = X+ \overline{Y}Z$
* Rangkaian ini merupakan contoh rangkaian logika kombinasional.
* Rangkaian logika kombinasional menghasilkan output tertentu.
* Rangkaian logika kombinasional memberi kita banyak perangkat yang berguna.
* Salah satu yang paling sederhana adalah half adder, yang menemukan jumlah dua bit.
* Kita dapat memperoleh beberapa wawasan tentang konstruksi setengah penjumlah dengan melihat tabel kebenarannya, yaitu:

Inputs  Outputs
| X | Y | Sum | Carry |
|---|---|-----|-------|
| 0 | 0 | 0   | 0     |
| 0 | 1 | 1   | 0     |
| 1 | 0 | 1   | 0     |
| 1 | 1 | 0   | 1     |

* Jumlahnya dapat ditemukan menggunakan operasi XOR dan sisanya menggunakan operasi AND.
 







