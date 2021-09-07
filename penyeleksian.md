Peyeleksian adalah suatu pilihan atau opsi dengan kondisi tertentu. Jika kondisi yang menjadi syarat terpenuhi, maka semua statement dalam blok kondisi tersebut akan dijalankan, jika tidak maka semua stetement dalam blok itu dilewati dan tidak dijalankan. Dalam Java terdapat dua macam penyeksian kondisi yaitu “IF-Else” dan “Switch”.

## If-Else

Bentuk umumnya adalah:

```java
if ( Boolean_expression_1 ) {
    //statement yang akan dijalankan ketika Boolean_expression_1 = true
}
if else ( Boolean_expression_2 ) {
    //statement yang akan dijalankan ketika Boolean_expression_2 = true
}
else {
    //statement yang akan dijalankan ketika semua Boolean expression false
}
```

Aturannya:

Berikut ini hal yang harus diketahui ketika menggunakan “If-else”:

1. IF statement bisa tidak memiliki “Else” statement, “Else” statement harus terletak setelah semua “Else If” statement (jika ada).
2. IF statement bisa memiliki banyak “Else If” statement dan semuanya harus terletak sebelum “Else” statement.
3. Ketika salah satu “Else If” statement dijalankan, tidak ada “Else If” statement lainnya yang akan dijalankan.

Contoh:

```java
int value = 50;
if (value <= 50) {
    System.out.println("C");
} if else (value <= 85) {
    System.out.println("B");
} if else (value > 85) {
    System.out.println("A");
} else {
    System.out.println("Eror");
}
```

## Switch

Fungsi dari statement Switch ini tidak jauh berbeda dengan If-else. Pada “Switch” terdapat satu variable uji yang digunakan untuk menguji kesamaan terhadap daftar nilai yang ada. Setiap nilai (daftar nilai) ini disebut case, dan variable uji akan diperiksa untuk setiap case.

Bentuk umumnya:

```java
switch ( test_variable) {
    case value :
        //statement
        break;
    case value :
        //statement
        break;
    default :
        //statement
}
```

> default sama artinya dengan else di “If-else”

Contoh penggunaan:

```java
int a = 5;
switch (a) {
    case 1:
        System.out.println("You chose One");
        break;
    case 2:
        System.out.println("You chose Two");
        break;
    case 3:
        System.out.println("You chose Three");
        break;
    case 4:
        System.out.println("You chose Four");
        break;
    case 5:
        System.out.println("You chose Five");
        break;
    default:
        System.out.println("Invalid Choice");
}
```

