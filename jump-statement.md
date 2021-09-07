Java mengenal tiga buah perintah untuk memindahkan alur program ke bagian lain
dari program, yaitu break, continue dan return. Perintah ini biasa disebut __Jump
Statement__.

## Break

Break Statement merupakan perintah yang dapat digunakan untuk menghentikan
proses perulangan secara paksa. Berikut ini contoh penggunaan break dalam
perulangan while, program akan berhenti paksa ketika nilai i=9.

Contoh:

```java
int n = 11;
int i = 1;

while (i<n) {
    System.out.println(i);
    i++;
    
    if (i==9) {
        break;
    }
}
```

## Continue

Perintah continue adalah perintah yang dapat digunakan untuk meloncati proses
perulangan. Perintah continue berbeda dengan perintah break yang menghentikan
proses perulangan, namun perintah continue hanya akan meloncati proses
perulangan dan proses perulangan masih tetap berjalan.

Contoh:

```java
for (int i=0; i<13; i++) {
    if (i==5) {
        continue;
    }

    System.out.println(i);
}
```

Program di atas akan menampilkan bilangan mulai dari 0 sampai 12, tetapi angka 5
tidak akan ditampilkan karena ketika nilai i=5 maka perintah "continue" akan
dijalankan.

## Return

Perintah return adalah perintah dalam java yang digunakan di dalam method.
Method dipanggil oleh bagian lain dari program dan dengan perintah return, alur
eksekusi dikembalikan ke bagian dari program yang memanggil method tersebut.
Akan dibahas kemudian.