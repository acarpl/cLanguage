# cLanguage
Berikut adalah contoh modul ajar untuk Bahasa C yang mencakup sejarah, pengertian, syntax, dan tipe data:


---

Modul Ajar: Bahasa Pemrograman C

I. Pendahuluan

1.1. Sejarah Bahasa C

Bahasa pemrograman C dikembangkan oleh Dennis Ritchie di Bell Labs pada awal 1970-an. Awalnya, C digunakan untuk mengembangkan sistem operasi UNIX, dan hingga saat ini menjadi salah satu bahasa pemrograman yang paling populer dan banyak digunakan.

Timeline Perkembangan:

1960-an: Bahasa B dikembangkan oleh Ken Thompson, dasar dari bahasa C.

1972: Dennis Ritchie mengembangkan bahasa C.

1978: Terbitnya buku "The C Programming Language" oleh Brian Kernighan dan Dennis Ritchie yang menjadi referensi utama dalam pembelajaran C.

1989: ANSI (American National Standards Institute) meresmikan standar pertama bahasa C, dikenal dengan ANSI C atau C89.

1990: ISO merilis standar internasional bahasa C yang dikenal dengan ISO C atau C90.


Bahasa C sering disebut sebagai "mother language" karena banyak bahasa pemrograman modern yang terinspirasi dari C, seperti C++, C#, Java, dan lainnya.

1.2. Pengertian Bahasa C

Bahasa C adalah bahasa pemrograman prosedural yang dibuat untuk menulis sistem perangkat lunak dan aplikasi tingkat rendah, seperti sistem operasi dan driver perangkat keras. Bahasa ini dikenal dengan sintaksnya yang sederhana, kemampuan memanipulasi memori secara langsung, dan efisiensi komputasi.


---

II. Syntax Dasar dalam Bahasa C

2.1. Struktur Program Dasar C

Setiap program dalam bahasa C terdiri dari fungsi-fungsi. Fungsi utama adalah main(), yang menjadi titik awal eksekusi program. Berikut adalah contoh sederhana program C:

#include <stdio.h> // Library standar input/output

int main() {
    printf("Hello, World!\n"); // Fungsi untuk menampilkan teks
    return 0; // Mengembalikan nilai 0, menunjukkan program selesai tanpa error
}

2.2. Penjelasan Program

#include <stdio.h>: Baris ini menyertakan library standar input/output untuk memungkinkan penggunaan fungsi seperti printf.

int main(): Ini adalah fungsi utama dari program. Setiap program C harus memiliki fungsi main.

printf("Hello, World!\n"): Perintah ini akan mencetak teks "Hello, World!" ke layar.

return 0;: Mengembalikan nilai 0 untuk menunjukkan bahwa program telah selesai dijalankan dengan sukses.


2.3. Komentar dalam C

Komentar digunakan untuk menjelaskan kode dan tidak akan dieksekusi oleh program.

Komentar satu baris: Menggunakan //.

// Ini adalah komentar satu baris

Komentar multi baris: Menggunakan /* */.

/* Ini adalah komentar 
   multi baris */



---

III. Tipe Data dalam Bahasa C

Dalam C, tipe data digunakan untuk menentukan jenis nilai yang bisa disimpan dalam variabel. Beberapa tipe data dasar di C adalah:

3.1. Tipe Data Dasar

1. int: Tipe data untuk bilangan bulat (integer).

int a = 10;


2. float: Tipe data untuk bilangan desimal dengan presisi tunggal (single precision).

float b = 3.14;


3. double: Tipe data untuk bilangan desimal dengan presisi ganda (double precision).

double c = 3.1415926535;


4. char: Tipe data untuk karakter tunggal.

char d = 'A';



3.2. Tipe Data void

Tipe data void digunakan untuk fungsi yang tidak mengembalikan nilai atau tidak menerima argumen. Contoh:

void fungsiTanpaKembalian() {
    printf("Ini adalah fungsi void.\n");
}

3.3. Tipe Data bool

Di C, tipe data boolean (bool) merepresentasikan nilai true (benar) dan false (salah). Namun, pada standar awal bahasa C tidak ada tipe data bool, sehingga digunakan nilai int (0 = false, selain 0 = true). Di C99, bool bisa digunakan dengan library stdbool.h:

#include <stdbool.h>
bool isTrue = true;


---

IV. Operasi dan Struktur Kontrol

4.1. Operasi Aritmatika

C mendukung berbagai operasi aritmatika:

+ Penjumlahan

- Pengurangan

* Perkalian

/ Pembagian

% Modulus (sisa pembagian)


Contoh:

int x = 10;
int y = 5;
int z = x + y; // z akan bernilai 15

4.2. Struktur Kontrol

1. if - Kondisi jika.

if (x > y) {
    printf("x lebih besar dari y");
}


2. else - Kondisi selainnya.

if (x > y) {
    printf("x lebih besar");
} else {
    printf("y lebih besar");
}


3. for - Perulangan yang sudah ditentukan jumlah iterasinya.

for (int i = 0; i < 10; i++) {
    printf("%d\n", i);
}


4. while - Perulangan selama kondisi benar.

while (x < 10) {
    printf("%d\n", x);
    x++;
}




---

V. Latihan dan Tugas

1. Latihan 1: Buat program C yang menerima input dua angka dan menampilkan hasil penjumlahan, pengurangan, perkalian, dan pembagiannya.


2. Latihan 2: Buat program untuk menentukan bilangan genap atau ganjil dengan menggunakan struktur if-else.


3. Tugas Akhir: Buat program yang menghitung nilai faktorial dari suatu bilangan menggunakan perulangan for.




---

VI. Kesimpulan

Bahasa C adalah bahasa pemrograman yang kuat dan fleksibel. Dengan memahami dasar-dasarnya seperti tipe data, operasi, dan struktur kontrol, kita bisa membuat berbagai program yang efisien. Pemahaman terhadap C juga membuka jalan untuk mempelajari bahasa pemrograman lain yang lebih modern.


---

Referensi:

Kernighan, Brian W., and Dennis M. Ritchie. The C Programming Language. 2nd ed. Prentice Hall, 1988.

Harbison, Samuel P., and Guy L. Steele. C: A Reference Manual. 5th ed. Prentice Hall, 2002.



---

Modul ini bisa dijadikan dasar untuk pembelajaran bahasa C, terutama bagi pemula yang baru mulai belajar pemrograman.

Untuk meng-compile program C menjadi file .exe (aplikasi executable), Anda memerlukan beberapa perangkat lunak yang akan bertindak sebagai compiler dan IDE (Integrated Development Environment) untuk mempermudah proses pengembangan. Berikut adalah beberapa aplikasi yang umum digunakan:

1. GCC (GNU Compiler Collection)

GCC adalah salah satu compiler C yang paling populer dan open-source. Pada sistem Windows, Anda bisa menggunakan MinGW atau Cygwin untuk mendapatkan versi GCC yang bisa digunakan di lingkungan Windows.

MinGW (Minimalist GNU for Windows): menyediakan GCC untuk Windows.

Link: http://www.mingw.org

Install MinGW dan pastikan Anda menambahkan direktori MinGW ke dalam path sistem agar bisa diakses dari Command Prompt.


Cygwin: menyediakan lingkungan mirip Linux di dalam Windows, termasuk compiler GCC.

Link: https://www.cygwin.com



2. Microsoft Visual Studio (MSVC)

Microsoft Visual Studio menyediakan IDE yang kuat dan compiler C/C++ bawaan yang disebut MSVC (Microsoft Visual C++). Ini sangat cocok untuk mengembangkan aplikasi Windows.

Link: https://visualstudio.microsoft.com

Instal Visual Studio dan pilih workload "Desktop development with C++" selama proses instalasi untuk mendapatkan compiler MSVC.


3. Code::Blocks

Code::Blocks adalah IDE gratis yang terintegrasi dengan GCC atau MinGW. Ini sangat mudah digunakan bagi pemula dan kompatibel dengan berbagai sistem operasi seperti Windows, Linux, dan macOS.

Link: https://www.codeblocks.org

Saat menginstal, Anda bisa memilih paket instalasi yang sudah termasuk compiler MinGW.


4. Dev-C++

Dev-C++ adalah IDE open-source yang ringan dan dilengkapi dengan MinGW untuk compiler C/C++. Ini sangat mudah digunakan dan cocok untuk pengembangan sederhana di Windows.

Link: https://sourceforge.net/projects/orwelldevcpp/


5. CLion (JetBrains)

CLion adalah IDE premium untuk C/C++ yang dikembangkan oleh JetBrains. Ini mendukung berbagai compiler seperti GCC, Clang, dan MSVC, serta memiliki integrasi yang kuat dengan CMake dan banyak alat pengembangan lainnya.

Link: https://www.jetbrains.com/clion/

CLion membutuhkan instalasi compiler terpisah seperti GCC atau MSVC.


6. Eclipse IDE for C/C++ Developers

Eclipse adalah IDE open-source yang mendukung berbagai bahasa pemrograman termasuk C dan C++. Untuk menggunakannya, Anda perlu menginstal plugin CDT (C/C++ Development Tooling) dan compiler seperti GCC atau MinGW.

Link: https://www.eclipse.org



---

Langkah Umum untuk Meng-compile C ke .exe

1. Menulis Program: Buat program C di editor atau IDE pilihan Anda.


2. Kompilasi:

Jika menggunakan Command Prompt dengan GCC/MinGW:

gcc program.c -o program.exe

Ini akan menghasilkan file program.exe yang bisa dijalankan di Windows.

Jika menggunakan Microsoft Visual Studio: Anda dapat mengklik "Build" pada menu di IDE, dan Visual Studio akan menghasilkan file .exe secara otomatis.



3. Menjalankan Program: Setelah file .exe dihasilkan, Anda dapat menjalankannya di Windows dengan mengklik dua kali pada file tersebut atau melalui terminal (Command Prompt).



Dengan aplikasi-aplikasi ini, Anda dapat dengan mudah meng-compile kode C menjadi aplikasi executable di Windows.
