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
1. Data valid diproses dan direkap.
2. Baris `A004,abc` dilewati tanpa menghentikan seluruh program.
3. Baris kosong dilewati.
4. Nilai 60 atau lebih dihitung lulus.
5. File input yang tidak ditemukan ditangani dengan pesan yang jelas.

## Hasil Pengujian
Dengan data contoh, program memproses lima data valid, menghasilkan rata-rata 83,40, nilai minimum 74, nilai maksimum 92, dan lima mahasiswa lulus.

## Refleksi
Saya mempelajari perbedaan mode `r`, `w`, dan `a`, serta penggunaan `try-except` untuk menangani kesalahan saat membaca dan memproses data.

