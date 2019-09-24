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

## Pengenal (identifier)
Aturan didalam variabel dart : 
- Nama tidak boleh menggunakan spasi.
- Nama pengenal tidak bileh menggunakan simbol, kecuali underscore ( _ ) dan dollar ($)
- Nama pengenal harus unik. 
- Nama Pengenal bersifat case-sensitive
## Dalam Dart, Semuanya adalah objek
Di dalam dart semua elemen kode dinyatakan sebagai objek. Misal 23 adalah objek dari kelas int, 23.4 adalah objek double dan 'Bahasa dart' objek dari String. Fungsi didalam dart juga sebagai objek. contoh sebagai berikut : 
<pre>
void ini_fungsi() {
// .....
}

void main() {
  print( ini_fungsi is Function) ; // Tampil true.
}
</pre>
Jadi seluruh kelas yang terdapat didalam dart adalah bagian dari turunan Object baik secara langsung atau tidak. 
## Identitas Objek 
identitas objek adalah sebuah identitas yang digunakan untuk menyimpan Nilai didalam memori komputer. Pengaksesan objek tersebut dilakukan melalui varibel. pada dart identitas objek dapat diambil dengan propert <b>hashCode</b> yang didefinisikan didalam kelas Object.
<pre> 
 void main() {
  int x = 1234;
  int y = 1234;
  double a = 123.456;
  String c = 'Bhs Dart';
  print ('a.hashCode:' + a.hashCode.toString());
  print ('c.hashCode:' + c.hashCode.toString());
  print ('x.hashCode:' + x.hashCode.toString());
  print ('y.hashCode:' + y.hashCode.toString());
  //cek identitas 
  print ('identitas(x,y):' + identical(a,b).toString());
 }
</pre>
seluruh nilai properti hashCode berupa bilangan bulat. sehingga untuk menyambung dengan string kita perlu <b> toString </b>
kode ditas nilai x dan y bernilai sama setelah dilakukan pemeriksaan identical.
