Semoga bisa membantu teman-teman semua juga :D

### FAQ

<details> <summary>click here to expand FAQ</summary>


- 7zip exception: The system cannot find the file specified

  Hal ini diduga disebabkan karena ada masalah permission untuk mendownload file `.7z`-nya ataupun masalah permission untuk memodifikasi folder tersebut. Salah satu cara yang pernah berhasil adalah men-download dan meng-extract TBHGrader pada direktori `C:\Users\<user name>\Downloads`. Cara lainnya adalah dengan mencoba menjalankan TBHGrader dengan *administrator privilege*

- java --version, javac --version, dan JNI error

  Hal ini biasanya disebabkan karena versi java yang sudah terinstall di laptop teman-teman perlu diupdate. Bisa juga karena ada miskonfigurasi pada instalasi JDK teman-teman. Solusinya bisa lihat [java --version error.md](java --version error.md)

- IOException

  Teman-teman coba periksa kembali apakah ada `final` pada variabel IO (seperti `in` atau `out` misalnya). Jika ada, teman-teman bisa menghapus keyword final pada variabel tersebut.

- Mengubah batas waktu TLE

  Untuk mengubah batas waktu TLE, teman-teman bisa mengubah isi file `.configurations\time_limit_in_ms.txt` dengan suatu bilangan bulat. Pastikan file hanya terdiri atas **1 baris**, dan **tidak ada karakter spasi maupun newline** di dalamnya.

- Output program berbeda dengan output pada VSCode/Intellij

  Jika hal ini terjadi, coba inisiasikan semua static variable pada awal-awal fungsi main(). Misal jika kita punya:  `public static int my_variable = 3;`, maka tambahkan: 

  ```java
  public static void main(String[] args) {
  	my_variable = 3;
  	// kode anda
  }
  ```

- Stuck di "parsing and wrapping your copied ..."  (solved in v1.3)

  Biasanya ini karena TBHGrader tidak bisa membaca/menulis ke folder `TBHGrader/bin/`. Merestart laptop atau kill process `java.exe` dan `javaw.exe` biasanya menjadi solusi umum. Pastikan juga tidak ada dua/lebih window TBHGrader yang terbuka secara bersamaan.

- Membuka file log.txt

  File log.txt dapat dibuka dengan cara klik kanan pada tulisan/logo TBHGrader (di pojok kiri atas)



</details>





