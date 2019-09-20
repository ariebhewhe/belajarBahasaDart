## Pengenalan Dart 
Dart adalah bahasa pemprograman yang diproduksi oleh Google, dirancang oleh Lars Bak dan Kasper Lund. dan diperkenalkan pada 10 oktober 2011. Dart digunakan untuk membuat aplikasi server(command line interface), web, maupun mobile (android dan ios). versi stabil adalah Dart 2.1 yang dirilis pada tanggal 15 november 2018. Dart akan dieksekusi secara langsung melalui Dart VM (virtual machine) tanpa adanya proses penerjemahan kode objek (bytecode) terlebih dahulu.
## Membuat dan menjalankan aplikasi Dart
- Buatlah direktori kerja. 
- Jalankan aplikasi pada Texteditor :
 <pre>
  void main() {
  print('Hello world!');
  }
 </pre>
- simpan file diatas dengan ekstensi .dart (misal hello.dart)
## Menjalankan aplikasi Dart 
- cd ~/kodedart
- dart hello.dart 
## Perintah program Dart
statement adalah instruksi yang nantinya akan dieksekusi oleh Dart VM, setiap instruksi diakhiri tanda titik koma(;)

## Blok Program dalam Program Dart 
Blok program adalah bagian kode yang berfungsi untuk mengelompokkkan beberapa perintah sebagai satu kesatuan. 
<pre> 
  if(a > 0 ) {
  print ('nilai a: $a');
  }
  int i = 0;
  while(i < a) {
  print('Baris $i);
    i++;
  }
</pre>
## Komentar Program Dart
- Komentar satu baris
   <pre> 
   // ini adalah contoh komentar 
   yang salah
   
   // ini komentar 
   //yang benar
   </pre>
- Komentar dua baris  atau lebih
  <pre> 
   /* 
    ini adalah contoh komen
    yang tediri dari
    tiga baris.
   */
  </pre>
- Komentar untuk dokumentasi
 <pre>
 //////////////////////////////////////
 /// program komentar
 /// author : ary budi warsito
 //////////////////////////////////////
 </pre>
## kata Kunci (keyword) dalam Dart 
untuk mengakses ini website : <a href="https://dart.dev/guides/language/language-tour#keywords">https://dart.dev/guides/language/language-tour#keywords </a>
