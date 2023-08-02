# Inilah Error yang Paling Sering Dilakukan Programmer Java Pemula

Ketika kita baru belajar pemrograman Java, pastinya tidak akan luput dari error. Mungkin saja karena lupa titik-koma (`;`) atau pun lupa tanda titik (`.`) bisa menyebabkan kita frustasi dalam mencari penyebab errornya. 

Berikut beberapa error yang biasanya dilakukan oleh para programmer Java pemula selama proses belajar pemrograman dan membuat kode program. Diharapkan kita dapat lebih memahami masing-masing pesan error tersebut dan segera memperbaiki kode program kita.

## Cannot find symbol

Pernahkah kalian mendapatkan pesan error seperti ini?

```shell
./Main.java:3: error: cannot find symbol
  symbol:   variable panjang
  location: class Main
```

Ketika pesan error tersebut tertulis `cannot find symbol`, berarti:
1. Bisa jadi kita menggunakan variabel yang belum pernah dideklarasikan sebelumnya. Misalnya kita punya kode program `int hasil = panjang * lebar` sedangkan variabel `panjang` atau `lebar` belum pernah kita buat sebelumnya. Berikut contoh kode program yang akan menghasilkan error seperti di atas.
  ```java
  public class Main {
    public static void main(String[] args) {
      int hasil = panjang * lebar;
      System.out.println(hasil);
    }
  }
  ```
2. Bisa jadi kita menggunakan variabel yang sudah dideklarasikan sebelumnya, namun kita tidak menuliskan nama variabel tersebut dengan sama persis. Misalnya kita punya kode program `int hasil = Panjang * Lebar` sedangkan variabel yang kita deklarasikan adalah `panjang` atau `lebar`, hal ini menyebabkan program tidak dapat mengenali variabel yang kita tulis karena perbedaan huruf kapital dan huruf kecil. Berikut contoh kode program yang akan menghasilkan error seperti di atas.
  ```java
  public class Main {
    public static void main(String[] args) {
      int panjang = 10;
      int lebar = 8;
      int hasil = Panjang * Lebar;
      System.out.println(hasil);
    }
  }
  ```
3. Bisa jadi kita sebenarnya tidak memanggil sebuah variabel, tetapi menggunakan String sebagai literal, namun kita lupa menambahkan tanda kutip ganda di awal dan di akhir literal String tersebut. Misalnya kita punya kode program `String nama = Budi`, sedangkan literal `Budi` tersebut dimaksudkan sebagai data nama, bukan variabel.
  ```java
  public class Main {
    public static void main(String[] args) {
      String nama = Budi;
      System.out.println(nama);
    }
  }
  ```

