Penjelasan Proses Praktikum

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
