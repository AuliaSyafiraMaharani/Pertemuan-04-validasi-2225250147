# Pertemuan 04 Seleksi Multi-Kondisi dan Validasi Input

Nama: Aulia Syafira Maharani
NIM: 2225250147
Kelas: 3A

## Tujuan

Membangun program validasi dan klasifikasi dengan rantai if-elif-else.

## Cara Menjalankan

Jalankan program menggunakan Python:

python latihan/01_predikat_nilai.py
python latihan/02_kategori_bilangan.py
python latihan/03_validasi_rentang.py
python latihan/04_validasi_tipe.py
python latihan/05_klasifikasi_segitiga_sudut.py
python praktik/validasi_klasifikasi_nilai.py

## Tabel Keputusan

| Kategori | Syarat | Contoh Masukan | Keluaran |
|---|---|---|---|
| A | Nilai >= 85 | 92 | A |
| B | Nilai >= 70 | 75 | B |
| C | Nilai >= 60 | 65 | C |
| D | Nilai >= 50 | 55 | D |
| E | Selain kondisi di atas | 40 | E |

## Hasil Pengujian

| Masukan | Keluaran Diharapkan | Keluaran Aktual | Status |
|---|---|---|---|
| 92 | Predikat A | Predikat A | Sesuai |
| 85 | Predikat A | Predikat A | Sesuai |
| 84.9 | Predikat B | Predikat B | Sesuai |
| 70 | Predikat B | Predikat B | Sesuai |
| 60 | Predikat C | Predikat C | Sesuai |
| 50 | Predikat D | Predikat D | Sesuai |
| 49.9 | Predikat E | Predikat E | Sesuai |
| -1 | Penolakan rentang | Penolakan rentang | Sesuai |
| abc | Penolakan tipe | Penolakan tipe | Sesuai |

## Refleksi

Salah satu masukan tidak valid yang dapat terlewat adalah masukan berupa teks seperti "abc". Masukan tersebut tidak dapat langsung dikonversi menjadi angka dengan float(). Oleh karena itu, digunakan try-except ValueError agar program dapat menampilkan pesan penolakan tanpa berhenti secara tiba-tiba.