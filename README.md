# Catatan Keuangan V4 — Tahap 1

Paket pengembangan awal modul Dashboard, Rekening, Kategori, Transaksi, dan Neraca Kekayaan (saldo rekening).

## Catatan penting
- Data disimpan lokal di browser/perangkat melalui localStorage.
- Jangan unggah workbook Excel asli atau cadangan JSON yang berisi data pribadi ke repository publik.
- Impor Excel pada tahap ini membaca sheet Rekening, Kategori, dan Transaksi. Modul lanjutan dan rekonsiliasi penuh dengan seluruh rumus workbook masih dalam proses.
- Neraca tahap 1 baru menghitung saldo rekening; belum memasukkan investasi, aset tetap, tabungan, piutang, dan utang.
- Impor Excel menggunakan pustaka SheetJS dari CDN sehingga proses impor memerlukan koneksi internet.
- Sebelum mengganti aplikasi yang sedang dipakai, buat cadangan JSON terlebih dahulu.
