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

Selain `true` atau `false`, boolean juga dapat diisi dengan expression yang menghasilkan `true` atau `false`, seperti contoh program berikut:

```java
public class Main {
  public static void main(String[] args) {
    int nilai = 89;
    boolean lulus = nilai > 65;
    System.out.println(lulus);
  }
}
```

Expression `nilai > 65` pada kode program di atas menghasilkan `true` atau `false`, bergantung kepada angka pada variabel `nilai`. Apabila angka pada variabel `nilai` lebih besar dari 65, maka expression `nilai > 65` akan menghasilkan `true`. Begitu juga sebaliknya.

> Eksperimen: cobalah mengganti angka pada variabel `nilai` menjadi angka 50, kemudian jalankan kembali kode program tersebut. Perhatikan output yang dihasilkan!

