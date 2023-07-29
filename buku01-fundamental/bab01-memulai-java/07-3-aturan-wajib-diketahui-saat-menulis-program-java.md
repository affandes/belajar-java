# 3 Aturan Yang Wajib Diketahui Saat Menulis Program Java

Menulis program Java ternyata ada aturannya. Umumnya programmer Java menggunakan aturan-aturan ini. Aturan ini dibuat untuk memudahkan kita membuat program Java. Trus, apa saja aturan-aturan tersebut?

## 1. Case Sensitive

Semua kode program Java bersifat *case sensitive*, berarti teks dengan huruf kecil akan dianggap berbeda dengan teks yang memiliki huruf kapital. Misalnya kata `Hallo` dengan kata `hallo` dianggap berbeda. Dengan begitu, ketika kita ingin menulis kode program Hello World di bawah ini, kita harus menuliskannya persis sama antara huruf kecil dan huruf kapitalnya.

```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello World");
  }
}
```

Perhatikan kode program Hello World di atas, kode program tersebut dimulai dengan kode `public` yang menggunakan huruf kecil. Apabila salah satu huruf tersebut diubah menjadi huruf kapital dan dijalankan, maka kode tersebut tidak akan dapat dijalankan. Ini juga berlaku untuk sebagian besar kode pada Java.

## 2. Indentasi

Setiap kode program Java tidak lepas dari blok kode. Setiap blok dimulai dan diakhiri dengan simbol `{}`. Perhatikan kode berikut ini.

```java
public class SayHello {                         // <-- Awal blok 1
  public static void main(String[] args) {      // <-- Awal blok 2
    System.out.println(say("World"));
  }                                             // <-- Akhir blok 2
  public static String say(String teks) {       // <-- Awal blok 3
    return "Hello " + teks;
  }                                             // <-- Akhir blok 3
}                                               // <-- Akhir blok 1
```

Setiap pergantian kode blok terdapat indentasi berupa spasi di awal setiap baris kode. Indentasi ini digunakan untuk memudahkan kita melihat blok kode program. Jika tidak ada indentasi, kita akan kesulitan membaca kode program. Perhatikan kode program Hello World di bawah ini apabila dihilangkan indentasinya.

```java
public class SayHello {                         // <-- Awal blok 1
public static void main(String[] args) {        // <-- Awal blok 2
System.out.println(say("World"));
}                                               // <-- Akhir blok 2
public static String say(String teks) {         // <-- Awal blok 3
return "Hello " + teks;
}                                               // <-- Akhir blok 3
}                                               // <-- Akhir blok 1
```

Hasilnya dapat kita lihat, kan? Kita sulit melihat blok kode di atas. Tanda kurung yang seharusnya berpasangan akan sulit dilihat, ini memungkinkan kita tidak dapat melihat apakah tanda kurung yang ada di dalam kode program sudah benar. Selain tanda kurung, kita juga kesulitan mencari dan membaca kode program yang ditulis. Inilah pentingnya kita menulis kode program yang rapi dan mudah dibaca. 

Saat ini sudah banyak *editor* yang memudahkan kita merapikan indentasi kode program. Namun begitu, kita tetap harus memperhatikan indentasi kode program yang sudah kita tulis. Karena tidak semua editor bisa langsung otomatis merapikan pada saat kita tulis. Tapi harus menekan tombolnya terlebih dahulu. 

## 3. Nama File dan Nama Class

Perhatikan kembali kode program Hello World di bawah ini.

```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello World");
  }
}
```

Ketika kita menyimpan kode program ini ke dalam file, nama file harus `HelloWorld.java`, tidak boleh berbeda sedikitpun. Nama file dan nama *class* harus mengikut aturan tersebut. Jika tidak, program kita tidak akan dapat dijalankan.

Jadi, ketika kita ingin membuat sebuah program Say Hello dengan kode berikut.

```java
public class SayHello {
  public static void main(String[] args) {
    System.out.println(say("World"));
  }
  public static String say(String teks) {
    return "Hello " + teks;
  }
}
```

Harus kita simpan ke dalam file dengan nama `SayHello.java`. 

## Kesimpulan

Kita sudah mengetahui ketiga aturan dasar dalam menulis kode program Java. Aturan ini diperlukan untuk memudahkan kita dalam menulis kode program. Selain itu juga memudahkan orang lain membaca kode program yang kita tulis.