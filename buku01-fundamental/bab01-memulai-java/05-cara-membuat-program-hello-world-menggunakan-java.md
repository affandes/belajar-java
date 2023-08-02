---
tags: java/fundamental, memulai-java
keywords: hello world
video: 0
published: false
---
# Cara Membuat Program Hello World Menggunakan Java

Buat kita yang memulai belajar Java, penting bagi kita mengetahui kesiapan dalam belajar. Cara paling populer adalah membuat program Hello World.

## Apa itu Program Hello World?

Sederhananya, program Hello World hanya program yang menampilkan *output* "Hello World".

```java
Hello World
```

Tidak penting kata apa yang mau di-*output*-kan, bisa "Hello World", "Salam" atau lainnya. Apabila kita berhasil membuat program Hello World berarti kita sudah siap untuk belajar bahasa pemrograman tersebut.

## Gimana Cara Membuat Program Hello World Menggunakan Java?

Sebelum membuat program Hello World, kita perlu mempersiapkan hal-hal berikut:
1. Pastikan kita sudah install **Java Development Kit (JDK)** dengan benar. Pelajari lebih lanjut tentang cara instalasi JDK untuk pengguna Windows.
2. Siapkan juga **Editor** untuk menulis kode program, kita bisa gunakan Integrated Development Environment (IDE) atau Code Editor atau Text Editor, misalnya IntelliJ IDEA, NetBeans, Visual Studio Code ataupun Notepad.

> Jika kita belum instalasi JDK, pelajari lebih lanjut tentang [Cara Instalasi JDK pada Windows](02-cara-instalasi-jdk-pada-windows.md). 

Setelah semua hal di atas dipersiapkan, barulah kita lanjut membuat program Hello World. Berikut langka-langkahnya,
1. Buat direktori untuk menyimpan file program Hello World.
2. Buat file `HelloWorld.java` di dalam direktori yang sudah dibuat pada langkah sebelumnya.
3. *Compile* file `HelloWorld.java`.
4. Jalankan program Hello World.

Kita bahas langkah-langkah di atas dengan lebih rinci sebagai berikut.

### Langkah 1. Buat direktori

Buat sebuah direktori atau *folder* untuk menyimpan program Hello World. Nama direktori dapat disesuaikan dengan kebutuhan, misalnya: `hello world` atau `hello-world`. Tidak ada aturan khusus dalam pembuatan nama direktori dan dimana lokasi direktori dibuat. Kita dapat menyesuaikan nama direktori dan lokasi direktori dibuat.

Bagi pengguna Windows, kita bisa buat direktori pada `C:\dev` atau direktori lain. Untuk pengguna Linux dapat dibuat pada `/home/yourname/dev`. Untuk pengguna MacOS bisa dibuat pada direktori `/Users/yourname/dev`.

### Langkah 2. Buat file `HelloWorld.java`

Buat sebuah file `HelloWorld.java` menggunakan *Editor*, kemudian ketik kode program berikut:

```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello World");
  }
}
```

Kemudian simpan file tersebut ke dalam direktori yang sudah kita siapkan sebelumnya.

### Langkah 3. Compile file `HelloWorld.java`

Kode program Java yang sudah kita tulis sebelumnya harus di-*compile* terlebih dahulu sebelum bisa dijalankan. File `HelloWorld.java` tadi akan diubah menjadi file `HelloWorld.class` setelah di-*compile*.

Untuk meng-*compile* file `HelloWorld.java` kita perlu menggunakan aplikasi Terminal (untuk pengguna Linux atau MacOS) atau Command Line (untuk pengguna Windows). Jalankan program tersebut, kemudian akses direktori yang digunakan untuk menyimpan file `HelloWorld.java` sebelumnya.

![Akses direktori menggunakan Terminal](aset/carbon-cli-open-terminal.png)

*Compile* file `HelloWorld.java` menggunakan perintah berikut:

```shell
$ javac HelloWorld.java
```

Setelah berhasil akan keluar sebuah file baru dengan nama `HelloWorld.class` yang merupakan file *binary* yang dapat dijalankan oleh Java.

### Langkah 4. Menjalankan program Hello World

Untuk menjalankan program Hello World yang sudah di-*compile* dapat menggunakan perintah berikut:

```shell
$ java HelloWorld
```

Setelah dijalankan akan keluar tulisan `Hello World` seperti berikut:

```shell
Hello World
```

Inilah program Hello World yang sudah kita buat menggunakan bahasa Java. Berjalannya program Hello World tersebut menunjukkan bahwa kita sudah siap untuk belajar pemrograman Java berikutnya.

## Selanjutnya

Berikut materi-materi yang dapat kita pelajari selanjutnya:
1. [Menggunakan komentar di dalam kode program Java](06-apa-itu-komentar-pada-java.md)
2. Mengetahui beberapa [aturan sederhana dalam menulis kode program Java](07-3-aturan-wajib-diketahui-saat-menulis-program-java.md)
3. Mempelajari tentang [Data, Variabel dan Tipe Data](../bab02-data-variabel-dan-tipe-data/01-kenalan-dengan-variabel-dan-tipe-data-pada-java.md)