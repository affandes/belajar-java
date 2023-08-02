---
tags: java/fundamental, operator-expression-statement-block-pada-java
keywords: operator aritmatika, operator
video: 0
published: false
---
# Memahami Operator Aritmatika Pada Java

Operator yang paling umum digunakan adalah Operator Aritmatika. Operator ini digunakan untuk melakukan operasi perhitungan sederhana. Berikut daftar Operator Aritmatika yang dapat digunakan.

Simbol | Contoh | Fungsi
---|---|---
`+` | `a + b` | Menjumlahkan `a` dan `b` 
`-` | `a - b` | Mengurangi `a` dengan `b`
`*` | `a * b` | Mengalikan `a` dengan `b`
`/` | `a / b` | Membagi `a` dengan `b`
`%` | `a % b` | Modulus `a` dengan `b`

## Cara Menggunakan Operator Aritmatika

Perhatikan kode program berikut:

```java
public class Main {
  public static void main(String[] args) {
    int a = 10;
    int b = 8;
    int c = a + b;
    int d = b - a;
    int e = 2 + c - 2 * d;
    System.out.println(c);
    System.out.println(d);
    System.out.println(e);
  }
}
```

Operator Aritmatika digunakan pada literal dan variabel dengan tipe data numerik seperti int, long, short, byte, double, float dan char. Perhatikan kode program berikut:

```java
public class Main {
  public static void main(String[] args) {
    char x = 'A' + 2;
    int y = 2 + 'A';
    System.out.println(x);
    System.out.println(y);
  }
}
```
