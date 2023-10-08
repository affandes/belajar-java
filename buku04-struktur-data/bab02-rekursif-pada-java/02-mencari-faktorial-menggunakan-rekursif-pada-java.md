---
tags: java/struktur-data, rekursif-pada-java
keywords: 
video: 0
published: false
---
# Mencari Faktorial Menggunakan Rekursif Pada Java

Di dalam ilmu Matematika, Faktorial adalah hasil perkalian bilangan bulat positif dari 1 sampai n. Misalnya Faktorial dari 5 dilambangkan dengan 5! berarti hasil perkalian dari 1 x 2 x 3 x 4 x 5 yaitu 120. 

Operasi Faktorial adalah salah satu operasi matematika yang sering digunakan dalam pemrograman. Dalam pemrograman Java, kita dapat menghitung faktorial dengan menggunakan fungsi rekursif. 

## Rumus Faktorial

Faktorial dilambangkan dengan simbol `!` (tanda seru), perhatikan contoh berikut:
- Faktorial 5 dilambangkan dengan 5!
- Faktorial 7 dilambangkan dengan 7!
- dan seterusnya

Di dalam notasi Matematika, rumus Faktorial ditulis sebagai berikut:
$$
n! = n \times (n-1) \times ... \times 1
$$
Misalnya:
$$
5!=5 \times 4 \times 3 \times 2 \times 1
$$
Secara singkat, rumus dari Faktorial dapat ditulis sebagai berikut:
$$
n!=\prod \limits_{k=1}^{n} {k}
$$
Rumus di atas sebenarnya mirip, hanya notasi saja yang membedakan. Tapi perlu diketahui, notasi rumus di atas sebenarnya adalah notasi yang memanfaatkan perulangan. Simbol di atas dapat dibaca dengan,

>*Perkalian setiap nilai k dimana k bernilai dari 1 sampai n*

Apabila nilai n = 5, maka dilakukan operasi perkalian dari k = 1 sampai k = 5. Sehingga perhitungan nya menjadi seperti berikut:
$$
5! = 1 \times 2 \times 3 \times 4 \times 5 = 120
$$
Di dalam pemrograman Java, rumus ini dapat ditulis menjadi kode program sebagai berikut:

```java
public class Faktorial {
	public static void main(String[] args) {
		int n = 5;
		int faktorial = 1;
		for(int k = 1; k <= n; k++) {
			faktorial = faktorial * k;	
		}
		System.out.println("Hasil = " + faktorial);
	}
}
```

Ketika kode program ini dijalankan akan menghasilkan output seperti berikut:

```shell
Hasil = 120
```

Lalu dimana rekursifnya? 

Kode program di atas bukanlah kode program Faktorial yang menggunakan Rekursif. Karena memang rumus Faktorial yang digunakan juga bukan rumus Faktorial yang Rekursif. Lalu adakah rumus Faktorial yang Rekursif? Ada.

## Rumus Faktorial Rekursif

Berbeda dari rumus sebelumnya, rumus Faktorial Rekursif adalah seperti ini:
$$
n!= \begin{cases} n \cdot(n-1)!&untuk\,\,n \ge 1 \\1&untuk\,\,n=0\end{cases}
$$
Kita bisa membaca rumus tersebut dengan cara,

>Jika n lebih besar atau sama dengan 1, maka Faktorial n adalah n dikali dengan Faktorial (n-1), jika n = 0, maka Faktorial n = 1

Dari penjelasan di atas, dapat kita pahami bahwa rumus Faktorial di atas menggunakan rekursif. Jelas terlihat di dalam fungsi Faktorial, terdapat rumus perkalian antara `n` dan fungsi Faktorial itu sendiri. Sehingga jika kita implementasikan ke dalam bahasa pemrograman Java, maka akan menghasilkan kode program sebagai berikut:

```java
public class Faktorial {
	public static void main(String[] args) {
		int n = 5;
		int hasil = faktorial(n);
		System.out.println("Hasil = " + hasil);
	}
	public static int faktorial(int n) {
		if(n >= 1) {
			return n * faktorial(n-1);
		} else {
			return 1;
		}
	}
}
```

Ketika kode program tersebut dijalankan akan menghasilkan output sebagai berikut:

```shell
Hasil = 120
```

## Kesimpulan

Permasalahan faktorial sebenarnya dapat diselesaikan dengan pendekatan perulangan ataupun dengan rekursif. Tentunya masing-masing punya teknik tersendiri. Dengan kita memahami rekursif kita mengetahui bahwa ada cara lain dalam menyelesaikan permasalahan perulangan.