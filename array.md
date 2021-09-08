Array adalah kelompok variabel dengan tipe sejenis dan dinyatakan dengan nama
yang sama. Array merupakan tipe khusus untuk menyatukan sekelompok variabel
dengan tipe yang sama. Dalam Java, pada saat mendeklarasikan sebuah array
panjang array harus ditentukan, dan tidak dapat diubah setelahnya. Setiap item
dalam sebuah array disebut element, dan setiap element diakses dengan indexnya.
Index array dimulai dari 0 sampai n-1, dengan n adalah panjang array.

## Deklarasi
Sebelum digunakan, Array harus dideklarasikan terlebih dahulu dengan
menentukan tipe data dan panjangnya. Berikut ini cara mendeklarasikan sebuah
array dengan panjang n.

Bentuk umum:

```java
tipeData[] namaArray = new tipeData[n];
//atau
tipeData namaArray[] = new tipeData[n];
```

Contoh:

```java
int[] anArray = new int[5];
```

## Mengisi

Ada beberapa cara untuk menginisialisasi array, diantaranya adalah:

```java
tipeData[] namaArray = { element1, element2, element3, element4 };

atau 

tipeData[] namaArray = new int[4];
namaArray[0] = element1;
namaArray[1] = element2;
namaArray[2] = element3;
namaArray[3] = element4;
```

Contoh:

```java
int[] anArray = { 132, 11, 134, 33};

atau

int[] anArray = new int[4];
anArray[0] = 132;
anArray[1] = 11;
anArray[2] = 134;
anArray[3] = 33;
```

## Mengakses

Untuk mengakses element tertentu pada array cukup dengan menyebutkan nama array
disertai dengan kurung siku dan index element yang ingin diakses.

Bentuk umum:

```java
namaArray[index];
```

## Array multi-dimensi

Array multidimensi dapat diilustrasikan sebagai array dalam array. Artinya
setiap element pada array tersebut adalah sebuah array juga (Array dua dimensi).
Hal ini juga berlaku untuk Array N dimensi. 

Contoh:

```java
int[][] arrayDuaDimensi = new int[3][2];
```

Kemudian untuk mengisinya dengan:

```java
int[][] array = {
    {1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1},
    {1, 1, 1, 1, 1}
};
```