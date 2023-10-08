---
tags: java/struktur-data, tipe-data-abstrak-pada-java
keywords: 
video: 0
published: false
---
# Struktur Data dan Manfaatnya

Pernahkan kita membuat program sederhana yang menyimpan nama seseorang pada sebuah variabel `String`? Perhatikan contoh kode program berikut:

```java
public class Main {
	public static void main(String[] args) {
		String nama = "Budi";
		System.out.printlnz("Hai " + nama);
	}
}
```

Kode program di atas cukup mudah untuk dipahami, kan? Namun, program seperti di atas tentu tidak begitu bermanfaat selain hanya untuk kebutuhan belajar pemrograman. Nyatanya kode program tersebut tidak menyelesaikan masalah apapun. Tentunya bukan itu tujuan sebenarnya kita membuat program.

## Tujuan Membuat Program

Seharusnya, ketika kita membuat program, ada tujuan tertentu yang harus tercapai, atau ada permasalahan yang dapat diselesaikan dengan program tersebut. Misalnya:
1. Mencari mahasiswa yang berprestasi
2. Mencari langkah penyelesaian labirin
3. Mencari jalur terpendek dari dan menuju ke suatu tempat
4. Memprediksi langkah permainan catur
5. Menyusun puzzle
6. dsb

## Data Yang Berstruktur

Ketika kita ingin mencari sebuah data di dalam kumpulan data yang banyak, tentu kita membutuhkan sebuah kumpulan data-data yang menyimpan berbagai data yang ingin dicari. Misalnya data mahasiswa di sekolah. 

![Kumpulan nama-nama Mahasiswa](image20230910113040.png)

Anggap saja kita ingin mencari mahasiswa yang berprestasi di sekolah. Tentu kita butuh lebih dari sekedar nama mahasiswa. Kita butuh nilai Matematika, nilai Bahasa Inggris dan nilai lainnya sebagai bahan pertimbangan untuk memilih mahasiswa berprestasi. Belum lagi data NIM, alamat, nomorHP dan jurusan mahasiswa.

![](image20230910113530.png)

Sehingga membuat program yang menyimpan banyak data mahasiswa tidak dapat dilakukan hanya dengan mengandalkan variabel `String` saja. Tetapi perlu Tipe Data lain yang lebih kompleks dan lebih terstruktur. Perhatikan contoh Class berikut:

```java
public class Mahasiswa {
	String nama;
	String nim;
	String alamat;
	String jurusan;
	String nomorHp;
	double nilaiMtk;
	double nilaiEng;
	double nilaiKom;
	double nilaiTim;
	//...
}
```

Class `Mahasiswa` di atas merupakan Tipe Data Referensi yang dirancang untuk menyimpan berbagai data mahasiswa yang dibutuhkan untuk menghitung prestasi. Inilah yang disebut dengan Data Berstruktur. 

Ada banyak sekali data-data yang harus dibuat berstruktur seperti data pada class `Mahasiswa` di atas. Misalnya: data barang di supermarket, data kendaraan, data lokasi, data penduduk, dan sebagainya.

## Koleksi Data Array

Ketika Data Berstruktur dari disimpan menjadi kumpulan data-data dalam bentuk koleksi, maka Array adalah salah satu Tipe Data yang dapat digunakan untuk menyimpan semua jenis Tipe Data Berstruktur. Dengan Array, kita dapat menyimpan semua data Mahasiswa ke dalam sebuah variabel atau objek, sehingga memudahkan dalam proses pencarian dan proses lainnya.

Berikut adalah ilustrasi sebuah koleksi data yang berisi kumpulan data Mahasiswa yang berstruktur. 

![](image20230910114711.png)

Setiap data Mahasiswa memiliki struktur data yang sama, yang terdiri dari: (1) nama; (2) nim; (3) jurusan; (4) alamat; dan (5) nomorHp. 

Sehingga dengan demikian akan memungkinkan untuk melakukan proses pencarian data Mahasiswa berdasarkan kriteria tertentu. Misalkan proses mencari mahasiswa yang beralamat di "jalan Sudirman" atau mahasiswa "jurusan Teknik Informatika".

## Struktur Data Berelasi

Ada kalanya setiap data dengan data lainnya memiliki relasi yang cukup kompleks dari sekedar kumpulan data pada Array. Bayangkan jika ada permasalahan di dalam pemrograman yang membutuhkan kumpulan data yang saling berelasi dengan cara yang berbeda. Misalnya adalah hubungan pertemanan Mahasiswa di dalam kelas seperti ilustrasi berikut.

![](image20230910115701.png)

Dari ilustrasi di atas ada beberapa Mahasiswa yang saling berteman satu dengan yang lain, namun ada juga Mahasiswa yang hanya berteman dengan satu orang Mahasiswa lainnya. Struktur Data seperti ini memungkinkan kita melakukan proses pencarian Mahasiswa yang paling berpengaruh dan yang tidak.

Selain itu, permasalahan dalam mencari rute terpendek juga merupakan permasalahan yang membutuhkan struktur data tertentu untuk diselesaikan. Tanpa struktur data tersebut, akan sangat sulit sekali untuk diselesaikan menggunakan pemrograman.

![](image20230910120935.png)

Itulah alasannya mengapa kita perlu Struktur Data yang sesuai dengan kebutuhan. Untuk contoh di atas kita dapat menggunakan Tree atau Graph untuk menghasilkan data dengan Struktur Data berelasi seperti di atas. Pembahasan lebih rinci tentang Tree dan Graph dipisahkan pada pembahasan tersendiri.

## Manfaat Struktur Data

Dari penjelasan di atas dapat disimpulkan beberapa manfaat Struktur Data dalam pemrograman, antara lain:
1. Memudahkan untuk menyelesaikan masalah pemrograman yang lebih kompleks, dan membutuhkan data dengan struktur tertentu.
2. Membantu memahami konsep penyelesaian masalah yang komplek.

Tentunya, selain manfaat-manfaat di atas, masing-masing Tipe Data Abstrak memiliki manfaatnya tersendiri. Misalnya Stack dapat digunakan untuk validasi sintaks pemrograman, atau menyelesaikan pencarian rute terpendek dari dan menuju ke suatu lokasi. Begitu juga Tree yang dapat digunakan untuk mencari jalan keluar dari sebuah labirin.

## Selanjutnya

Kita sudah mengetahui secara umum tentang Struktur Data dan berbagai Tipe Data Abstrak yang ada. Selanjutnya kita dapat memahami secara mendalam

