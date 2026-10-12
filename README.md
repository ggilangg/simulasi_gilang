# Simulator Kredit Mobil (PWA)

Simulator kredit konvensional, hybrid, Mini For Max (8 tahun), dan EV. Bisa dipasang di HP lewat Chrome dan tetap jalan tanpa internet.

## Isi paket
```
index.html              aplikasi
manifest.webmanifest    data instalasi (nama, ikon, warna)
sw.js                   service worker (mode offline)
icons/                  ikon mobil sport (192, 512, maskable, apple-touch, favicon)
README.md               panduan ini
```

## 1. Upload ke GitHub
1. Buka github.com, login, lalu **New repository**. Beri nama, misalnya `simulator-kredit`, pilih **Public**, klik **Create repository**.
2. Klik **uploading an existing file**, lalu seret **semua isi paket** (termasuk folder `icons`). Pastikan `index.html` ada di halaman utama repository, bukan di dalam subfolder.
3. Klik **Commit changes**.

## 2. Aktifkan GitHub Pages
1. Di repository, buka **Settings > Pages**.
2. Pada **Source**, pilih **Deploy from a branch**. Pilih branch `main` dan folder `/ (root)`, lalu **Save**.
3. Tunggu 1-2 menit. Alamat aplikasi muncul di halaman yang sama:
   `https://USERNAME.github.io/simulator-kredit/`

## 3. Pasang di HP (Chrome Android)
1. Buka alamat di atas di **Chrome**.
2. Ketuk tombol **Pasang** di pojok kanan atas aplikasi, atau menu Chrome (titik tiga) lalu **Instal aplikasi** / **Tambahkan ke layar utama**.
3. Ikon mobil sport muncul di layar utama. Buka dari sana dan aplikasi tampil layar penuh.

## Catatan penting
- **Data tersimpan di HP itu sendiri.** Riwayat hitungan dan perubahan di tab Database (bunga, admin, dan lainnya) disimpan di browser perangkat. Tidak otomatis tersinkron antar HP dan hilang kalau Anda menghapus data situs Chrome.
- Kalau ingin database bersama untuk satu tim, itu perlu server atau layanan penyimpanan tambahan.
- **Memperbarui aplikasi:** ganti `index.html` di GitHub, lalu naikkan angka versi di `sw.js` (`sim-kredit-v1` menjadi `sim-kredit-v2`). Tutup dan buka lagi aplikasi di HP, dan versi baru dipakai.
- Tarif (bunga, admin, asuransi, dan lainnya) mengikuti Excel Juni 2026. Cek ulang kalau memo tarif berubah.
