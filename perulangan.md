Perulangan (Looping) adalah suatu blok kode yang akan terus berjalan selama
syarat yang diberikan masih memenuhi.

Setiap perulangan memiliki empat bagian, yaitu `inisialisasi`, `body`,
`iterasi`, dan `terminasi/kondisi`.

1.  Inisialisasi adalah statement yang menyatakan keadaan awal sebuah
    perulangan.
2.  Body atau badan program adalah blok statement yang akan dijalankan terus
    menerus selama perulangan berlangsung.
3.  Iterasi adalah statement atau bagian program yang nilainya terus berubah
    (ascending, descending atau cara lainnya) untuk mencapai batas atau keadaan
    untuk berhenti.
4.  Terminasi atau kondisi adalah statement bernilai Boolean yang menyatakan
    batas atau keadaan untuk menghentikan perulangan.

Pada Java dikenal tiga macam bentuk perulangan, yaitu: `while`, `do-while`, dan
`for`.

Pada dasarnya semua perulangan dalam Java memiliki cara kerja yang sama
yaitu selama kondisi masih bernilai true maka perulangan akan terus dilakukan
hinggi kondisi bernilai false.

## For

For adalah perulangan yang banyaknya perulangan diketahui atau banyaknya
perulangan sudah jelas(tentu).

Bentuk umum:

```java
for (inisialisasi; kondisi; iterasi) {
    //body
}
```

Contoh:

```java
int n = 99;

for (int i=0; i<n; i++) {
    System.out.println(i);
}
```

## While

While adalah perulangan yang banyaknya perulangan tidak menentu dan lebih
sederhana dari pada perulangan for.

Bentuk umum:

```java
Inisialisasi;

while (kondisi) {
    //body
    Iterasi; //opsional
}
```

Contoh:

```java
int n = 19;
int i = 0;

while (i<n) {
    System.out.println(i);
    i++;
}
```

## Do-while

Pada perulangan ini bagian body (semua dalam kurung kurawal setelah "do")
dijalankan terlebih dahulu sebelum pengecekan kondisi.

Sehingga walaupun kondisi dari awal bernilai false, bagian body tetap dijalankan
sekali. Berbeda dengan perulangan while apabila kondisi diawal bernilai false
maka bagian body tidak akan dijalankan.

Bentuk umum:

```java
Inisialisasi;

do {
    //body
    Iterasi; //opsional
} while (kondisi);

```

Contoh:

```java
int n = 19;
int i = 0;

do {
    i++;
} while (i<n)

System.out.println(i);
```