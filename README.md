# CKP V4 — fondasi aplikasi PWA

Paket tahap awal untuk mengembangkan CKP V4 menjadi aplikasi web yang dapat dipasang di Android (PWA).

## Isi paket
- `index.html` — fondasi UI dan fitur prototipe yang sudah ada, ditambah sound effect.
- `manifest.json` — metadata instalasi PWA.
- `service-worker.js` — cache dasar agar shell aplikasi dapat dibuka offline setelah pernah dimuat.
- `icon.svg` — ikon aplikasi.
- `WORKBOOK_AUDIT.md` — inventaris struktur workbook tanpa data pribadi.

## Sound effect
Menggunakan Web Audio API (nada sintetis pendek, tidak menggunakan musik panjang atau file audio eksternal). Efek yang disediakan: click, menu, success, income, expense, transfer, delete, backup, warning, error, dan pop. Pengaturan ON/OFF dan volume tersedia di menu **Lainnya**.

Browser Android biasanya baru mengizinkan audio setelah interaksi pengguna pertama. Karena itu, tekan tombol atau tombol **Tes sound effect** sekali untuk mengaktifkan audio.

## Keamanan data
- Jangan unggah workbook `NEW CKP V4.xlsx` asli ke repositori GitHub publik.
- Jangan masukkan backup JSON yang berisi rekening/transaksi pribadi ke repositori.
- Data prototipe disimpan lokal di browser perangkat. Hapus data browser dapat menghilangkannya; ekspor backup secara berkala.

## Batas tahap ini
Ini **belum merupakan porting penuh Excel V4**. Prototipe lama baru memiliki dashboard sederhana, transaksi, rekening, anggaran, impor sebagian workbook, dan backup JSON. Workbook asli memiliki 18 sheet dan banyak formula; rumus dan modul lanjutan harus dipetakan, dipindahkan ke logika aplikasi, lalu diuji terhadap hasil Excel sebelum dinyatakan setara.

Pustaka XLSX pada prototipe lama masih dimuat dari CDN, sehingga impor Excel memerlukan koneksi internet. Cache PWA saat ini menyimpan shell aplikasi, bukan pustaka CDN tersebut.

## Uji lokal
Buka `index.html` melalui server lokal atau hosting HTTPS. Service worker dan instalasi PWA tidak aktif bila dibuka langsung sebagai `file://`.
