---
tags: java/struktur-data, rekursif-pada-java
keywords: 
video: 0
published: false
---
# Mengenal Rekursif Pada Java

Rekursif (recursive) merupakan sifat dari suatu prosedur atau algoritma, sedangkan rekursi (recursion) adalah objek prosedur atau algoritma itu sendiri. Secara bahasa, rekursif berarti suatu aturan atau prosedur yang dapat diterapkan berulang-ulang.

Rekursif pada pemrograman juga dapat diartikan dengan suatu konsep pemrograman yang memungkinkan sebuah fungsi dapat memanggil fungsi itu sendiri. Tujuan memanggil dirinya sendiri adalah untuk menghasilkan proses perulangan dengan pola tertentu dan batasan tertentu.

## Antara Perulangan dan Rekursif

Untuk memudahkan kita memahami perbedaan antara Perulangan dan Rekursif, perhatikan kode program berikut ini:

```java
public class Main {
	public static void main(String[] args) {
		for(int i = 0; i < 10; i++) {
			System.out.println("Nomor " + i);
		}
	}
}
```

Kode program di atas adalah contoh kode perulangan pada Java menggunakan `for`. Perhatikan kode program rekursif berikut ini:

```java
public class Faktorial {
	public static int hitungFaktorial(int n) {
		if (n == 0) {
			return 1;
		} else {
			return n * hitungFaktorial(n - 1);
		}
	}

	public static void main(String[] args) {
		int n = 5;
		int hasilFaktorial = hitungFaktorial(n);
		System.out.println("Faktorial dari " + n + " adalah " + hasilFaktorial);
	}
}
```

Dari kedua kode program di atas terlihat jelas perbedaan antara perulangan dan rekursif. Hal penting yang perlu digarisbawahi adalah:
1. Rekursif tidak menggunakan statement `for` atau `while` untuk melakukan looping, sedangkan pada Perulangan (iterasi) menggunakan statement `for` atau `while` untuk melakukan looping.
2. Rekursif harus menggunakan fungsi atau method untuk melakukan looping, sedangkan pada Perulangan (iterasi) cukup menggunakan statement `for` atau `while` untuk melakukan looping.
3. Rekursif harus menggunakan statement `if` atau `switch` untuk melakukan looping, sedangkan Perulangan (iterasi) tidak harus menggunakan statement `if` atau `switch` untuk melakukan looping.

## Contoh Rekursif

Berikut adalah salah satu contoh kode program Rekursif menggunakan Java.

```java
public class Faktorial {
	public static int hitungFaktorial(int n) {
		if (n == 0) {
			return 1;
		} else {
			return n * hitungFaktorial(n - 1);
		}
	}

	public static void main(String[] args) {
		int n = 5;
		int hasilFaktorial = hitungFaktorial(n);
		System.out.println("Faktorial dari " + n + " adalah " + hasilFaktorial);
	}
}
```

Perhatikan fungsi atau method `hitungFaktorial` di atas. Method tersebut adalah method yang Rekursif. Karena di dalam method `hitungFaktorial` terdapat kode program yang memanggil method `hitungFaktorial` itu sendiri. Namun, setiap kali method tersebut dipanggil, nilai variabel `n` selalu dikurangi dengan 1. Sehingga program harus menyelesaikan setiap method yang dipanggil secara berulang-ulang. 

Ketika kode program tersebut dijalankan, kita akan melihat output sebagai berikut:
```shell
Faktorial dari 5 adalah 120
```

## Memahami Konsep Rekursif

Ada dua elemen di dalam sebuah fungsi Rekursif, antara lain:
1. Kasus Basis (Base Case) yaitu kondisi yang menyatakan Rekursif harus berhenti. Rekursif akan terus berulang jika kondisi ini tidak terpenuhi.
2. Kasus Berulang (Inductive Case) yaitu langkah berulang yang digunakan untuk menyelesaikan masalah pemrograman.

```java
public class Faktorial {
	public static int hitungFaktorial(int n) {
		if (n == 0) {                                 // -->> Kasus Basis
			return 1;
		} else {
			return n * hitungFaktorial(n - 1);          // -->> Kasus Berulang
		}
	}

	public static void main(String[] args) {
		int n = 5;
		int hasilFaktorial = hitungFaktorial(n);
		System.out.println("Faktorial dari " + n + " adalah " + hasilFaktorial);
	}
}
```

Kedua elemen pada fungsi Rekursif dapat dikenali dengan mudah. Misalnya saja Kasus Berulang, dapat ditandai dengan kode program yang memanggil nama fungsinya sendiri. Sedangkan Kasus Basis tidak ditandai dengan pemanggilan nama fungsinya sendiri. Dan, kedua jenis elemen ini berada di dalam statement kondisi `if` atau `switch`. 

## Studi Kasus: Faktorial

Pada dasarnya, rumus faktorial dapat kita selesaikan dengan cara perulangan biasa, seperti kode program berikut ini:

```java
public class Faktorial {
	public static void main(String[] args) {
		int n = 5;
		int hasil = 1;
		for(int i = 1; i <= 5; i++) {
			hasil = hasil * i;
		}
		System.out.println("Faktorial dari " + n + " adalah " + hasil);
	}
}
```

Kode program di atas akan menghasilkan output yang sama dengan kode yang menggunakan Rekursif. Berikut adalah kode program Faktorial menggunakan Rekursif:

```java
public class Faktorial {
	public static int hitungFaktorial(int n) {
		if (n == 0) {
			return 1;
		} else {
			return n * hitungFaktorial(n - 1);
		}
	}

	public static void main(String[] args) {
		int n = 5;
		int hasilFaktorial = hitungFaktorial(n);
		System.out.println("Faktorial dari " + n + " adalah " + hasilFaktorial);
	}
}
```

## Kesimpulan

Rekursif punya banyak kesamaan dengan perulangan, namun menghasilkan kode program yang berbeda dengan perulangan. 