# Audit struktur workbook NEW CKP V4

File sumber tidak disertakan dalam paket aplikasi karena dapat berisi data keuangan pribadi. Audit ini hanya memuat nama sheet, ukuran, jumlah sel terisi, dan jumlah rumus.

| Sheet | Ukuran maksimum | Sel terisi | Rumus |
|---|---:|---:|---:|
| Cara Pakai | 41 × 3 | 70 | 0 |
| Dashboard | 84 × 5 | 245 | 136 |
| Neraca Kekayaan | 144 × 3 | 318 | 257 |
| Rekening | 24 × 17 | 257 | 166 |
| Kategori | 37 × 3 | 106 | 0 |
| Anggaran | 45 × 6 | 208 | 159 |
| Transaksi | 5061 × 13 | 29,103 | 25,245 |
| Lembar1 | 1 × 1 | 0 | 0 |
| Utang Saya | 328 × 22 | 1,715 | 1,238 |
| Piutang Saya | 215 × 13 | 1,083 | 819 |
| Filter Pencarian | 5066 × 13 | 55,579 | 55,547 |
| Riwayat Kekayaan Bersih | 49 × 13 | 217 | 195 |
| Tabungan | 240 × 23 | 817 | 720 |
| Anggaran Bulanan | 344 × 16 | 4,254 | 341 |
| Investasi | 192 × 12 | 786 | 579 |
| Aset Tetap | 37 × 14 | 137 | 90 |
| Asuransi | 225 × 12 | 443 | 340 |
| Cek Data | 18 × 4 | 56 | 25 |

## Status porting

- Workbook memiliki 18 sheet.
- Formula Excel belum otomatis berjalan di browser hanya karena file diimpor; aturan perhitungan perlu dipindahkan dan diuji di JavaScript.
- Sheet `Transaksi` memiliki formula hingga baris 5.050, dan sheet `Filter Pencarian` juga memuat formula turunan.
- Tahap awal aplikasi hanya mengimpor sebagian struktur (rekening, kategori, transaksi, anggaran bulanan). Ini belum memenuhi kesetaraan seluruh workbook.
- Modul yang harus dipetakan dan diuji meliputi Dashboard, Neraca Kekayaan, Rekening, Kategori, Anggaran, Transaksi, Utang Saya, Piutang Saya, Filter Pencarian, Riwayat Kekayaan Bersih, Tabungan, Anggaran Bulanan, Investasi, Aset Tetap, Asuransi, dan Cek Data.