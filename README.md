# Algoritma Genetika (*Genetic Algorithm*)
## Pengertian Algoritma Genetika
**Algoritma Genetika** adalah teknik pencarian yang di dalam ilmu komputer untuk menemukan penyelesaian perkiraan untuk optimisasi dan masalah pencarian. Algoritma genetika adalah kelas khusus dari algoritma evolusioner dengan menggunakan teknik yang terinspirasi oleh biologi evolusioner seperti warisan, mutasi, seleksi alam dan rekombinasi (atau *crossover*).

Algoritma Genetika pertama kali dikembangkan oleh **John Holland** pada tahun 1970-an di New York, Amerika Serikat. Dia beserta murid-murid dan teman kerjanya menghasilkan buku berjudul "*Adaption in Natural and Artificial Systems*" pada tahun 1975.

Algoritma Genetika khususnya diterapkan sebagai simulasi komputer di mana sebuah populasi representasi abstrak (disebut kromosom) dari solusi-solusi calon (disebut individual) pada sebuah masalah optimisasi akan berkembang menjadi solusi-solusi yang lebih baik. Secara tradisional, solusi-solusi dilambangkan dalam biner sebagai *string* '0' dan '1', walaupun dimungkinkan juga penggunaan penyandian (*encoding*) yang berbeda. Evolusi dimulai dari sebuah populasi individual acak yang lengkap dan terjadi dalam generasi-generasi. Dalam tiap generasi, kemampuan keseluruhan populasi dievaluasi, kemudian multiple individuals dipilih dari populasi sekarang (*current*) tersebut secara stochastic (berdasarkan kemampuan mereka), lalu dimodifikasi (melalui mutasi atau rekombinasi) menjadi bentuk populasi baru yang menjadi populasi sekarang (*current*) pada iterasi berikutnya dari algoritma.

**Sumber**: https://id.wikipedia.org/wiki/Algoritme_genetik

## Prosedur Algoritma Genetika
Secara sederhana, algoritma umum dari algoritma genetika ini dapat dirumuskan menjadi beberapa langkah, yaitu:
1.  **Membentuk suatu populasi** individual dengan keadaan acak
2.  **Mengevaluasi kecocokan** setiap individual keadaan dengan hasil yang diinginkan
3.  **Memilih individual** dengan kecocokan yang tertinggi
4.  Bereproduksi, **mengadakan persilangan** antar individual terpilih diselingi mutasi
5.  Mengulangi langkah 2-4 sampai ditemukan individual dengan hasil yang diinginkan

Dalam *code* ini, digunakan prosedur algoritma genetika sebagai berikut:
1.  Membentuk **Kromosom** yang mempresentasikan solusi dari permaslahan yang dibahas.
2.  Mendefinisikan **Fungsi Fitness** yang digunakan untuk menentukan baik atau buruknya suatu kromosom.
3.  Membentuk **Populasi Awal (pop)** yang terdiri dari *n* kromosom.
4.  Menentukan peluang ***crossover* (popc)**, **peluang mutasi (popm)**, dan **maksimum generasi (N)**.
5.  Melakukan **Seleksi** untuk memilih 2 kromosom dari populasi.
6.  Membentuk kromosom baru dengan melakukan **Crossover** pada kromosom yang terpilih dari seleksi.
7.  Lakukan **Mutasi** pada kromosom baru.
8.  Ulangi langkah 5-7 sebanyak *n* kali (sesuai jumlah kromosom).
9.  **Gabungkan** semua kromosom (populasi awal, hasil *crossover*, dan hasil mutasi) yang ada dan pilih *n* kromosom terbaik (berdasarkan *fitness*) sebagai Populasi Baru.
10. Ulangi langkah 5-9 sebanyak N kali (maksimum generasi).

## Contoh Penerapan Algoritma Genetika
Salah satu contoh penerapan algoritma genetika adalah ***Traveling Salesman Problem***. Berikut adalah contoh *coding*nya:
1. https://github.com/thaliahfauza/algoritmagenetika/blob/main/GeneticAlgorithmTSP1_Thaliah_Fauz_Ardamayanti_06111840000034.ipynb
2. https://github.com/thaliahfauza/algoritmagenetika/blob/main/GeneticAlgorithmTSP2_Thaliah_Fauz_Ardamayanti_06111840000034.ipynb

## Penjelasan Files
1. File GeneticAlgorithmTSP1_Thaliah Fauz Ardamayanti_06111840000034.ipynb : Algoritma genetika menggunakan Python untuk kasus TSP.
2. File GeneticAlgorithmTSP2_Thaliah Fauz Ardamayanti_06111840000034.ipynb : Algoritma genetika menggunakan Python untuk kasus TSP (Harder Case).
