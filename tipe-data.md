Java merupakan bahasa pemrograman yang strongly typed, maka kita tidak bisa mengabaikan tipe data. Kita harus tahu data seperti apa yang disimpan ke dalam variabel. Selain itu, Java juga bersifat statically typed, yang artinya setiap variabel harus dideklarasikan terlebih dahulu sebelum digunakan <sup>[1](#1)</sup>.

## Tipe Data Primitif

### Integer

1. byte
    
    byte adalah tipe data yang menampung angka dengan range -127 - 128 (2^8).

    ```java
    byte n = 12;
    ```

2. short
    
    short adalah tipe data yang menampung angka dengan range -32.768 - 32.767
    (2^16).

    ```java
    short n = 1200;
    ```

3. int

    int adalah tipe data yang menampung angka dengan range 2^32.

    ```java
    int n = 289000;
    ```

4. long

    long adalah tipe data yang lebih panjang dari int, yaitu 2^64.

    ```java
    long n = 122334445;
    ```
### Floating point

Tipe data ini adalah tipe data bilangan desimal, misalnya 1.2, 3.4, 3.14, dst.

1. float

    Tipe data float adalah tipe data yang bisa nemapung nilai 2^32.

    ```java
    float n = 3.14f;
    ```
    penulisannya ditambahkan huruf `f` di belakang angkanya, ini untuk menandai
    bahwa bilangan tersebut adalah `float` bukan `double`.

2. double

    Tipe data double mirip dengan tipe data float, kecuali data yang bisa ditamp
    ungnya adalah 2^64.

    ```java
    double n = 144.2;
    ```
### Characters

Tipe data char adala tipe data yang hanya bisa menampung satu huruf saja.
Misalnya:

```java
char c = 'a';
```
Nilai yang diberikan disimpan dalam satu tanda kutip.

### Boolean

Boolean adalah tipe data yang bisa menampung dua nilai, yaitu benar atau salah.

Tipe data ini akan banyak digunakan kemudian.

```java
boolean b = true;
```

### String

String adalah tipe data yang menampung karakter. String bisa menampung lebih
dari satu karakter, misalnya kata, kalimat atau paragraf.

```java
String name = "Deo";
```

perhatikan, penulisan `String` menggunakan kapital di awal kata, kemudian isinya
disimpan di dalam tanda kutip dua ("...").

## Deklarasi variabel

Sebuah data dapat disimpan ke dalam variabel. Format penulisannya sebagai
berikut:

```java
type namaVariabel;
```
### Deklarasi

Deklarasi adalah pembuatan sebuah variabel, namun belum di isi dengan suatu
nilai. Contoh:

```java
int n;
boolean b;
char c;
```

### Inisiasi

Inisiasi adalah pengisian sebuah variabel dengan data. Contoh:

```java
n = 12;
b = false;
c = 'A';
```

Deklarasi sekaligus inisiasi juga dapat dilakukan, misalnya dengan:

```java
float f = 21.0f;
boolean b = false;
```

### Inisiasi dinamis

Dua atau lebih data dapat di isi secara bersamaan dalam satu baris dengan syarat
tipe datanya sama. Contoh:

```java
int a = 12, b = 13, c = 14;
```
atau bisa juga jika semua data memiliki nilai yang sama, misalnya:

```java
int x = y = z = 100;
```

## Mengubah tipe ke tipe data lain

Suatu tipe data dapat di ubah ke tipe data lain, misalnya dari byte ke int.
Syaratnya adalah:

-   kedua tipe data kompatible, misalnya antara byte dengan int, int dengan
    float, tetapi char dan boolean tidak memiliki kompatible.
-   tipe data yang dituju memiliki ruang penyimpanan yang lebih besar, misalnya
    byte memiliki ruang penyimpanan 2^8, akan diubah ke int yang memiliki
    penyimpanan 2^32. Tetapi jika dari tipe data int ke byte, maka jika nilai
    yang akan diubah lebih besar dari 2^8, maka akan menyebabkan nilai akhir
    adalah hasil modulo dari ukuran byte.

Cara mengubah tipe data dapat dicontohkan sebagai berikut:

```java
int n = 12;
byte b = (int) n;
```

Bagaimana jika int ke float, silahkan coba sendiri.

### Konversi otomatis

Misalnya terdapat a, b, c yang merupakan byte, kemudian dilakukan operasi sebagai
berikut:

```java
byte a = 40;
byte b = 50;
byte c = 100;
int d = a * b / c;
```

maka nilai a, b dan c akan otomatis diubah menjadi int.

Aturan promosi ini adalah:

1. byte, short, char akan di ubah ke int,
2. jika operasinya adalah long, maka akan diubah ke long,
3. float akan di ubah ke double,
4. jika operasi melibatkan double, maka otomatis akan diubah semua ke double.

<a name="1">1</a>: https://www.dicoding.com/academies/60/tutorials/1803?from=1797