---
tags: java/struktur-data, rekursif-pada-java
keywords: 
video: 0
published: false
---

# Mencari Deret Fibonacci Menggunakan Rekursif Pada Java

Permasalahan rekursif yang sering dibahas adalah deret Fibonacci. Deret Fibonacci adalah deret bilangan yang nilainya di ambil dari hasil penjumlahan 2 angka sebelumnya. Perhatikan deret Fibonacci berikut:
```text
0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, ...
```

Deret Fibonacci ke 0 adalah 0, deret Fibonacci ke 2 adalah 1, deret Fibonacci ke 6 adalah 8, dan seterusnya.

## Rumus Deret Fibonacci?

Deret Fibonacci memiliki rumus sebagai berikut:
$$
F(n)= \begin{cases} F(n-1) + F(n-2)&untuk\,\,n \gt 1 \\1&untuk\,\,n=1
\\0&untuk\,\,n=0\end{cases}
$$

Rumus tersebut dapat kita baca:

>Jika n besar dari 1, maka Fibonacci ke n adalah penjumlahan antara Fibonacci ke n-1 dan Fibonacci ke n-2. Sedangkan jika n = 1 atau n = 0, maka Fibonacci ke n adalah n itu sendiri.

Dari rumus di atas terlihat jelas bahwa rumus Fibonacci di atas adalah rumus rekursif. Kita dapat implementasi langsung rumus Fibonacci tersebut ke dalam kode program Java seperti berikut ini:

```java
public class Fibonacci {
	public static void main(String[] args) {
		int n = 8;
		System.out.println("Fibonacci ke 8 adalah " + F(n));
	}
	public static int F(int n) {
		if(n > 1) {
			return F(n-1) + F(n-2);
		} else if(n = 1) {
			return 1;
		} else {
			return 0;
		}
	}
}
```

Penjelasan per kondisi
Mengapa menggunakan return
Selanjutnya