---
title: Teorema Bayes

---

# Teorema Bayes
Teorema Bayes merupakan suatu konsep dalam probabilitas yang memperhitungkan bagaimana probabilitas suatu peristiwa dapat dipengaruhi oleh peristiwa lainnya. Teorema Bayes digunakan untuk mengestimasi atau menghitung parameter dalam suatu distribusi probabilitas. Teorema Bayes ini menyatakan bahwa peristiwa di masa depan atau yang belum terjadi dapat diprediksi dengan mempertimbangkan peristiwa sebelumnya yang telah terjadi. Teorema Bayesian merupakan dasar dari ditemukannya Metode Bayesian.

## Contohnya:
Bagaimana kemungkinan/probabilitas usia paruh baya tekanan darah sangat tinggi kemungkinan penyakit Hipertensi (H) atau Tidak (T)


|No|Usia|Tekanan Darah|Penyakit(H/T)
|--|-------|-------- |-----|
|1.| Muda  | Normal | T |
|2.| Muda  | Tinggi | T |
|3.| Paruh baya| Normal | T |
|4.| Paruh baya| Tinggi | H |
|5.| Tua  | Normal | H |
|6.| Tua  | Sangat Tinggi| H |
|7.| Muda | Normal | T |
|8.| Tua  | Tinggi | H |

Dari tabel di atas tentukan:
1. Hitunglah probabilitas Hipertensi terhadap usia paruh baya tekanan darah sangat tinggi
2. Hitunglah probabilitas Tidak Hipertensi terhadap usia paruh baya tekanan darah sangat tinggi

Sehingga menggunakan **Teorema Bayes**:
Teorema Bayes Yaitu hubungan antara prior, likelihood, dan posterior dinyatakan dalam Teorema Bayes. Secara matematis, teorema Bayes dapat ditulis sebagai berikut:

$P( H| X) = \frac{P(X|H) \cdot P(H)}{P(X)}$

- $P(H | X)$ adalah posterior probabilitas dari parameter $H$ setelah melihat data $X$.
- $P(X | H)$ adalah likelihood dari data $X$ dengan parameter $H$.
- $P(H)$ adalah prior probabilitas dari parameter $H$.
* $P(X)$ adalah probabilitas dari data $X$.


- **Prior**
Prior adalah pengetahuan awal tentang parameter yang tidak diketahui dihubungkan dengan informasi yang diperoleh dari pengamatan sebelumnya.

- **Likelihood**
Likelihood adalah distribusi probabilitas dari data yang diberikan parameter. Likelihood memberikan informasi tentang sejauh mana parameter dapat menjelaskan data yang diamati. 

- **Posterior**
Posterior Merupakan distribusi probabilitas yang diperbarui setelah menggabungkan informasi dari prior dan likelihood. Posterior probability menggambarkan keyakinan kita tentang parameter setelah memperhitungkan data yang diamati.

### Jawaban:
1. $P(H | X)$ = $P(X_1| H)$ **.** $P(X_2 | H)$ **.** $P(H)$
= $P(\frac{1}{4})$ **.** $P(\frac{1}{4})$ **.** $P(\frac{4}{8})$
= $0.03125$

2. $P(T | X)$ = $P(X_1| T)$ **.** $P(X_2 | T)$ **.** $P(T)$
= $P(\frac{1}{4})$ **.** $(0)$ **.** $P(\frac{4}{8})$
= $0$