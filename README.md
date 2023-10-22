# Lab2Web
# CSS Dasar
## Profil
| Variable | Isi |
| -------- | --- |
| **Nama** | Ricky alfian saputra |
| **NIM** | 312210279 |
| **Kelas** | TI.22.A4 |
| **Mata Kuliah** | Pemrograman WEB |

### Tugas
1. Buatlah repository baru dengan nama Lab2Web.
2. Kerjakan semua latihan yang diberikan sesuai urutannya.
3. Screenshot setiap perubahannya.
4. Buatlah file README.md dan tuliskan penjelasan dari setiap langkah praktikum beserta
screenshotnya.
5. Commit hasilnya pada repository masing-masing.
6. Kirim URL repository pada e-learning ecampus

## 1. Membuat dokumen HTML


**Hasil :**

![0.1](Gambar/1.png)

## 2. Mendeklarasikan CSS internal

**Hasil :**
![0.1](Gambar/3.png)

## 4. Membuat CSS External

**Hasil :**

![0.1](Gambar/4.png)

## 5. Menambahkan CSS selector

**Hasil :**

![0.1](Gambar/5.png)

### Ini adalah sourcecode akhir pada tugas kali ini.

![]()

## Pertanyaan dan Tugas Pada P2
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.

2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!

3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!

4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! `<p id="paragraf-1" class="text-paragraf">`

## Jawaban
1.

2. `h1 {...}:`
    Ini adalah sebuah selektor CSS umum yang akan mempengaruhi semua elemen `<h1>` di halaman HTML.
    Dalam hal ini, gaya yang didefinisikan akan berlaku untuk setiap elemen `<h1>` di seluruh halaman.

   `#intro h1 {...}:`
    Ini adalah selektor CSS yang lebih spesifik dan berlaku hanya untuk elemen `<h1>` yang berada di dalam elemen dengan ID intro.
    Dalam hal ini, gaya yang didefinisikan hanya akan mempengaruhi elemen `<h1>` yang merupakan turunan dari elemen dengan ID intro.
   
    Dalam kedua kasus di atas, h1 dan `#intro h1` adalah selektor CSS yang mengacu pada elemen `<h1>`. 
    Namun, perbedaannya terletak pada ruang lingkup elemen yang dipengaruhi oleh gaya yang didefinisikan. 
    `h1 {...}` akan mempengaruhi semua elemen `<h1>` di halaman, sedangkan `#intro h1 {...}` akan mempengaruhi hanya elemen `<h1>` yang berada di dalam elemen dengan ID intro.

3. Urutan penulisan berperan ketika spesifisitasnya sama. Spesifisitas diukur berdasarkan kombinasi dari selektor CSS yang digunakan. Semakin spesifik selektor, semakin tinggi              spesifisitasnya.
   Umumnya, urutan prioritas adalah sebagai berikut (dari yang paling rendah ke yang paling tinggi):

    - 1). Deklarasi CSS dari file eksternal.
    - 2). Deklarasi CSS yang ada secara internal.
    - 3). Deklarasi inline CSS.

4. - Deklarasi CSS menggunakan ID memiliki keutamaan lebih tinggi daripada deklarasi CSS menggunakan class.
   - Ketika ada konflik, deklarasi CSS dengan ID akan menggantikan deklarasi CSS dengan class.
  
   CONTOH :

   Misalkan ada dekralasi CSS sebagai berikut.
     ```CSS
     #paragraf-1 {
     color: red;
     font-weight: bold;
     }

     .text-paragraf {
     color: blue;
     }
     ```

   Dan element HTML seperti ini.
     ```HTML
     <p id="paragraf-1" class="text-paragraf">Contoh paragraf</p>
     ```
     
   Dalam contoh di atas, meskipun elemen `<p>` memiliki class `"text-paragraf"`, deklarasi CSS dengan ID `#paragraf-1` akan mendominasi dan mengaturnya menjadi teks berwarna merah dan      tebal (sesuai dengan deklarasi di atas). Deklarasi `color: blue;` dari class akan diabaikan dalam hal ini.
   Jadi, deklarasi dengan ID memiliki prioritas lebih tinggi daripada deklarasi dengan class dalam menentukan gaya elemen.
 