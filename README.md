# TUGAS PRAKTIKUM 8
Buat program sederhana dengan mengaplikasikan penggunaan class. Buatlah
class untuk menampilkan daftar nilai mahasiswa, dengan ketentuan:
• Method tambah() untuk menambah data
• Method tampilkan() untuk menampilkan data
• Method hapus(nama) untuk menghapus data berdasarkan nama
• Method ubah(nama) untuk mengubah data berdasarkan nama

## Step 1 : Deklarasi Class

![foto](Foto/ss1.png)

* class: Membuat sebuah class bernama DaftarNilaiMahasiswa.
* Class ini adalah tempat untuk mendefinisikan atribut (data) dan method (fungsi) yang akan digunakan untuk mengelola daftar nilai mahasiswa.

## Step 2 : Konstruktor (__init__)

![foto](Foto/ss2.png)

* __init__: Fungsi yang dipanggil otomatis saat objek class dibuat.
* self: Mengacu pada instance dari class tersebut.
* self.data_mahasiswa: Atribut berupa list kosong yang akan digunakan untuk menyimpan data mahasiswa dalam bentuk dictionary.

## Step 3  : Method tambah

![foto](Foto/ss3.png)

Fungsi:
Menambahkan data mahasiswa ke dalam atribut self.data_mahasiswa.
### Penjelasan Baris:
1. def tambah(...): Mendefinisikan fungsi tambah dengan parameter:
    * nama: Nama mahasiswa.
    * nim: Nomor Induk Mahasiswa.
    * nilai_uts, nilai_uas, nilai_tugas: Nilai akademik mahasiswa.
2. Membuat dictionary mahasiswa:
rata_rata: Dihitung menggunakan rumus:

![foto](Foto/ss8.png)

## Step 4 : Method tampilkan

![foto](Foto/ss4.png)

Fungsi:
Menampilkan semua data mahasiswa dalam bentuk tabel.
### Penjelasan Baris:
1. Cek data kosong:

![foto](Foto/ss9.png)

* Jika self.data_mahasiswa kosong, tampilkan pesan dan keluar dari fungsi.

2. Header Tabel :

![foto](Foto/ss10.png)

* Mengatur format kolom dengan lebar tertentu menggunakan string formatting.

3. Menampilkan setiap data :

![foto](Foto/ss11.png)

* Menggunakan loop untuk menampilkan setiap data di list self.data_mahasiswa.
* enumerate: Memberikan nomor urut pada setiap data.

## Step 5 : Method hapus

![foto](Foto/ss5.png)

Fungsi:
Menghapus data mahasiswa berdasarkan nama.
### Penjelasan Baris :
1. Loop mencari nama:

![foto](Foto/ss12.png)

* Loop untuk mencari data mahasiswa dengan nama sesuai input.

2. Menghapus data ;

![foto](Foto/ss13.png)

* Jika ditemukan, data dihapus dari list self.data_mahasiswa.

3. Jika tidak ditemukan :

![foto](Foto/ss14.png)

* Menampilkan pesan error jika nama tidak ditemukan.

## Step 6 : Method ubah

![foto](Foto/ss6.png)

Fungsi:
Mengubah data mahasiswa berdasarkan nama.
### Penjelasan Baris :
1. Loop mencari nama

![foto](Foto/ss15.png)

* Loop untuk mencari data mahasiswa dengan nama sesuai input.

2. Mengupdate data :

![foto](Foto/ss16.png)

* Meminta input baru untuk data mahasiswa.
* Mengupdate nilai rata-rata.

3. Jika tidak di temukan :

![foto](Foto/ss17.png)

## Step 7 : Menu Interaktif

![foto](Foto/ss7.png)
Penjelasan:
1. while True: Program berjalan terus sampai pengguna memilih keluar.
2. Menu: Menampilkan pilihan yang bisa dipilih pengguna.
3. Input pengguna:
    * Memilih menu dengan angka.
    * Setiap angka memanggil method yang sesuai:
        1: tambah
        2: tampilkan
        3: hapus
        4: ubah
        5: Keluar program dengan break.

# Hasil Output

## 1. Menambahkan Data Mahasiswa :

### Contoh Input :

![foto](Foto/ss18.png)

### Output :

![foto](Foto/ss19.png)

* Penjelasan:
  Program berhasil menambahkan data mahasiswa "Budi" beserta NIM dan nilai akademiknya ke dalam list self.data_mahasiswa. Selain itu, nilai rata-rata dihitung dan disimpan di dalam data tersebut.

## 2. Menampilkan Daftar Mahasiswa :

### Contoh Input :

![foto](Foto/ss21.png)

### Hasil Output :

![foto](Foto/ss21.png)

* Penjelasan:
Program menampilkan daftar mahasiswa yang sudah dimasukkan ke dalam self.data_mahasiswa.
Tabel berisi:
    * No: Nomor urut.
    * Nama: Nama mahasiswa.
    * NIM: Nomor Induk Mahasiswa.
    * UTS, UAS, Tugas: Nilai yang dimasukkan.
    * Rata-rata: Rata-rata dari nilai UTS, UAS, dan Tugas.



