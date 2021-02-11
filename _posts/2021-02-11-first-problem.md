---
layout: post
title:  "Need, Know, How, Solve, and Check! Problem 1"
date:   "2021-02-11 08:21:31 +0700"
categories: analysis
---
---
{: data-content="ATTENTION"}

`Gunakan Tablet/PC untuk pengalaman membaca yang optimal karena artikel ini mengandung banyak persamaan Matematis yang mungkin tidak terlalu nyaman dilihat di mobile device`

---
{: data-content="Introduction"}

Need, Know, How, Solve and Check adalah sebuah penstrukturan terhadap suatu masalah agar kita bisa melihat dengan lebih jelas masalah tersebut dan potensi penyelesaiannya.

Dengan membagi-bagi masalah menjadi 3 aspek, yaitu What we need?, What we know? and How do we solve it? akan membuat masalah menjadi lebih terstruktur dan menghilangkan detail detail yang kurang relevan.

Saya diberikan dua problem sebagai tugas yang bertujuan untuk melatih mahasiswa menerapkan metode Need Know How Solve, and probably check. Berikut adalah penjabaran dari problem pertama, problem kedua akan ada di post berikutnya di link ini.

- [Need, Know, How, Solve, and Check! Problem 2](https://reverseon.github.io/blog/analysis/2021/02/11/second-problem.html)

---
{: data-content="Table of Contents"}
- [First Problem](#first-problem)
    * [1.0 Overview](#10-overview)
    * [1.1 Need](#11-need)
    * [1.2 Know](#12-know)
    * [1.3 How](#13-how)
    * [1.4 Solve](#14-solve)
        + [1.4.1 Assumptions](#141-assumptions)
        + [1.4.2 Calculations](#142-calculations)
        + [1.4.3 Conclusions](#143-conclusions)

---
{: data-content="Contents"}

## First Problem

### 1.0 Overview

Kabel baja vertikal digunakan untuk menyangga bagian jalan dalam sebuah konstruksi jembatan gantung. Salah satu kabel vertikal yang panjangnya 4.00 m digunakan untuk menyangga beban 20.0 ton. Akibat beban tersebut, kabel baja bertambah panjang 20.0 cm. Jika beban yang sama disangga oleh kabel baja jenis yang sama dengan panjang 8.00 m. berapa besar pertambahan panjangnya?

### 1.1 Need

Oke, setelah melihat deskripsi problem di bagian overview, sudah jelas hal yang harus dijawab dari permasalahan tersebut adalah

- Berapa besar pertambahan panjang kabel baja dengan panjang 8.00 m saat diberikan beban sebesar 20.0 ton?

### 1.2 Know

Dari deskripsi problem, kita mengetahui bahwa 

- kabel baja yang sama, dengan panjang berbeda yaitu 4.00 m, diberikan beban yang sama, akan bertambah panjang sepanjang 20.0 cm.

### 1.3 How

Dengan informasi dan objektif yang sudah tersedia, sepertinya konsep Stress and Strain dari realm of physics bisa diterapkan untuk menyelesaikan masalah ini.

### 1.4 Solve

Pertama, persamaan utama yang akan kita gunakan adalah definisi Modulus Young yang dinyatakan sebagai

$$E=\frac{\frac{F}{A}}{\frac{\Delta L}{L_0}}=\frac{F \cdot L_0}{A \cdot \Delta L}$$

dengan $$E$$ adalah Modulus Young, $$F$$ adalah gaya stress, $$A$$ adalah permukaan yang terefek gaya, $$\Delta L$$ adalah perubahan kabel akibat gaya, dan $$L_0$$ adalah panjang awal kabel.

#### 1.4.1 Assumptions

Berdasarkan persamaan dasar, ada beberapa asumsi yang harus kita gunakan, yaitu


<ol type="a">
<li>Karena tidak disebutkan, dan melihat bahwa kabel ini digunakan untuk menyangga jembatan yang cukup besar, saya mengasumsikan bahwa kabel baja yang digunakan adalah <b>ASTM-A36</b> Steel bertipe High-tensile Strength Steel</li>

<li>Peristiwa ini terjadi dalam kondisi ideal (tidak ada air resistance and such) </li>

<li>Peristiwa ini terjadi di bumi</li>

<li>Peristiwa ini terjadi di suhu ruangan (20 hingga 27 derajat celsius)</li>

<li>Kabel berbentuk silinder sempurna</li>

<li>Ton yang dimaksud pada soal adalah Metric Ton</li>

<li>Diagram benda bebasnya terlihat seperti ini</li>
</ol>

![Free Body](/blog/assets/img/freebody.jpg)

#### 1.4.2 Calculations

Berdasarkan deskripsi problem dan asumsi yang ditambahkan, kita sejauh ini sudah mengetahui:

$$E = 200 \:  GPa = 2 \cdot 10^5 \: Pa$$ 

[See Source][^1]

$$M_{beban} = 20 \: metric \: Ton = 2 \cdot 10^4 \: kg$$

$$g = 9.8 \: m/s^2$$

$$L_{0_{kabel1}} = 4.0 \: m$$

$$\Delta L_{kabel1} = 20 \: cm = 2 \cdot 10^{-2} \: m$$

$$L_{0_{kabel2}} = 8.0 \: m$$

Lalu, karena gaya yang bekerja pada kabel hanya disebabkan oleh gaya berat benda, maka

$$F=m_{beban} \cdot g = 2 \cdot 10^4 \cdot 9.8 = 1.96 \cdot 10^5 \: N$$

Dengan meninjau kabel 1, kita bisa menemukan luas permukaan yang terefek gaya pada kabel 1 dengan persamaan

$$E=\frac{F \cdot L_{0_{kabel1}}}{A \cdot \Delta L_{kabel1}} \implies A=\frac{F \cdot L_{0_{kabel1}}}{E \cdot \Delta L_{kabel1}}$$

Dengan persamaan tersebut, didapatkan

$$A=\frac{1.96 \cdot 10^5 \cdot 4}{2 \cdot 10^5 \cdot 2 \cdot 10^{-2}} = 196 \: m^2$$

Lalu, dengan informasi tersebut, kita bisa melanjutkan untuk menghitung pertambahan panjang kabel 2 dengan persamaan

$$E=\frac{F \cdot L_{0_{kabel2}}}{A \cdot \Delta L_{kabel2}} \implies \Delta L_{kabel2}=\frac{F \cdot L_{0_{kabel2}}}{A \cdot E}$$

Maka

$$\Delta L_{kabel2}=\frac{1.96 \cdot 10^5 \cdot 8}{196 \cdot 2 \cdot 10^5} = 0.04 \: m  = 40 mm$$


#### 1.4.3 Conclusions

Berdasarkan perhitungan di atas, besar pertambahan panjang kabel baja dengan panjang 8.00 m saat diberikan beban sebesar 20.0 ton adalah `40 milimeter`.

---
{: data-content="Citations"}
[^1]: Young’s Modulus - Tensile and Yield Strength for common Materials. (n.d.). Engineering Toolbox. Retrieved February 11, 2021, from https://www.engineeringtoolbox.com/young-modulus-d_417.html
