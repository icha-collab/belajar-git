# 1. Instalasi git bash 

 1. Download git pada browser dan ketik 'git-scm'
![[belajar_git/asset/kedua.png|590]]

2. Setelah itu kita klik yang bagian atas GIT dan kita download githubnya seperti gambar dibawah ini, lalu kalau sudah terdownload githubnya nanti ada tahap-tahap menginstalannya dan klik sja NEXT terus sampai selesai.
![[pertama.png|590]]

# 2. Login akun github 

1. Buka browser dan ketik github dan klik paling atas yaitu github.com

![[belajar_git/asset/1.png]]

2. Jika sudah memiliki akun github silahkan dimasukkan username dan password yang telah dibuat sebelumnya dan jika belum mempunyai akun github silahkan klik create an account

![[belajar_git/asset/Picture.png]]

3.  Jika sudah memasukkan username dan password maka akan tampil gambar seperti ini
![[35 (2).png]]
![[2]]

# 3. Buat repository

1. Jika sudah berhasil masuk di akun anda kita kilk logo disamping kanan ini dan akan muncul beberapa opsi

![[2.png]]

Dan kita pilih New repository

![[30 (1).png]]

2. Setelah mengklik "New repository" akan tampil gambar seperti dibawah ini

![[3.png]]

3. Jika sudah mengklik new repository kita bisa menambahkan nama repository sesuai keinginan kita,  seperti gambar di bawah ini

![[30 (2).png]]

4. lalu klik Create repository dan repository akan dibuat secara otomatis oleh github 

![[Picture.png]]

5. Dan setelah membuat repository maka akan tampil gambar seperti dibawah ini

![[5.png]]

# 4. Buat file lokal (VS CODE)

1. Silahkan membuat folder didalam obsidian kalian 

![[obsidian.png]]

2. Setelah membuat folder baru, buatlah file baru (belajar_git) di dalam folder yang sudah dibuat sebelumnya

![[beljr.png]]

# 5. Konfigurasi awal di git bash

1. Buka aplikasi gitbashnya 

![[0.png]]

2. Setelah itu  kita mengetikkan  git verson 

Yang dimana kita mengetikkan ''git --version"  adalah sebuah perintah yang digunakan untuk menampilkan versi Git yang saat ini terpasang di sistem. Saat Anda menjalankan perintah ini di terminal atau command prompt, Git akan mengembalikan nomor versi, Seperti gambar dibawah ini :

![[6.png]]
  Dan outputnya itu "git version 2.45.2.windows.1" Ini berarti Anda menggunakan "Git versi 2.45.2."


3.   Dan mengetik perintah  `git config --list` untuk menampilkan semua konfigurasi Git yang sedang aktif, termasuk pengaturan nama pengguna, email, editor teks, dan lainnya. Jika belum ada user.name dan user.email silahkan masukkan terlebih dahulu. 

```cs
 $ git confiq --list
```

![[8.png]]

4.  Jika belum ada user.name dan user.email silahkan masukkan terlebih dahulu. Dan mengetikkan kode perintah seperti dibawah ini

```cs
 $ git confiq --global user.name "nama akun github"
  $ git confiq --global user.email "nama email kalian"
 
```

![[9.png]]\

5. kita mengecek kembali konfigurasinya seperti gambar bawah ini, dan jika user.name dan user.email kalian sudah seperti gambar dibawah ini berarti kalian sudah berhasil memasukkan user.name dan user.email kalian!!! 

![[7.png]]

# 6. Akses folder proyek di git bash

1. Sesudah kita mamasukkan user.name dan user.email, Kita mengetikkan kode `$ cd d:` untuk Perintah `$ cd d` digunakan untuk berpindah ke direktori bernama "d" dalam direktori saat ini yg kita gunakan. Dan Perintah `$ ls` digunakan untuk menampilkan daftar file dan direktori yang ada dalam direktori saat ini. 

![[11.png]]

2. setelah itu kita ketikkan lagi `cd OBSIDIAN` ini adalah sebuah perintah digunakan untuk masuk ke direktori "OBSIDIAN" dari lokasi saat ini.

![[10 (2).png]]

3. Dan disini kita sudah masuk di folder "OBSIDIAN" yang sudah dibuat tadi, Kita ketikkan lagi perintah `ls` lalu enter, ketikkan lagi perintah `cd belajar_git` lalu enter, dan disini kita sudah masuk di dalam folder file"OBSIDIAN" yaitu file "belajar_git"
![[12.png]]

# 7. Hubungkan folder proyek lokal ke github

## 1. INISIALISASI REPOSITORY

 ketikkan lagi perintah ` git init ` untuk menginisialisasi sebuah repositori Git baru di direktori saat ini. Ini membuat direktori git yang akan melacak semua perubahan, Dan ketikkan lagi 
 `git remote add origin  https://github.com/username/nama-repository.git` untuk menjalankan perintah dan untuk menghubungkan repositori lokal Anda ke repositori
GitHub yang telah Anda buat sebelumnya seperti gambar dibawah ini . Dan jika sudah ada terdapat tulisan seperti gambar dibawah ini yaitu (master) berarti sudah terhubung ke repositori Githubnya 


![[15 (2).png]]

## 2. HUBUNGKAN KE REPOSITORY GITHUB
 Dan ketikkan lagi  `git remote add origin` ` https://github.com/username/nama repository.git` untuk menjalankan perintah dan untuk menghubungkan repositori lokal Anda ke repositori GitHub yang telah Anda buat sebelumnya seperti gambar dibawah ini . Dan jika sudah ada terdapat tulisan seperti gambar dibawah ini yaitu (master) berarti sudah terhubung ke repositori Githubnya.
 
![[15 (1).png]]

## 3. TAMPILKAN SEMUA FILE-FILE BARU ATAU PERUBAHAN MENGGUNAKAN

`git status` untuk perintah Git yang digunakan untuk melihat status terkini repositori, termasuk perubahan yang belum di-_commit_, file baru yang belum dilacak, dan informasi tentang cabang yang sedang aktif.

![[16.png]]

## 4. TAMPILKAN SEMUA FILE-FILE BARU ATAU PERUBAHAN MENGGUNAKAN

`$ git add.` perintah ini digunakan untuk menyiapkan file yang telah diubah agar bisa di-commit ke repositori.

![[20.png]]

## 5. TAMPILKAN STATUS COMMIT / KONEKSI FILE KE GITHUB

`git status` untuk perintah Git yang digunakan untuk melihat status terkini repositori, termasuk perubahan yang belum di-_commit_, file baru yang belum dilacak, dan informasi tentang cabang yang sedang aktif.

![[tera.png|390]]

## 6. TAMBAHKAN PESAN COMMIT MENGGUNAKAN 

  perintah `$ git commit -m "pesan commit` atau `awal belajar` digunakan untuk menyimpan perubahan yang telah disiapkan dengan pesan deskriptif. Pesan commit menjelaskan apa yang telah diubah atau ditambahkan.
![[20 (2).png]] 

## 7. UNGGAH SELURUH PERUBAHAN MENGGUNAKAN

Dan dijalankan perintah berikut untuk mengunggah kode Anda ke GitHub dan
ketikkan perintah `git push -u origin master` seperti gambar dibawah ini 

![[20 (3).png]]

## 8.  LOGIN KE AKUN GITHUB ATAU GUNAKAN TOKEN

Disini anda disuruh untuk  login akun github yang sudah dibuat dan Perintah ini akan mengunggah kode Anda ke repositori GitHub

 ![[35 (6).png]]
 
# Navigasi Dasar Git dengan cd, ls, dan pwd

Dalam menggunakan Git, ada beberapa perintah dasar yang sering digunakan untuk navigasi
di dalam sistem file. Tiga perintah tersebut adalah `cd , ls ,` dan `pwd `.
## cd

- Fungsi: Digunakan untuk berpindah ke direktori (folder) lain dalam sistem file.
- Contoh penggunaan:
`cd nama document`
- `cd Documents` - Berpindah ke direktori "Documents".
- `cd` .. - Berpindah ke direktori induk (satu level di atas).
## ls

- Fungsi: Digunakan untuk melihat daftar file dan direktori yang ada di dalam direktori saat ini.
- Contoh penggunaan:
`ls`
- `ls` - Menampilkan daftar fle di dalam direktori saat ini
## pwd (Print Working Directory)

- Fungsi: Digunakan untuk melihat path (jalur) direktori kerja saat ini.
- Contoh penggunaan:
- `pwd` - Menampilkan path direktori kerja saat ini.Kegunaan dalam Konteks Git
## Kegunaan dalam Konteks Git

- `cd` : Memungkinkan Anda berpindah ke direktori repositori Git yang Anda inginkan untuk bekerja.
- `ls` : Memungkinkan Anda melihat file dan direktori yang ada di dalam repositori Git.
- `pwd` : Memungkinkan Anda melihat lokasi direktori kerja saat ini, yang berguna saat Anda bekerja dengan beberapa repositori Git.

Penggunaan perintah-perintah ini secara efektif dapat membantu Anda menavigasi dan
berinteraksi dengan repositori Git Anda dengan lebih mudah.
 
