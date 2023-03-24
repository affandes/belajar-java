# Mengenal Tipe Data Floating Point, Real, Double pada Java

Istilah *Floating Point*, *Float*, *Real*, *Double* mengacu kepada maksud yang sama, yaitu bilangan berkoma. Di dalam pemrograman, penting bagi kita mengetahui tentang tipe data ini, karena tipe data ini dapat menyimpan angka berkoma.

Angka berkoma pada dasarnya adalah bilangan pecahan. Misalnya pecahan ½ sebenarnya adalah angka 0,5 (dibaca: nol koma lima). Berikut kode program untuk menampilkan angka berkoma:

![Kode program untuk menampilkan bilangan berkoma](aset\carbon--21-.png)

Variabel **nilai** berupa tipe data *double*. Dengan demikian variabel tersebut dapat menyimpan angka 87,9 (dibaca: delapan puluh tujuh koma sembilan).

> TIPS: Tanda koma pada Java menggunakan simbol titik "." sedangkan tanda pemisah ribuan menggunakan simbol garis-bawah "_". 

Berikut contoh-contoh kode program untuk menyimpan angka berkoma:

![Contoh kode program untuk membuat dan menyimpan angka berkoma](aset\carbon--24-.png)

Pada kode program di atas, variabel **nilaiD** dapat menyimpan angka berkoma walaupun ditulis tanpa tanda koma.

## Float dan Double

Tipe data *Floating Point* ada dua jenis yaitu *Float* dan *Double*. Tentunya masing-masing memiliki range data tersendiri. Berikut spesifikasi masing-masing tipe data floating point pada Java.

| Tipe Data | Ukuran | Range                   |
| --------- | ------ | ----------------------- |
| float     | 4 byte | Hingga 7 angka desimal  |
| double    | 8 byte | Hingga 15 angka desimal |

> TIPS: Hampir sebagian besar kasus kita cukup menggunakan *double* untuk berbagai macam kalkulasi dan kode program. Sehingga penggunaan *float* hampir tidak pernah atau jarang sekali digunakan karena tingkat presisinya 7 angka di belakang koma.

## Beda Literal/Data Float dengan Double

Karena perbedaan antara kedua tipe data ini hanya tingkat presisinya, sehingga angka 2,5 dengan angka 2,50000 memiliki nilai yang sama walaupun jumlah angka di belakang koma tidak sama. Dengan demikian, harus ada cara untuk membedakan literasi/data 2,5 versi *float* dengan literasi/data 2,5 versi *double*.

Perhatikan kode program berikut ini:

![Kode program untuk membuat variabel dengan tipe data float](aset\carbon--25-.png)

Kita harus menambahkan huruf **F** atau **f** setelah angka supaya angka tersebut dianggap sebagai tipe data *float*. Jika kita tidak menambahkan huruf **F** atau **f** maka Java akan menganggap angka tersebut sebagai *double*. Untuk membuktikannya kita perhatikan kode program berikut:

![Tanpa huruf F diakhir angka, maka tidak bisa disimpan ke variabel float](aset\carbon--26-.png)

Jika kode program tersebut dijalankan akan menghasilkan *error* seperti berikut:

![Pesan error dari kode program sebelumnya](aset\carbon--28-.png)

Pesan *error* tersebut menjelaskan adanya tipe data yang tidak kompatibel. Variabel *float* tidak dapat digunakan untuk menyimpan data *double*. Data *double* yang dimaksud adalah angka 2.5 tanpa disertai dengan huruf **F** atau **f**.

## Kesimpulan

Kita sudah mengenal tipe data Floating Point yang terdiri dari tipe data float dan double. Tipe data ini digunakan untuk menyimpan data angka berkoma atau angka desimal. Sedangkan jika kita ingin menyimpan data bilangan bulat, kita dapat menggunakan tipe data Integer.