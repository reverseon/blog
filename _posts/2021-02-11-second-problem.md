---
layout: post
title:  "Need, Know, How, Solve, and Check! Problem 2"
date:   "2021-02-11 08:27:31 +0700"
categories: analysis
---
---
{: data-content="Introduction"}

Artikel ini adalah artikel lanjutan dari artikel problem 1 sebelumnya, untuk membaca problem 1 silahkan klik link di bawah ini. 

- [Need, Know, How, Solve, and Check! Problem 1](https://reverseon.github.io/blog/analysis/2021/02/11/first-problem.html)

With that said, mari kita lanjutkan ke problem kedua.

---
{: data-content="Table of Contents"}
- [Second Problem](#second-problem)
    * [2.0 Overview](#20-overview)
    * [2.1 Need](#21-need)
    * [2.2 Know](#22-know)
    * [2.3 How](#23-how)
    * [2.4 Solve](#24-solve)
        + [2.4.1 Assumptions](#241-assumptions)
        + [2.4.2 Calculations](#242-calculations)
        + [2.4.3 Conclusions](#243-conclusions)

---
{: data-content="Contents"}
## Second Problem

### 2.0 Overview

Berapa jumlah kios cukur rambut pria (barbershop) di kota Bandung (jumlah penduduk sekitar 2.5 juta jiwa)?

### 2.1 Need

Dari deskripsi problem di bagian overview, kita perlu menjawab pertanyaan

- Berapa jumlah barbershop di kota Bandung?

### 2.2 Know

Dari deskripsi problem di bagian overview, kita mengetahui bahwa kota Bandung memiliki penduduk sekitar 2.5 juta jiwa

### 2.3 How

Simpel saja, dengan memanfaatkan teknologi, saya akan melakukan riset seberapa banyak queries "Barbershop di Kota Bandung" yang muncul di Google Maps.

### 2.4 Solve

Mudah saja, pergi ke Google Maps, masukan query "Barbershop di Kota Bandung," Google akan menampilkan list Barbershop yang sesuai.

![gmaphome](/blog/assets/img/bkb.jpg)

[See Source][^1]

Tentu saja, dengan metode riset senaif ini, akan banyak asumsi dan kompromi yang harus digunakan untuk menjustify riset abal-abal ini.

#### 2.4.1 Assumptions

<ol type="a">
<li>Seluruh Barbershop di kota Bandung <b>MEMILIKI</b> address di Google Maps dan <b>TERINDEKS</b> query Google Maps</li>
<li>Query Google Maps memberikan hasil list yang akurat</li>
</ol>

#### 2.4.2 Calculations

Oke, sederhana saja, kita tinggal manual swipe hingga mentok tidak ada queries lagi yang ditampilkan. Ini akan memberikan estimasi figur yang cukup baik untuk Barbershop yang ada di Kota Bandung.

![gmapfull](/blog/assets/img/bkbfull.jpg)

Terlihat ada 246 Barbershop yang terindeks oleh Google Maps dengan query "Barbershop di Kota Bandung." Namun, tidak semuanya adalah barbershop **di Kota Bandung**, bahkan ada yang bukan Barbershop sama sekali, Trans Studio Mall, misalnya. Maka dari itu, figur 246 akan kita kurangi 15% untuk mengkompensasi ketidakakuratan tersebut. Berarti

$$246 \cdot (1 - \frac{15}{100}) \approx 209$$

Kita berakhir dengan figur 209 Barbershop di Kota Bandung

#### 2.4.3 Conclusions

Berdasarkan riset dan kalkulasi singkat diatas, estimasi jumlah kios cukur rambut pria (barbershop) di kota Bandung adalah `209 outlet`.

---
{: data-content="Citations"}
[^1]: Barbershop di kota bandung - google maps. (n.d.). Google Maps. Retrieved February 11, 2021, from https://www.google.com/maps/  search/barbershop+di +Kota+Bandung/
