Pertemuan 04 - Seleksi Multi-Kondisi dan Validasi Input

Nama: Euis Hasanah Ramadani
NIM: 2225250193
Kelas: 3F

Tujuan

Membangun program validasi dan klasifikasi menggunakan struktur "if-elif-else", serta menerapkan validasi tipe dan rentang nilai.

Struktur Folder

pertemuan-04-validasi-NIM/
├── README.md
├── .gitignore
├── latihan/
│   ├── 01_predikat_nilai.py
│   ├── 02_kategori_bilangan.py
│   ├── 03_validasi_rentang.py
│   ├── 04_validasi_tipe.py
│   └── 05_klasifikasi_segitiga_sudut.py
└── praktik/
    └── validasi_klasifikasi_nilai.py

Cara Menjalankan

Untuk menjalankan Praktik 1:

python3 praktik/validasi_klasifikasi_nilai.py

Tabel Keputusan

Kondisi| Keputusan
Data bukan angka| Input ditolak
Nilai di luar 0-100| Input ditolak
Kehadiran kurang dari 80%| Tidak memenuhi syarat kehadiran
Nilai akhir >= 85| Predikat A, Lulus
Nilai akhir >= 70| Predikat B, Lulus
Nilai akhir >= 60| Predikat C, Lulus
Nilai akhir >= 50| Predikat D, Belum lulus
Nilai akhir < 50| Predikat E, Belum lulus

Rumus Nilai Akhir

Nilai akhir dihitung menggunakan rumus:

Nilai akhir = 0.6 × nilai ujian + 0.4 × nilai tugas

Hasil Pengujian

Ujian| Tugas| Kehadiran| Hasil
90| 80| 95| 86.00, A, Lulus
75| 70| 85| 73.00, B, Lulus
60| 60| 80| 60.00, C, Lulus
55| 50| 90| 53.00, D, Belum lulus
40| 30| 100| 36.00, E, Belum lulus
90| 90| 75| Tidak memenuhi syarat kehadiran
105| 80| 90| Penolakan nilai ujian
80| -5| 90| Penolakan nilai tugas
80| 80| abc| Penolakan tipe

Refleksi

Salah satu masukan yang perlu diperhatikan adalah masukan berupa teks seperti "abc". Masukan tersebut tidak dapat dikonversi menjadi "float", sehingga program menggunakan "try-except ValueError" untuk menolak input dengan pesan yang sesuai. Selain itu, nilai di luar rentang 0 sampai 100 juga harus ditolak sebelum proses klasifikasi dilakukan.

Kesimpulan

Pada pertemuan ini dibuat program menggunakan "if-elif-else" untuk melakukan seleksi multi-kondisi. Program juga menerapkan validasi tipe dan rentang sebelum melakukan perhitungan dan klasifikasi. Pengujian dilakukan menggunakan beberapa nilai biasa, nilai batas, dan masukan yang tidak valid.