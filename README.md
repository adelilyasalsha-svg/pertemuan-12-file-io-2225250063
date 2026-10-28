# Pertemuan 12 - File I/O dan Error Handling

**Nama:** Adelilya Salsha  
**NIM:** 2225250063  
**Kelas:** 3B

## Tujuan
Mempelajari cara membaca, menulis, memproses, dan memvalidasi data menggunakan file Python serta menangani error dasar.

## Struktur Proyek
- `latihan/`: enam latihan file I/O dan error handling.
- `data/`: file catatan, data nilai, dan hasil rekap.
- `tugas/`: program rekap nilai dari file.

## Format File Input
Data pada `data/nilai.txt` menggunakan format `NIM,nilai`, satu data per baris.

Contoh:
```text
A001,85
A002,78
A003,92
```

## Cara Menjalankan
```powershell
python tugas/rekap_nilai_file.py
```

## Error yang Ditangani
- `FileNotFoundError`: file input tidak ditemukan.
- `ValueError`: format baris salah atau nilai tidak dapat dikonversi menjadi angka.

## Test Case

Pengujian dilakukan untuk memastikan program dapat membaca file, memproses data nilai, dan menangani kesalahan dengan baik.

| No. | Skenario Pengujian | Data/Kondisi | Hasil yang Diharapkan |
|---|---|---|---|
| 1 | Membaca data valid | `A001,85` | NIM dan nilai berhasil dibaca. |
| 2 | Memproses nilai bukan angka | `A004,abc` | Baris dilewati dan pesan data tidak valid ditampilkan. |
| 3 | Menangani baris kosong | Baris tanpa isi | Baris dilewati tanpa menghentikan program. |
| 4 | Menangani file tidak ditemukan | File `data/nilai.txt` tidak tersedia | Pesan `File tidak ditemukan` ditampilkan. |
| 5 | Menghitung statistik nilai | Terdapat lima data nilai valid | Jumlah data, rata-rata, nilai minimum, dan maksimum dihitung. |
| 6 | Menghitung jumlah mahasiswa lulus | Nilai minimal 60 | Mahasiswa dengan nilai ≥ 60 dihitung lulus. |
| 7 | Menulis hasil rekap | Data nilai berhasil diproses | Hasil rekap disimpan ke `data/hasil_rekap.txt`. |

### Hasil Pengujian
Berdasarkan data contoh pada `data/nilai.txt`, program berhasil memproses lima data valid. Baris `A004,abc` dilewati karena nilai bukan angka. Hasil rekap menunjukkan rata-rata **83,40**, nilai minimum **74**, nilai maksimum **92**, dan jumlah mahasiswa lulus **5 orang**.

Pengujian menunjukkan bahwa program dapat memproses data nilai serta menangani kesalahan format data dan file yang tidak ditemukan.

## Refleksi
Saya mempelajari perbedaan mode `r`, `w`, dan `a`, serta penggunaan `try-except` untuk menangani kesalahan saat membaca dan memproses data.

