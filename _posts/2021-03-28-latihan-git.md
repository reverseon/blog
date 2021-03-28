---
layout: post
title:  "Mencoba Git (Untuk Kesekian Kalinya)"
date:   "2021-03-28 21:22:03 +0700"
categories: ranting
---
---
{: data-content=" Introduction "}
Pada kesempatan kali ini, saya ingin menuliskan pengalaman saya (untuk kesekian kalinya) menggunakan git dan mengintegrasikannya dengan platform GitHub. Without further ado, let's delve right into it.

---
{: data-content=" Git and GitHub TL;DR "}
Git     : VCS (Version Control System) untuk memanage dan mentrack perubahan yang dibuat ke source code.

GitHub  : Layanan Hosting berbasis Cloud untuk memanage git repositories. 

---
{: data-content=" Initialization "}
![cmdinit](https://media.discordapp.net/attachments/600014936336367616/825739730418663464/unknown.png)

Kita akan membuat folder dengan nama tugas-prd1 dan melakukan git init didalamnya. Setelah itu, akan terlihat .git folder yang akan menyimpan seluruh informasi yang diperlukan untuk repositori.

---
{: data-content=" Membuat file "}
![cmdinit](https://media.discordapp.net/attachments/600014936336367616/825740265779888148/unknown.png)

File yang akan kita buat kali ini, sesuai instruksi, adalah Latihan-1.txt yang berisi string "Ini adalah latihan mandiri pertama." pada baris pertama. Untuk memasukan string tersebut ke dalam --dan membuat-- file kita akan menggunakan command echo.

Lalu, kita akan mengecek apakah command echo kita sukses dengan command type untuk membaca string yang ada didalam file Latihan-1.txt. Kita juga akan menggunakan command dir/a --for extra sure-- untuk melihat apakah file kita sudah berhasil terbuat atau belum. Saya juga mengecek di git status apakah file tersebut sudah berhasil masuk ke untracked files atau belum.

---
{: data-content=" First Commit "}
![cmdinit](https://media.discordapp.net/attachments/600014936336367616/825745903368929330/unknown.png)

Setelah yakin bahwa tidak ada yang salah dalam tahap pembuatan file, kita akan memasukan file tersebut kedalam commit kita. 

Gunakan command git add untuk memasukan files ke dalam sesi commit ini --saya cek dengan git status juga apakah file berhasil di add-- dan akan menggunakan command git commit -m dengan keterangan commit "Membuat file Latihan-1.txt."

---
{: data-content=" First Change (and second Commit) "}
![cmdinit](https://media.discordapp.net/attachments/600014936336367616/825751783426883625/unknown.png)

Di bagian kali ini, kita akan menambahkan string "Saya sedang coba memahami Git." pada baris kedua file Latihan-1.txt dengan kembali menggunakan command echo.

Setelah standard check menggunakan git status dan type, kita akan menggunakan git add untuk menambahkan file Latihan-1.txt yang sudah diubah ke dalam commit baru. menggunakan git commit -m, kita akan memberi keterangan commit ini "Menambah baris kedua."

Extra last step, kita akan menggunakan git diff untuk mendeteksi apa yang berubah antara id commit satu dengan id commit yang lainnya.

---
{: data-content=" Ngepush ke Repo gan "}

![push](https://media.discordapp.net/attachments/600014936336367616/825760503305469972/unknown.png)

Setelah membuat kedua commit tersebut, kita siap untuk mengepush (apa ya bahasa indonesianya?) commit kita ke repository yang kita inginkan.

Sebelumnya, saya sudah membuat repositori ku1202-percobaan-2[^1] yang saya buat di akun github pribadi saya, namun tidak sempat saya dokumentasikan, jadi kita akan langsung lanjut saja ke step berikutnya.

Kita akan menambahkan repositori tujuan push kita, jangan lupa **git checkout master** juga bila memiliki banyak branch --ini juga saya lupa dokumentasikan hehe-- untuk mengepush commit yang kita add ke master branch menuju repo yang kita inginkan.

Setelah pengecekan terakhir dengan git remote, dir/a, dan git log untuk terakhir kalinya, kita siap push commit dari branch yang kita inginkan ke repositori dengan command git push --tambahkan origin master untuk extra sure bila ingin push master-- dan hasilnya bisa terlihat di tangkapan layar cmd berikut.

![gg](https://media.discordapp.net/attachments/600014936336367616/825760888975654992/unknown.png)

Untuk melihat apakah push kita sukses --selain dari cmd-- kita bisa langsung menuju repositori yang kita tuju di browser kita dan melihat apakah file yang kita commit sudah tampak di repositori tersebut. Dalam hal ini, sudah, yey!

![yey](https://media.discordapp.net/attachments/600014936336367616/825761829753323541/unknown.png)

---
{: data-content=" After Thoughts "}

GitHub menawarkan layanan yang sangat fleksibel dan efisien dalam hal Version Control System. dengan bantuan GitHub (dan git tentunya) kita bisa dengan mudah mentrack apa saja changes yang kita buat ke repositori kita. Ini berguna ketika nanti terjadi error, kita bisa tahu versi mana yang works sebelum error itu muncul dan akan mudah diidentifikasi bagian mana yang menyebabkan error pada program kita

Additionally, para program open source juga bisa memanfaatkan GitHub sebagai platform yang bisa mengakomodir pengguna dari sebuah program tersebut untuk berkontribusi terhadap pengembangan program tersebut secara fleksibel dan seamless.

Mungkin hanya sekian yang bisa saya ceritakan mengenai pengalamn saya dalam mencoba git (dan github). Terima kasih telah membaca dan Have a Good Day!

---
{: data-content=" Helpful Links "}
[^1]: Repo: [https://github.com/reverseon/ku1202-percobaaan-2](https://github.com/reverseon/ku1202-percobaaan-2)