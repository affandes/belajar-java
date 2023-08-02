# Memahami Tipe Data String

Tipe Data String tidak termasuk ke dalam Tipe Data Primitif pada Java. String termasuk ke dalam Tipe Data Referensi atau Nonprimitif. Coba perhatikan kode program berikut:

```java
public class Main {
  public static void main(String[] args) {
    String nama = "Budi";
    System.out.println(nama);
  }
}
```

Kode di atas akan menghasilkan output seperti berikut:

```shell
Budi
```

Literal String dapat dibuat menggunakan tanda kutip-ganda `"` pada awal dan akhir literal. Sedangkan tanda kutip satu hanya digunakan untuk membuat *char*. 

## Membuat Variabel String

Ada dua cara membuat sebuah variabel String, perhatikan kode program berikut:

```java
public class Main {
  public static void main(String[] args) {
    String nama = "Budi";
    String prodi = new String("Teknik Informatika");
    System.out.println(nama);
    System.out.println(prodi);
  }
}
```

Cara pertama tentunya cara yang biasanya dilakukan, sedangkan cara kedua menggunakan kata kunci `new String()`. Kedua cara ini akan sama-sama menghasilkan variabel dengan tipe data String.

## Operasi pada String

Sebuah variabel String memiliki operasi-operasi tertentu yang membantu dalam mengelola isi dari variabel String tersebut. Hal ini karena String adalah Tipe Data Referensi, sehingga memiliki operasi yang mungkin berguna. Perhatikan kode program berikut:

```java
public class Main {
  public static void main(String[] args) {
    String nama = "Budi";
    String namaKapital = nama.toUpperCase();
    System.out.println(nama);
    System.out.println(namaKapital);
  }
}
```

Ketika kode program dijalankan, akan menghasilkan output seperti berikut:

```shell
Budi
BUDI
```

Operasi `nama.toUpperCase()` berguna untuk mengubah teks menjadi huruf kapital. Selain itu, ada beberapa operasi lainnya yang perlu kita ketahui:

No | Operasi | Deskripsi
---|---|---
1 | charAt | Menghasilkan char pada posisi indeks yang diinginkan
2 | concat | Menggabungkan dua buah String
3 | equals | Membandingkan du buat String
4 | length | Menghasilkan jumlah String
5 | replace | Mengubah isi String
6 | substring | Menghasilkan sebagian dari isi String
7 | toLowerCase | Mengubah isi String menjadi huruf kecil
8 | toUpperCase | Mengubah isi String menjadi huruf kapital
9 | trim | Menghilangkan spasi di awal dan di akhir

Dan masih ada beberapa operasi lainnya yang dapat digunakan pada String. Bagi kalian yang tertarik mempelajari lebih lengkap tentang operasi pada String, dapat dipelajari pada website [W3School](https://www.w3schools.com/java/java_ref_string.asp).

## Kesimpulan

Kita sudah mempelajari tentang berbagai tipe data dasar pada Java. Tipe-tipe dasar ini sangat banyak digunakan dalam pembuatan program menggunakan Java. Untuk memahami cara menggunakan tipe data tersebut, kita dapat mempelajari tentang [Operator, Expression](../bab03-operator-expression-statement-block/01-kenalan-dengan-operator-operand-dan-expression-pada-java.md), Statement dan Block.