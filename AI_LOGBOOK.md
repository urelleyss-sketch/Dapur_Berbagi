# AI Logbook - DapurBerbagi

Dokumentasi ini mencatat proses interaksi dan pemanfaatan kecerdasan buatan (AI) dalam pengembangan aplikasi web DapurBerbagi.

## Tahap 1: Eksplorasi Ide & Perancangan Solusi
- **Interaksi AI**: Meminta saran konsep aplikasi berbasis web untuk mengurangi limbah makanan (*food waste*) di tingkat tetangga/kecamatan.
- **Hasil Saran AI**: Mengusulkan fitur utama seperti feed berbagi makanan antar warga, pelacak stok kulkas dengan indikator kedaluwarsa, resep pintar berdasarkan bahan sisa, serta integrasi kupon UMKM lokal.
- **Validasi & Modifikasi Mandiri**: Kami memilih dan memfokuskan wilayah administratif ke Kabupaten Trenggalek dan sekitarnya agar relevan dengan kondisi lokal, serta menyesuaikan alur konfirmasi pengambilan makanan menjadi 2 tahap (Booking & Selesai Diambil) demi keamanan warga.

## Tahap 2: Penyusunan Kerangka Kode (Scaffolding)
- **Interaksi AI**: Meminta bantuan pembuatan struktur dasar file modular (`index.html`, `style.css`, `script.js`) menggunakan Tailwind CSS dan font modern.
- **Hasil Saran AI**: Draf kode kerangka antarmuka pengguna ala aplikasi seluler (*mobile-first layout*) dengan navigasi bawah (*bottom navigation*).
- **Validasi & Modifikasi Mandiri**: Kami merapikan struktur tag HTML, memastikan tautan file CSS dan JavaScript terhubung dengan benar di GitHub Pages, serta menambahkan database dropdown wilayah berjenjang (Kabupaten > Kecamatan > Desa).

## Tahap 3: Pemecahan Masalah & Penanganan Galat (Debugging)
- **Interaksi AI**: Berkonsultasi terkait tautan foto Unsplash eksternal yang terkadang gagal dimuat (*broken image*) serta error 404 saat *deployment* di GitHub Pages.
- **Hasil Saran AI**: Menambahkan fungsi penanganan error gambar (`onerror` fallback dengan SVG/gambar cadangan kategori) dan pengecekan nama file *case-sensitive*.
- **Validasi & Modifikasi Mandiri**: Kami menguji coba kode galat tersebut langsung di browser dan memastikan seluruh path file menggunakan huruf kecil seluruhnya agar sukses online di GitHub Pages.

## Tahap 4: Refleksi & Penjelasan Kode
- **Pemahaman Tim**: Kami memahami bahwa aplikasi ini menggunakan `localStorage` untuk penyimpanan data sisi klien (*client-side*) secara lokal tanpa memerlukan *backend* server yang rumit. 
- **Verifikasi Mandiri**: Seluruh logika fungsi JavaScript mulai dari filter resep berdasarkan bahan utama, penambahan stok kulkas, hingga sistem poin pahlawan pangan telah diverifikasi dan diuji coba secara mandiri oleh tim.
