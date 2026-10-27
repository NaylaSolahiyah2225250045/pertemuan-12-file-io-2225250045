# Pertemuan 12 - File I/O dan Error Handling
Nama: Nayla Solahiyah
NIM: 2225250045
Kelas: 3A

## Tujuan
Membaca, memvalidasi, mengolah, dan menulis data file dengan Python.

## Format File Input
NIM,nilai

Contoh:
```text
A001,85
A002,78
A003,92
A004,abc
A005,74
A006,88
```

## Cara Menjalankan
```bash
python tugas/rekap_nilai_file.py
```

## Error yang Ditangani
- FileNotFoundError
- ValueError

## Test Case

| Kondisi | Hasil yang Diharapkan | Hasil Aktual | Status |
|---|---|---|---|
| Semua nilai valid | Data diproses dan rekap dibuat | Belum diuji | Belum diuji |
| Ada nilai tidak valid, seperti `A004,abc` | Baris tidak valid dilewati dan proses berlanjut | Baris 4 dilewati | Sesuai |
| File input tidak ditemukan | Pesan file tidak ditemukan ditampilkan | Belum diuji | Belum diuji |
| Ada baris kosong | Baris kosong dilewati | Belum diuji | Belum diuji |
| Menghitung rekap nilai | Jumlah data valid 5, rata-rata 83.40, minimum 74, maksimum 92, dan jumlah lulus 5 | Belum diuji | Belum diuji |

## Refleksi
Salah satu error yang ditemukan pada tugas ini adalah ValueError ketika nilai seperti `abc` diubah menjadi angka. Program menangani error tersebut menggunakan try-except, sehingga baris yang tidak valid dilewati dan data lainnya tetap diproses.