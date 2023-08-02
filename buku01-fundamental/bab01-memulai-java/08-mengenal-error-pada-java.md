# Mengenal Error pada Java

Error sering kali terjadi ketika kita membuat kode program, khususnya di Java. Karena Java termasuk bahasa pemrograman yang cukup ketat aturan penulisannya. Sehingga, kesalahan sedikit saja dapat menyebab terjadi error di kode program kita.

## Apa itu Error?

Secara sederhana, Error adalah kesalahan pada penulisan kode program yang menyebabkan program tidak dapat dijalankan. Coba perhatikan contoh kode program berikut ini.

```java
public class Main {
  public static void main(String[] args) {
    int nama = "Budi";
    System.out.println(nama);
  }
}
```

Ketika kode program di atas di-compile, maka akan terjadi error yang menghasilkan pesan error sebagai berikut:

```shell
./Main.java:3: error: incompatible types: String cannot be converted to int
    int nama = "Budi";
               ^
1 error
```

Pada tahapan ini kita dapat mengetahui bahwa:
1. Telah terjadi error pada kode program yang kita buat
2. Setiap error menyebabkan kode program secara keseluruhan tidak dapat dijalankan

## Memahami Error pada Java

Setiap kali terjadi error, Java selalu memberikan pesan error yang cukup membantu kita mengetahui sumber permasalahan yang terjadi. Coba perhatikan kembali pesan error berikut!

```shell
./Main.java:3: error: incompatible types: String cannot be converted to int
    int nama = "Budi";
               ^
1 error
```

Dari pesan error di atas, kita dapat beberapa informasi sebagai berikut:
1. Pesan `Main.java:3` pada pesan error di atas menunjukkan bahwa terdapat error pada file `Main.java` pada baris ke `3`. 
2. Pesan `incompatible types: String cannot be converted to int` menunjukkan informasi error yang terjadi karena `String` tidak dapat dikonversi ke `int`. Biasanya kesalahan seperti ini terjadi karena kita salah menentukan tipe data. 
3. Pesan `int nama = "Budi"` menunjukkan baris kode program yang berada pada file `Main.java` baris ke `3` yang menjadi penyebab error terjadi. Terdapat tanda panah ke atas `^` yang menunjukkan posisi kode program yang bermasalah.
4. Pesan `1 error` menunjukkan jumlah penyebab error yang ditemukan.

Dari pesan error di atas, sebenarnya kita sudah memiliki cukup informasi untuk mencari penyebab terjadinya error. Dengan demikian, kita akan dimudahkan dalam membuat kode program.

> Pelajari [beberapa pesan error yang biasa dilakukan oleh programmer Java](09-inilah-error-yang-paling-sering-dilakukan-programmer-java-pemula.md) yang baru belajar pemrograman

## Selanjutnya

Selain error, ada juga istilah lain yaitu Bug. Antara error dan bug memiliki ciri-ciri yang berbeda. Yuk pelajari lebih lanjut tentang Bug pada Java.

