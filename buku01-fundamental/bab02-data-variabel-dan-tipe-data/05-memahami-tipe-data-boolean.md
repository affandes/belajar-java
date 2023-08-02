---
tags: java/fundamental, data-variabel-dan-tipe-data-pada-java
keywords: tipe data, boolean
video: 0
published: false
---
# Memahami Tipe Data Boolean

Tipe data boolean adalah tipe data yang paling sederhana, namun kenyataannya tipe data ini sangat banyak digunakan di dalam kode program manapun. Karena tipe data ini menentukan logika pemrograman yang dibuat. 

Secara sederhana, tipe data ini hanya bernilai `true` atau `false` saja. Perhatikan contoh kode program berikut:
  
```java
public class Main {
  public static void main(String[] args) {
    boolean lulus = true;
    boolean bisaTerbang = false;
    System.out.println(lulus);
    System.out.println(bisaTerbang);
  }
}
```

Selain `true` atau `false`, boolean juga dapat diisi dengan *expression* yang menghasilkan `true` atau `false`, seperti contoh program berikut:

```java
public class Main {
  public static void main(String[] args) {
    int nilai = 89;
    boolean lulus = nilai > 65;
    System.out.println(lulus);
  }
}
```

*Expression* `nilai > 65` pada kode program di atas menghasilkan `true` atau `false`, bergantung kepada angka pada variabel `nilai`. Apabila angka pada variabel `nilai` lebih besar dari 65, maka *expression* `nilai > 65` akan menghasilkan `true`. Begitu juga sebaliknya.

> Eksperimen: cobalah mengganti angka pada variabel `nilai` menjadi angka 50, kemudian jalankan kembali kode program tersebut. Perhatikan output yang dihasilkan!

Ada banyak sekali *expression* yang dapat menghasilkan `true` atau `false`, perhatikan contoh kode program berikut:

```java
public class Main {
  public static void main(String[] args) {
    int a = 9;
    int b = 10;
    boolean x = a < b;
    boolean y = a + 1 >= b;
    boolean z = a != b;
    System.out.println(x);
    System.out.println(y);
    System.out.println(z);
  }
}
```

Ketiga *expression* di atas jika ditampilkan ke layar akan menghasilkan *output* berikut:

```shell
true
true
true
```

Untuk memahami lebih lanjut tentang bagaimana cara membuat *expression* yang menghasilkan `true` atau `false` kita dapat mempelajari tentang [Operator, Expression](01-kenalan-dengan-operator-operand-dan-expression-pada-java.md), Statement dan Block.

## Kesimpulan

Untuk saat ini, kita sudah mengetahui tentang tipe data boolean dan berbagai cara membuat variabel boolean. Penggunaan tipe data boolean cukup banyak digunakan di dalam kode program. Materi tersebut akan kita pelajari pada Percabangan.

Selanjutnya kita masih harus memahami satu lagi tipe data yang biasa digunakan pada Java, yaitu [Tipe Data String](06-memahami-tipe-data-string.md).