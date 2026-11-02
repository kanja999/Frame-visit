# Ambil Frame Video (PWA)

Aplikasi web untuk mengambil satu frame dari video atau memproses foto menjadi JPEG berukuran **640 × 852 px**, dengan time stamp opsional dan konversi ke base64. Semua proses berjalan di browser; file tidak diunggah ke server mana pun.

## Fitur
- Pilih video atau foto dari perangkat
- Slider/timeline dan tombol -1 / +1 frame
- Hasil JPEG 640 × 852 px (opsi: isi penuh atau muat utuh)
- Time stamp `dd/mm/yyyy, jam:menit:detik` (236 × 22 px, hitam 50%), waktu otomatis atau manual, posisi bisa dipilih
- Konversi ke base64 dengan tombol Salin dan Bagikan
- Bisa dipasang sebagai aplikasi dan dipakai offline

## Deploy ke GitHub Pages
1. Buat repository baru di GitHub (misalnya `ambil-frame`), public.
2. Unggah **semua isi** folder ini ke root repository (`index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`, `.nojekyll`, `README.md`). Bisa lewat tombol **Add file > Upload files** atau `git push`.
3. Buka **Settings > Pages**. Pada *Build and deployment*, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu **Save**.
4. Tunggu 1 sampai 2 menit. Alamatnya: `https://USERNAME.github.io/ambil-frame/`
5. Buka alamat itu di HP atau laptop, lalu pilih **Tambahkan ke layar utama** atau ikon **Install** di address bar.

GitHub Pages memakai HTTPS, jadi syarat PWA dan fitur salin/bagikan terpenuhi.

## Memperbarui aplikasi
Setelah mengubah file, naikkan nama cache di `sw.js` (misalnya `ambil-frame-v8` menjadi `ambil-frame-v9`) agar pengguna mendapat versi terbaru.

## Uji lokal
Jalankan server lokal di folder ini, misalnya `python3 -m http.server 8000`, lalu buka `http://localhost:8000`.
