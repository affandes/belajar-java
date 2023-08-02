---
tags: java/fundamental, memulai-java
keywords: komentar, comment
video: 0
published: false
---
# Apa itu Komentar pada Java

Sebelum kita membahas lebih jauh tentang Komentar pada kode program Java, perhatikan kode program berikut:

```java
public class Main {
  public static void main(String[] args) {
    
    // Membuat variabel
    String nama = "Andi";
    
    // Menampilkan isi variabel
    System.out.println(nama);
    
  }
}
```

Baris kode program yang diawali dengan simbol "//" merupakan Komentar. Setiap komentar pada kode program Java **tidak akan dieksekusi** atau diproses untuk dijalankan. Sehingga kita dapat menuliskan apapun sesuai dengan kebutuhan.

## Untuk Apa Komentar?

Komentar digunakan untuk memberikan catatan atau informasi tambahan terhadap kode program. Catatan dapat berupa penjelasan fungsi dari kode program, atau nama programmer yang menulis kode program tersebut.

Komentar hanya ditujukan untuk programmer atau siapapun yang membaca kode program. Komentar tidak ditujukan untuk komputer, karena komputer tidak akan memproses Komentar saat mengeksekusi kode program.

## Cara Menggunakan Komentar

Ada beberapa cara menggunakan komentar, di antaranya:
1. *Inline*, komentar **pada baris** kode program.
2. *Single line*, komentar **untuk satu baris** kode program.
3. *Multi line*, komentar **untuk banyak baris** kode program.

Berikut contoh penggunaan komentar pada kode program:

```java
public class Main {
  public static void main(String[] args) {
    
    // Membuat variabel
    String nama = "Andi";
    int nilai = 78;
    
    // Menampilkan isi variabel
    System.out.println(nama);
    
    /*
    Jika nilai lebih besar dari 50,
    maka tampilkan pesan lulus, jika
    tidak maka tampilkan pesan gagal.
    */
    if(nilai > 50) {
      System.out.println("Selamat Anda Lulus!"); // Pesan lulus
    } else {
      System.out.println("Anda Tidak Lulus"); // Pesan tidak lulus
    }
    
  }
}
```

Ada perbedaan antara komentar *single-line* dan komentar *multi-line*. Pada *single-line* kita menggunakan simbol garis miring ganda "**//**" di awal komentar, sedangkan pada komentar *multi-line* kita menggunakan simbol garis miring dan asteriks "**/\***" di awal komentar dan ditutup dengan asteriks dan garis miring "**\*/**" di akhir komentar.

Sampai disini gimana? Sudah paham kah cara menggunakan komentar pada Java?

> Pelajari selanjutnya tentang [Data, Variabel dan Tipe Data](../bab02-data-variabel-dan-tipe-data/01-kenalan-dengan-variabel-dan-tipe-data-pada-java.md).