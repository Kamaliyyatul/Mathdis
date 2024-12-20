---
title: Deret dan Rekursi

---

# Deretan dan Rekursi

## Deretan
- Deretan adalah suatu urutan atau susunan elemen atau objek yang disusun secara teratur berdasarkan suatu aturan tertentu. Elemen dalam deretan biasanya berupa angka, huruf, simbol, atau objek lainnya, dan urutannya dapat didasarkan pada pola, nilai, atau hubungan tertentu.

- Definisi: Sebuah deretan adalah fungsi dari subset suatu himpunan bilangan bulat (biasanya N atau P) ke sebuah himpunan S.
N = {1, 2, 3, 4, ...}
S misalnya {2, 4, 6, 8, ...}, {1/3, 1/5, 1/7, ...}, dsb
Notasi deretan: $\{a_n\}$
- Deretan umumnya dinyatakan dalam suatu formula, misalnya:
$a_n$ = $2_n$
$a_n$ = $1/_n$
$a_n$ = $7-3_n$

Dalam konteks matematika, deretan sering merujuk pada barisan bilangan, yaitu kumpulan bilangan yang disusun dalam suatu pola tertentu. Misalnya:
1. Deretan bilangan ganjil: 1, 3, 5, 7, ...
2. Deretan bilangan genap: 2, 4, 6, 8, ...
3. Deretan bilangan yang membentuk deret aritmatika: 3, 6, 9, 12, ...
- Contoh - contoh deretan dan formulanya:
- 
### - Deret Aritmatika
Deret dengan pola kenaikan atau penurunan tetap.
Contoh: 2, 5, 8, 11, 14, ...
**Rumus suku ke-n**:
          $U_n = a + (n-1).b$
Di mana:
$a$ : suku pertama
$b$ : beda(selisih antar suku)
$n$ : nomor suku yang dicari

### - Deret Geometri
Deret dengan pola kelipatan tetap.
Contoh: 3, 6, 12, 24, 48, ...
**Rumus suku ke-n**:
        $U_n = a . r^{(n-1)}$
Di mana:
$a$ = suku pertama
$r$ = rasio(perbandingan antar suku)
$n$ = nomor suku yang dicari

### - Deret Bilangan Kuadrat
Deret dengan pola nilai berupa kuadrat bilangan bulat.
Contoh: 1, 4, 9, 16, 25, ...
**Rumus suku ke-n:**
           $U_n = n^{2}$

### - Deret Bilangan Kubik
Deret dengan pola nilai berupa kubik bilangan bulat.
Contoh: 1, 8, 27, 64, 125, ...
**Contoh suku ke-n:**
         $U_n = n^{3}$

### - Deret Fibonacci
Deret dengan pola di mana setiap suku merupakan jumlah dua suku sebelumnya.
Contoh: 0, 1, 1, 2, 3, 5, 8, ...
**Rumus suku ke-n**(rekrusif):
             $F_n = F_n + F_n-_2 . F_0 = 0 . F_1= 1$
             
- String adalah deretan berhingga karakter berbentuk: $a_1 a_2 a_3 a_4 ....a_n$
Panjang string S adalah jumlah karakter di dalam string tersebut
Contoh: *informatika* adalah string dengan panjang 11 karakter 10100101 adalah string biner dengan panjang 8 bit.
- String kosong dilambangkan dengan $\lambda$, panjangnya = 0
### Penjumlahan deretan
jumlah deretan
    $a_m, a_{m+1}, a_{m+2}, \dots, a_n$
adalah
$a_m + a_{m+1} + a_{m+2} + \dots + a_n$
atau dalam notasi sumasi:
$\sum_{k=m}^{n}a_k$

$k$ adalah indeks sumasi,
$m$ adalah batas bawah indeks,
$n$ adalah batas atas indeks

Contoh: Berapa nilai $\sum_{k=1}^{5}k^2$ ?
Jawaban:
  $\sum_{k=1}^{5}k^2$ $= 1^2 + 2^2 + 3^2 + 4^2 + 5^2 = 1 + 9 + 16 + 25 = 55$
  
Contoh2: Sumasi dapat dipecah dengan membagi dua indeksnya, misalnya
$\sum_{k=1}^{100}k^2$ = $\sum_{k=1}^{49}k^2$ + $\sum_{k=50}^{100}k^2$


|      *Sum*        |    *Closed Form*   |
| ----------------- | ------------------ | 
|              $\sum_{k=0}^{n} a^k \quad \quad (r \neq 0)$|    $\frac{ar^{n+1} - a}{r - 1}, \quad r \neq 1$     |
|$\sum_{k=1}^n k$  |$\frac{n(n+1)}{2}$| 
|$\sum_{k=1}^n k^2$|$\frac{n(n+1)(2n+1)}{6}$ |
|$\sum_{k=1}^n k^3$|$\frac{n^2(n+1)^2}{4}$|
|$\sum_{k=0}^\infty x^k, \quad \lvert x \rvert < 1$| $\frac{1}{1-x}$
|$\sum_{k=1}^\infty kx^{k-1}, \quad \lvert x \rvert < 1$|$\frac{1}{(1-x)^2}$|      |

### Sumasi ganda
Di dalam algoritma, kita perlu menghitung berapa kali suatu operasi tertentu dilakukan di dalam sebuah kalang bersarang (nested loop). Penjumlahan semua operasi di dalam kalang bersarang dinyatakan dalam bentuk sumasi ganda.
Contoh: $\sum_{i=1}^{4}$ $\sum_{j=1}^{3}ij$ 
Untuk menghitung sumasi ganda, mula-mula ekspansi sumasi terdalam, lalu dilanjutkan sumasi terluar:
$\sum_{i=1}^{4}$ $\sum_{j=1}^{3}ij$ = $\sum_{i=1}^{4}$ $(i + 2i + 3i)$ = $\sum_{i=1}^{4}$ $6i$ = 6 + 12 + 18 + 24 = 60 

Contoh penggunaan: Berapa kali operasi + dilakukan di dalam algoritma di bawah ini?
      x = 0
      for $j$ = 1 to 10 do
         for $k$ = 1 to $j$ do
             x = x + 2
         end for
        end for
Penyelesaian:
Operasi + terdapat di dalam pernyataan x = x + 2 Operasi ini dilakukan satu kali pada setiap pengulangan.
Jumlah seluruh operasi + adalah:
t = $\sum_{j=1}^{10}$ $\sum_{k=1}^{j}1$
    = $\sum_{j=1}^{10}$ (1 + 1 + ...+ 1 *sebanyak j kali*)
    = $\sum_{j=1}^{10}j$
    = $\frac{10(10+1)}{2}$ = 55
  
## Rekursi
- Sebuah objek dikatakan **rekursif** (*recursive*) jika ia didefinisikan dalam terminologi dirinya sendiri.
- Proses mendifinisikan objek dalam terminologi dirinya sendiri disebut **rekusri** (*recursion*).

### Fungsi Rekursif
Fungsi rekursif didefinisikan oleh dua bagian:
(1). Basis 
- Bagian yang berisi nilai fungsi yang terdefinisikan secara eksplisit.
- Bagian ini juga sekaligus menghentikan rekursif (dan memberikan sebuah nilai yang terdefinisi pada fungsi rekursif).
(2). Rekurens
- Bagian ini mendifinisikan fungsi dalam terminologi dirinya sendiri.
- Berisi kaidah untuk menemukan nilai fungsi pada suatu input dari nilai-nilai lainnya pada input yang lebih kecil.
Contoh: misalkan $f$ didefinisikan secara rekursif yaitu:

$f(n)$ =\begin{cases} 3, & \text{jika } n = 0 \quad basis \\ 2f(n-1) + 4, & \text{jika } n > 0 \quad rekurens\end{cases}

Tentukan nilai f(4)!
Solusi: f(4) = 2f(3) + 4
        =  2(2f(2) + 4) + 4
		=  2(2(2f(1) + 4) + 4) + 4
		=  2(2(2(2f(0) + 4) + 4) + 4) + 4
		=  2(2(2(2 . 3 + 4) + 4) + 4) + 4	
	    =  2(2(2(10) + 4) + 4) + 4
		=  2(2(24) + 4) + 4
		=  2(52) + 4
		= 108	
Adapun cara lain untuk menghitungnya:
f(0) = 3
f(1) = 2f(0) + 4 = 2 . 3 + 4 = 10
f(2) = 2f(1) + 4 = 2 . 10 + 4 = 24
f(3) = 2f(2) + 4 = 2 . 24 + 4 = 52
f(4) = 2f(3) + 4 = 2 . 52 + 4 = 108
Jadi, f(4) = 108.

contoh: Nyatakan n! dalam definisi rekursif
Solusi: 
$n!$ = $1 \times 2 \times 3 \times \dots \times (n-1) \times n =\underbrace{1 \times 2 \times 3 \times \dots \times (n-1)}_{(n-1)!} \times n = (n-1)! \times n$
Misalkan f(n) = n!, maka
$n!$ =\begin{cases} 1  & , n = 0 \quad  \\ n . (n-1)!  &  ,n > 0 \quad \end{cases}

Menghitung 5! secara rekursif adalah:
5! = 5 . 4! = 5 . 4 . 3! = 5 . 4 . 3 . 2!
= 5 . 4 . 3 . 2 . 1! = 5 . 4 . 3 . 2 . 1 . 0! = 5 . 4 . 3 . 2 . 1 . 1 = 120

Algoritma menghitung faktorial:
function *Faktorial* (input $n$ : integer) -> integer
*{menegembalikan nilai n!:
basis : jika n = 0, maka 0! =1
rekurensi : jika n > 0, maka n! = n x (n-1)!}*
DEKLARASI
ALGORITMA:
if n = 0 then
   return 1
else 
   return n * *Faktorial* (n - 1) *{rekurens}*
end

### Struktur Rekursif
Struktur data yang penting dalam komputer adalah pohon biner (*binary tree*)
![Screenshot (68)](https://hackmd.io/_uploads/Sk2laNgXyx.png)

- Simpul (*node*) pada pohon biner mempunyai paling banyak dud buah anak.
- Jumlah anak pada setiap simpul bisa 1, 2, atau 0.
- Simpul yang mempunyai anak disebut simpul cabang (*branch node*) atau simpul dalam (*internal node*).
- Simpul yang tidak mempunyai anak disebut simpul daun (*leave*).
- Pohon biner adalah struktur yang rekursif, sebab setiap simpul mempunyai cabang yang yang juga berupa pohon. Setiap cabang disebut upapohon(*subtree*).
 ![Screenshot (69)](https://hackmd.io/_uploads/ry7DANxQJe.png)

- Oleh karena itu, pohon dapat didefinisikan secara rekursif sebagai berikut:
(a). Basis: kosong adalah pohon biner
(b). Rekurens: jika $T_1$ DAN $T_2$ adalah pohon biner, maka **.** adalah pohon biner.
