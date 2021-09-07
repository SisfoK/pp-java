## Struktur program

Struktur dasar sebuah bahasa pemrograman Java adalah sebagai berikut:

```java
class Main{
    public static void main(String args[]){

    }
}
```

```java 
class Main
```

adalah class utama, nama `Main` harus sesuai dengan nama file. Aturan penulisannya
adalah dengan menggunakan huruf kapital di huruf pertama. Misalnya: `Main`, `Utama`,
dsb-nya.

```java
public static void main(String args[])
```

adalah kode utama yang akan dijalankan ketika kita menjalankan sebuah program Java.

## Menjalankan program

Java adalah bahasa yang dicompile terlebih dahulu sebelum dirun.

Untuk meng-compile java:

```bash
javac NamaFile.java
```

dan kemudian akan menghasilkan sebuah file dengan nama `NamaFile.class`.
File inilah yang kemudian dijalankan dengan menggunakan perintah:

```bash
java NamaFile
```
perhatikan, untuk menjalankan, tidak perlu menggunakan `NamaFile.class`, cukup dengan
menggunakan `NamaFile` saja.