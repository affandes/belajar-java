# Membuat program Hello World pada Java - Cara mudah memulai membuat program Java untuk pemula
Cara paling mudah untuk memulai membuat program Java adalah dengan membuat program Hello World. Yuk kita mulai!

## Membuat file Java
Ketik kode berikut ini menggunakan Text Editor seperti NotePad atau sejenisnya.
```java
public class Main {
	public static void main(String[] args) {
		System.out.println("Hello world");
	}
}
```

> **Catatan**: usahakan sama persis seperti kode di atas, termasuk huruf kapital, huruf kecil, spasi, tanda titik, koma dan titik-koma.

Kemudian simpan dengan nama `Main.java`. 

## Menyimpan file Java
File `Main.java` dapat disimpan pada direktori yang sudah kita siapkan, misalnya `C:\dev` (untuk pengguna Windows) atau `/home/user/dev` (untuk pengguna Linux) atau `/Users/budi/dev` (untuk pengguna Mac). 
Kita juga bisa simpan pada direktori lainnya yang mudah untuk diakses. Hindari menyimpan pada direktori yang digunakan untuk sistem, atau direktori yang terkunci. Ada banyak pilihan direktori yang bisa kita gunakan. Tidak ada keharusan menyimpan pada direktori khusus.

## Menjalankan file Java
Misalkan kita sudah memiliki file `Main.java` pada direktori `C:\dev`, buka aplikasi terminal/console/command line, kemudian akses direktori `C:\dev`. Kemudian jalankan perintah berikut:

```shell
$ javac Main.java
```

> Perhatian: simbol $ tidak perlu ditulis pada terminal, karena biasanya sudah otomatis tertulis pada terminal.

Perintah di atas adalah perintah untuk meng-compile file `Main.java` dan diubah menjadi file `Main.class`. Setelah berhasil, kita lanjutkan untuk menjalankan program hasil compile dengan menjalankan perintah berikut:

```shell
$ java Main
```

Setelah dijalankan perintah di atas, akan muncul hasil output sebagai berikut:

```shell
Hello world
```

Selamat! Kita sudah berhasil membuat program Hello world menggunakan Java. Dengan begitu kita bisa [lanjut mempelajari materi berikutnya](#selanjutnya).

## Gimana jika tidak berhasil?
Biasanya yang membuat program Hello world tidak dapat dijalankan adalah:
1. [Penulisan kode program yang tidak tepat](membuat-program-hello-world-pada-java.md#penulisan-kode-program-yang-tidak-tepat).
2. Belum ada [JDK (Java Development Kit) yang terinstall](membuat-program-hello-world-pada-java.md#instalasi-jdk) dengan benar pada komputer.

### Penulisan kode program yang tidak tepat
Ketika menulikan kode program Java, sebaiknya kita perlu memperhatikan hal-hal berikut:
1. Perhatikan huruf kapital dan huruf kecil, beberapa kode yang seharusnya ditulis dengan huruf kecil tidak akan dapat dijalankan jika ditulis dengan huruf besar. Begitu juga sebaliknya.
2. Perhatikan spasi, tanda titik, koma, titik-koma dan simbol lainnya. Simbol-simbol tersebut harus ditulis sesuai dengan yang seharusnya, tidak dapat diubah-ubah sembarangan.
3. Perhatikan tanda kurung. Berbagai jenis tanda kurung punya kegunaan masing-masing. Tanda kurang `[]` tidak dapat diganti dengan tanda `()`. Penggunaan tanda kurung yang salah dapat membuat program tidak dapat dijalankan.

> Pelajari lebih lanjut tentang [cara penulisan program Java yang wajib kita ketahui](cara-penulisan-program-java-yang-wajib-kita-ketahui).

### Instalasi JDK
Penyebab lain yang membuat kode program Java tidak dapat dijalankan adalah JDK yang tidak terinstal dengan baik. JDK (Java Development Kit) adalah program yang digunakan untuk menjalankan kode program Java. 
Jika JDK belum terinstal dengan baik di komputer kita, silahkan pelajari lebih lanjut tentang cara instalasi JDK berikut ini:
1. Instalasi JDK untuk pengguna Windows
2. Instalasi JDK untuk pengguna Linux
3. Instalasi JDK untuk pengguna Mac
4. Apa saja JDK yang banyak digunakan programmer Java?
5. Instalasi beberapa versi JDK untuk pengguna Windows
6. Instalasi beberapa versi JDK untuk pengguna Linux
7. Instalasi beberapa versi JDK untuk pengguna Mac

## Selanjutnya
