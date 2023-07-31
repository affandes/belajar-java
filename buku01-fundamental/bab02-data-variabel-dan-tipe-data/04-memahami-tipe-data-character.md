# Memahami Tipe Data Character

Character adalah tipe data yang unik di Java. Selain termasuk ke dalam tipe data numerik (angka), tipe data ini sebenarnya mewakili karakter atau simbol satuan pada teks. Perhatikan contoh kode program berikut:

```java
public class Main {
  public static void main(String[] args) {
    char label = 'A';
    System.out.println(label);
  }
}
```

Sekilas variabel label di atas mirip dengan tipe data String. Namun variabel label bukanlah String, tetapi tipe data *char* atau Character. Berikut beberapa perbedaan antara Character dan String.

Character | String
--- | ---
Merepresentasikan 1 karakter teks atau huruf atau simbol | Merepresentasikan kumpulan karakter yang menjadi sebuah teks
Menggunakan tanda kutip satu | Menggunakan tanda kutip ganda
Dapat direpresentasikan dengan angka | Tidak dapat direpresentasikan dengan angka

## Membuat Variabel Char

Untuk membuat variabel *char*, kita dapat menggunakan tanda kutip satu dan diikuti dengan 1 karakter saja, tidak dapat diisi lebih dari satu karakter ataupun kurang dari 1 karakter. Variabel char juga dapat dibuat dengan angka ataupun dengan kode Unicode. Perhatikan kode program berikut:

```java
public class Main {
  public static void main(String[] args) {
    char huruf = 'Z';
    char simbolPersen = '%';
    char simbol = 66;
    char kode = '\u03A9';
    System.out.println(huruf);
    System.out.println(simbolPersen);
    System.out.println(simbol);
    System.out.println(kode);
  }
}
```

Output yang dihasilkan adalah sebagai berikut:

```shell
Z
%
B
Ω
```

## Kesimpulan

Kita sudah mempelajari tentang tipe data char dan cara membuat variabel char. Selanjutnya kita dapat mempelajari tentang [Tipe Data Boolean](05-memahami-tipe-data-boolean.md).