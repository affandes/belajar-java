---
tags: java/fundamental, operator-expression-statement-block-pada-java
keywords: operator, operand, expression
video: 0
published: false
---
# Kenalan Dengan Operator, Operand dan Expression Pada Java

Data dan variabel tidak akan berguna jika tidak dioperasikan. Operasi data dan variabel sangat banyak sekali. Misalkan menambahkan antara variabel pertama dan variabel kedua, dan sebagainya.

Itulah mengapa kita perlu memahami tentang fundamental dari _Operator_ pada Pemrograman Java. Materi kali ini bakal kita bahas tuntas tentang berbagai jenis operator pada Java.

## Operator dan Operand

Ada 2 (dua) istilah yang harus kita pahami pada awal pembahasan ini, yaitu **Operator** dan **Operand**. *Operator* adalah simbol yang berfungsi untuk menjalankan operasi. Sedangkan *operand* adalah literal, data atau variabel yang dioperasikan.

Supaya kita lebih mudah mengenali *operator* dan *operand* yang ada di dalam kode program, perhatikan ilustrasi berikut ini!

![Operator dan operand](image-5.png)
Tanda ➕ pada ilustrasi di atas adalah sebuah _operator_. Sedangkan angka 10 dan angka 25 adalah _operand_. Ketika operator dijalankan terhadap _operand_, maka _operator_ tersebut akan menghasilkan sebuah data baru. Pada contoh di atas, angka `10` ditambahkan dengan angka `25` akan menghasilkan angka baru, yaitu angka `35` dengan tipe data `int`.

Selain tanda ➕ juga terdapat banyak simbol lainnya yang berfungsi sebagai _operator_. Mengetahui berbagai macam _operator_ akan memudahkan kita untuk membuat sebuah instruksi pada pemrograman Java. Perhatikan kode program berikut ini!

```java
public class Main {
  public static void main(String[] args) {
    int nilai = 10;
    int hasil = nilai + 20;
  }
}
```

Pada kode `int nilai = 10;` di atas, simbol `=` (baca: sama dengan) adalah juga _operator_. Simbol tersebut berfungsi untuk menyimpan data yang ada pada _operand_ sebelah kanan, disimpan ke _operand_ sebelah kiri.

Pada kode `int hasil = nilai + 20;` di atas terdapat 2 (dua) _operator_ yang berbeda, yaitu _operator_ `=` (baca: sama dengan) dan *operator* `+` (baca: plus). Kedua _operator_ ini akan dioperasikan berurutan sesuai dengan ketentuan tertentu. Perhatikan ilustrasi berikut!
![Urutan operasi operator](image-6.png)
Berikut tahapan untuk memproses *operator* di atas:
1. Proses bagian kanan terlebih dahulu, yaitu kode `nilai + 20`. Variabel `nilai` dan literal `20` adalah *operand*. Sedangkan tanda `+` adalah *operator* penjumlahan. 
2. Variabel `nilai` digantikan ke literalnya yaitu `10` (perhatikan kode program sebelumnya). Berikutnya dilakukan penjumlahan antara literal `10` dan literal `20`.
3. Hasil perhitungan sebelumnya menghasilkan literal `30`. Literal `30` ini sebagai *operand*. Begitu juga variabel `hasil` adalah *operand*. *Operator*-nya adalah simbol `=` (baca: sama dengan). Proses ini memindahkan literal `30` ke dalam variabel `hasil`, sehingga ketika proses ini selesai, data di dalam variabel `hasil` adalah `30`.

Apabila terdapat beberapa _operator_ dalam satu instruksi, maka setiap _operator_ akan diproses sesuai dengan ketentuan dan tingkat prioritas dari masing-masing _operator_. Ketentuan ini disebut dengan _precedence_.

Pada contoh ilustrasi di atas, _operator_ yang dijalankan terlebih dahulu adalah _operator_ `+` yaitu menambahkan data pada variabel `nilai` ditambahkan dengan angka `20` sehingga menjadi angka `30`. Selanjutnya baru dijalankan _operator_ `=` untuk menyimpan angka `30` tadi ke dalam variabel `hasil`.

## Jenis-Jenis Operator

Ada banyak sekali operator yang dapat digunakan pada Java. Sebagian di antaranya sering sekali digunakan, sedangkan lainnya jarang digunakan. Berikut operator-operator pada Java yang dikategorikan berdasarkan fungsinya:
1. Operator Aritmatika
2. Operator *Increment* dan *Decrement*
3. Operator *Assignment*
4. Operator Perbandingan
5. Operator Logika
6. Operator Bitwise dan Bit Shift
7. Operator Pada String
8. Operator Ternary

## Selanjutnya

Sampai disini kita sudah kenal dengan istilah operator dan operand. Selanjutnya kita perlu memahami berbagai macam operator yang ada. Di antaranya melakukan assignment dan perhitungan aritmatika dan lain sebagainya.