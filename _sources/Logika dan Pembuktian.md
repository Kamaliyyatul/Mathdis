---
title: Logika dan Pembuktian

---

# Logika Matematika

## Negasi
Negasi adalah operasi yang menghasilkan kebalikan dari nilai kebenaran suatu pernyataan.
Berikut adalah tabel kebenaran:


| Pernyataan (p )|Negasi($\neg p$)| 
| -------- | -------- | 
| True     | Fals     |   
| Fals     | True     |

## Konjungsi
Konjungsi dalam logika adalah operasi yang menghubungkan dua pernyataan dengan kata "dan" sehingga hasilnya benar jika kedua pernyataan tersebut benar.
Berikut adalah tabel kebenaran:


| Pernyataan ( p) |Pernyataan (q) |Konjungsi (p^q)|
| -------- | -------- | -------- |
| True | True|  True  |         
| True | Fals|  Fals  |  
| Fals | True|  Fals  |
| Fals | Fals|  Fals  |


## Disjungsi
Disjungsi adalah logika matematika yang membandingkan dua obyek.
Berikut adalah tabel kebenaran:


| Pernyataan (p ) | Pernyataan (q) |Disjungsi (p $\lor$ q)|
| -------- | -------- | -------- |
| True     | True     | True     |  
| True     | Fals     | True     |
| Fals     | True     | True     |
| Fals     | Fals     | Fals     |

## Implikasi 
Implikasi adalah kalimat majemuk yang menggunakan kata hubung "JIKA" p "MAKA" q.
Berikut adalah tabel kebenaran:


| Pernyataan (p ) | Pernyataan (q)| Konjungsi $P\implies Q$ 
| -------- | -------- | -------- |
| True     | True    | True    |  
| True     | Fals    | Fals    |
| Fals     | True    | True    |
| Fals     | Fals    | True    |



## Bimplikasi
Bimplikasi adalah pernyataan majemuk dengan kata hubung "...jika dan hanya jika".

Buatlah tabel kebenaran untuk~pernyataan berikut $$P\lor(R\to\ Q)$$

$$\begin{array}{c|c|c|c|cc}P&Q&R&\ Q&R\to\ Q&P\lor(R\to\ Q)\\\hline\text{Т}&\text{Т}&\text{T}&\text{T}&\text{T}&\text{T}\\\text{Т}&\text{Т}&\text{F}&\text{F}&\text{T}&\text{T}\\\text{T}&\text{F}&\text{T}&\text{T}&\text{F}&\text{T}\\\text{T}&\text{F}&\text{F}&\text{T}&\text{T}&\text{T}\\\text{F}&\text{T}&\text{T}&\text{F}&\text{T}&\text{T}\\\text{F}&\text{T}&\text{F}&\text{F}&\text{T}&\text{T}\\\text{F}&\text{F}&\text{T}&\text{T}&\text{F}&\text{F}\\\text{F}&\text{F}&\text{F}&\text{T}&\text{T}&\text{T}&\text{}\end{array}$$
