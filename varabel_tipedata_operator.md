## Variabel di dalam dart
Variabel adalah nama yang digunakan untuk menyimpan nilai tertentu.  nilai didalam variabel dapat diubah sesuai kebutuhan dari aplikasi.
<pre> 
int a = 3; 
</pre>
cara untuk memanggilnya adalah : 
<pre> String s = a.toString(); </pre>

## Deklarasi Variabel 
Agar varibel dapat disimpan didalam memori komputer perlu dideklarasikan terlebih dahulu.

format : <i>tipe namaVariabel </i>

Contoh : 
<pre> 
 // program deklarasi variabel.
</pre>

## Inisialisasi Variabel 
Nilai yang akan disimpan didalam variabel tersebut.

format : <i> tipe namaVariabel = nilaiAwal; </i>

Contoh : 
<pre>
//program inisialisasi variabel  
</pre>

## Menggunakan kata kunci Var
Jika selama ini variabel sebelumnya hanya dapat diisi oleh tipe tertentu maka didalam bahasa dart ada variabel <b>bernilai dinamis</b>. maksudnya dinamis adalah dapat berupa bilangan bulat, rill maupun teks. untuk membuat variabel tipe ini kita perlu menggunakan kata kunci <b> var </b>

format : <i> var namaVariabel; </i>

Contoh : 
<pre>
void main () {
 // program variabel var 
 var a; 
 // int 
 a =1; 
 print('Nilai' + a.toString());
 print('Nilai' + a.runtimeTypetoString());
 // Double
 a =123.222; 
 print('Nilai' + a.toString());
 print('Nilai' + a.runtimeTypetoString());
 // bool 
 a =true; 
 print('Nilai' + a.toString());
 print('Nilai' + a.runtimeTypetoString());
 // string 
 a ='bhs Dart'; 
 print('Nilai' + a.toString());
 print('Nilai' + a.runtimeTypetoString());
 }
</pre>

## Menggunakan Tipe dynamic 
Dart akan menganggap  variabel menggunakan kata kunci var dengan tanpa proses inisialisasi nilai maka dart menganggap bertipe dynamic.

format : <i> dynamic namaVariabel; </i>

Contoh : 
<pre>
var a; 
print('a is dynamic'); // true
// atau 
dynamic a ;
print('a is dynamic'); // true
</pre>
Anda bisa menggunakan contoh tipe var diatas dengan mengubah variabel pada <i> "var a;"  ke "dynamic a;"</i>

## Variabel Global dan Variabel lokal
- Variabel global 
variabel global adalah variabel yang dideklarasikan diluar fungsi dan akan dikenal atau dapat diakses oleh semua fungsi yang ada.
<pre> 
import 'dart:io';
int globalVar = 20;

void updateGlobalVar(int val){
 globalVar = val;
}
void printG(){
 print(globalVar);
}
void main(){
 stdout.write('Sebelum diubah:');
 printG();
 updateGlobalVar(30);
 stdout.write('Setelah diubah');
 printG();
}
</pre>

- Variabel lokal
Variabel lokal adalah variabel yang dideklarikan di dalam fungsi.

<pre>
double div(double a, double b) {
 double c = a/b;
 return c;
}
int  intDiv(int a, int b){
 int c = a ~/ b;
 return c;
}
void main(){
 print (intDiv(10, 3).toString());
 print (Div(10.0, 3.0).toString());
}
</pre>


## Menampilkan data ke dalam layar
- Menggunakan Fungsi print() 

<pre>
print('Hello');
print ('World');
</pre>

- Menggunakan metode stdout.write()

<pre>
 stdout.write('hello);
 stdout.write('world');
</pre>

- Menggunakan Fungsi stdout.writeln()

<pre>
 stdout.writeln('hello);
 stdout.writeln('world');
</pre>

## Membaca data dari keyboard
Agar kita dapat membaca keyboard kita perlu menggunakan  <b> stdin.readLineSync() </b> 
<pre>
import 'dart:io";
voidn main(){
 int a; 
 String b ;
 
 stdout.write('Masukan bilangan bulat');
 a = int.parse(stdin.readLineSync());
 
 stdout.write('Masukan Teks');
 b = stdin.readLineSync();
 
 print('\n$a bertipe ${a.runtimeType.toString()}');
 print('\n$b bertipe ${b.runtimeType.toString()}');
}
</pre>

## Konstanta 
Konstanta adalah variabel yang tidak dapat diubah nilainya.
format : <i> cont namaKonstanta = nilai;  atau cont tipe namaKonstanta = nilai; </i>
Format : <i> final tipe namaVariabel;  </i>
<pre>
  final String Bhs ='Dart';
  print('$Bhs');
</pre>

## Tipe Data
- Tipe Bilangan 
tipe data yang dinyatakan dengan kelas int dan double dan merupakan turunan dari kelas num.
- Tipe int
Direpresentasikan bilangan bulat. contoh : 123, -1,13 dst.
- Tipe Double 
Tipe yang meresentasikan bilangan rill (bilangan yang mengandung angka dibelakang koma). Contoh : -1.1, 2.3,..dst
- Tipe Num 
tipe yang dapat diisi dengan bilangan bulat atau rill. contoh : num a = 13 atau num b = 13.4
- Tipe Teks 
Merupakan  nilai yang berupa teks atau kumpulan karakter.
<pre>
String s1 ='dart';
String s2 ="flutter";
String s3 = ''' tulisan lebih dari satu baris
baris ke 2 ''';
String s4 =""" ini baris ke 2
ini baris ke 3 """;
</pre>
- Tipe Logika 
Tipe yang dinyatakan dengan tipe bool. hanya di isi true dan false.
- Tipe list 
List adalah objek koleksi yang menyimpan daftar objek. 

- Tipe Map

link contoh untuk tipe list dan tipe map silakan <a href="https://gist.github.com/ariebhewhe/af72d10b552ceaa76e52c137e01cf836">klik disini</a>


## Operator 
- Operator penugasan : a = 3
- Operator Aritmetika : +,-,*,/,~/,%
- Operator Increment :++
- Operator Decrement  : --
- Operator Relasional :==,!=,>,<,<=
- Operator Logika :&&, || !
- Operator Bitwise 
