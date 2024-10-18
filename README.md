Penjelasan Proses Praktikum

Latihan 1

1. Penggunaan end

Pada bagian ini, end='' digunakan untuk menentukan apa yang akan dicetak setelah suatu print statement. Secara default, print() menambahkan baris baru setelah mencetak sesuatu. Namun, dengan menambahkan end='', kita menghilangkan baris baru tersebut dan menggantinya dengan karakter kosong sehingga semua output berada dalam satu baris.

print('A', end='')
print('B', end='')
print('C', end='')

Output:

ABC

Setelah itu, dua print() berikutnya tanpa end='' akan mencetak baris baru setelah setiap pernyataan:

print('X')
print('Y')
print('Z')

Output:

X
Y
Z

2. Penggunaan separator

Pada bagian ini, sep= digunakan untuk menentukan pemisah antar elemen yang dicetak dalam satu perintah print(). Secara default, sep=' ' (spasi), namun dapat diubah sesuai kebutuhan:

w, x, y, z = 10, 15, 20, 25
print(w, x, y, z)

Output:

10 15 20 25

print(w, x, y, z, sep=',')

Output:

10,15,20,25

print(w, x, y, z, sep='')

Output:

10152025

print(w, x, y, z, sep=':')

Output:

10:15:20:25

print(w, x, y, z, sep='-----')

Output:

10-----15-----20-----25

3. String format

Bagian ini menunjukkan dua cara menampilkan angka dengan format tertentu:

Tanpa format khusus, angka dan hasil pangkat ditampilkan secara biasa:


print(0, 10**0)
print(1, 10**1)

Output:

0 1
1 10

Dengan format {0:>3} {1:>16}, kita menyesuaikan lebar kolom:

{0:>3}: angka pertama akan diatur dalam lebar 3 karakter dengan rata kanan.

{1:>16}: hasil pangkat akan diatur dalam lebar 16 karakter dengan rata kanan.



print('{0:>3} {1:>16}'.format(0, 10**0))
print('{0:>3} {1:>16}'.format(1, 10**1))

Output:

0                1
  1               10


---


Latihan 2

1. Input Nilai

input() digunakan untuk mendapatkan input dari pengguna. Pada kode ini, pengguna diminta memasukkan dua nilai untuk variabel a dan b:


a=input("masukkan nilai a:")
b=input("masukkan nilai b:")

Misalnya, pengguna memasukkan 5 untuk a dan 10 untuk b.


2. Penggabungan String

Pada bagian ini, menggunakan .format() untuk mencetak penggabungan dua nilai a dan b. Namun, ada kesalahan dalam kode karena percobaan menggunakan % dan .format() secara bersamaan. Seharusnya, cukup memilih salah satu:


print("hasil penggabungan {1}&{0}={}".format(a, b, a+b))


3. Konversi Tipe Data

Sebelum melakukan operasi matematika, variabel a dan b yang awalnya bertipe string diubah menjadi tipe int agar bisa dilakukan operasi aritmetika:


a = int(a)
b = int(b)


4. Operasi Matematika

Penjumlahan dan pembagian dilakukan setelah konversi:


print("hasil penjumlahan {1}+{0}=%d".format(a, b) %(a + b))
print("hasil pembagian {1}/{0}=%d".format(a, b) %(a / b))

Namun, bagian ini juga memiliki kesalahan. Penggunaan .format() tidak kompatibel dengan %d. Seharusnya cukup menggunakan .format() seperti ini:

print("hasil penjumlahan {1}+{0}={}".format(a, b, a + b))
print("hasil pembagian {1}/{0}={}".format(a, b, a / b))


---


Latihan 3 (Bagian 1): Menentukan Bilangan Terbesar dari Tiga Buah Bilangan

1. Inisialisasi Input: Pengguna diminta untuk memasukkan tiga buah bilangan, yaitu bil1, bil2, dan bil3.

2. Pemeriksaan Bilangan Terbesar:
Program memeriksa apakah bilangan pertama (bil1) lebih besar dari bilangan kedua (bil2) dan bilangan ketiga (bil3). Jika benar, bilangan pertama adalah yang terbesar.
Jika kondisi pertama tidak terpenuhi, program kemudian memeriksa apakah bilangan kedua (bil2) lebih besar dari bilangan ketiga (bil3). Jika benar, bilangan kedua adalah yang terbesar.
Jika kedua kondisi sebelumnya tidak terpenuhi, bilangan ketiga (bil3) adalah yang terbesar.


3. Menampilkan Hasil: Program menampilkan bilangan terbesar di antara tiga bilangan yang diinputkan.



Flowchart Proses Bagian 1:

1. Mulai
2. Input bil1, bil2, bil3
3. Apakah bil1 > bil2 dan bil1 > bil3? Jika ya, bilangan terbesar = bil1, jika tidak lanjut ke langkah berikutnya.
4. Apakah bil2 > bil3? Jika ya, bilangan terbesar = bil2, jika tidak bilangan terbesar = bil3.
5. Cetak bilangan terbesar
6. Selesai


---

Latihan 3 (Bagian 2): Menentukan Bilangan Terbesar dari N Buah Bilangan

1. Inisialisasi Variabel: Sebuah variabel boo diinisialisasi dengan nilai None untuk menyimpan bilangan terbesar yang ditemukan sejauh ini.

2. Looping Input Bilangan:
Program akan terus meminta input bilangan dari pengguna dengan loop tanpa henti (infinite loop).
Jika pengguna memasukkan angka 0, loop berhenti, dan program lanjut ke proses berikutnya.
Setiap kali pengguna memasukkan bilangan baru, program memeriksa apakah bilangan tersebut lebih besar dari boo. Jika ya, nilai boo diperbarui dengan bilangan yang lebih besar tersebut.

3. Menampilkan Bilangan Terbesar: Setelah loop berhenti (karena input 0), program menampilkan bilangan terbesar yang telah disimpan di variabel boo.



Flowchart Proses Bagian 2:

1. Mulai
2. Inisialisasi variabel boo = None
3. Input bilangan noo
4. Apakah noo == 0? Jika ya, lanjut ke langkah 8, jika tidak lanjut ke langkah berikutnya.
5. Apakah boo None atau noo > boo? Jika ya, update boo = noo
6. Kembali ke langkah 3
7. Jika ya pada langkah 4, cetak bilangan terbesar (boo)
8. Selesai
