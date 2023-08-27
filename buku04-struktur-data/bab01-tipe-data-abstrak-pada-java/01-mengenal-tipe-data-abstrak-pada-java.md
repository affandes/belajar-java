---
tags: java/struktur-data, tipe-data-abstrak-pada-java
keywords: 
video: 0
published: false
---
# Tipe Data Pada Java

Masih ingat dengan 3 jenis tipe data pada Java? Ada Tipe Data Primitif, Tipe Data Referensi dan Tipe Data Spesial.

```mermaid
flowchart LR
  root(Tipe Data di Java) --> a(Tipe Data Primitif);
  root --> b(Tipe Data Referensi);
  root --> c(Tipe Data Spesial);
  b --> ba[String];
  b --> bb["<b>Class</b>"];
  classDef pri fill:#eee;
  class ba,bb pri;
```

Tipe Data Primitif berisi int, long, double boolean dan sebagainya. Sedangkan Tipe Data Referensi diisi oleh String dan semua Class yang ada di Java. Tentunya setiap Class punya fungsi masing-masing, yang tidak dapat dibahas semua satu persatu. Terakhir adalah Tipe Data Spesial yang diisi oleh Array. Masing-masing dari ketiga tipe data tersebut memiliki ciri khas dan fungsi yang berbeda.

## Tipe Data Abstrak

Pada Java, Tipe Data Abstrak (Abstract Data Type / ADT) adalah Class yang 

> A set of data values and associated operations that are precisely specified independent of any particular implementation. - NIST

```mermaid
flowchart LR
  root(Tipe Data di Java) --> a(Tipe Data Primitif);
  root --> b(Tipe Data Referensi);
  root --> c(Tipe Data Spesial);
  b --> ba[String];
  b --> bb["<b>Stack</b>"];
  b --> bc["<b>Queue</b>"];
  b --> bd["<b>Linked List</b>"];
  b --> be["<b>Hash Table</b>"];
  b --> bf["<b>Tree</b>"];
  b --> bg["<b>Graph</b>"];
  classDef pri fill:#eee;
  class ba,bb,bc,bd,be,bf,bg pri;
```
