# Website Al Barokah — GitHub Pages

Paket website statis. Alamat yang disiapkan: https://albarokah.ojieidgroup.my.id

## Publikasi

1. Buat repository GitHub terpisah, misalnya `albarokah-website`, agar source website utama tidak tertimpa. Repository publik dapat digunakan dengan GitHub Pages pada akun Free; repository privat memerlukan paket yang mendukung Pages.
2. Unggah `index.html`, `CNAME`, dan `.nojekyll` ke root branch `main`.
3. Buka Settings > Pages. Pada Build and deployment pilih Deploy from a branch, branch `main`, folder `/ (root)`, lalu Save.
4. Pastikan Custom domain di Settings > Pages adalah `albarokah.ojieidgroup.my.id`.
5. Pada Cloudflare > domain ojieidgroup.my.id > DNS, tambahkan record berikut:
   - Type: CNAME
   - Name: albarokah
   - Target: ojieid03-cmd.github.io
   - Proxy status: DNS only (awan abu-abu) untuk verifikasi awal dan sertifikat GitHub Pages.
   - TTL: Auto
6. Jangan mengubah record domain utama atau www. Jika record albarokah sudah ada, periksa penggunaannya sebelum mengubahnya.
7. Tunggu DNS check dan penerbitan sertifikat selesai, kemudian aktifkan Enforce HTTPS di GitHub Pages.
8. Periksa https://albarokah.ojieidgroup.my.id melalui perangkat lain.

CNAME mengasumsikan repository dibuat di akun `ojieid03-cmd`. Jika akun pemilik berbeda, sesuaikan target DNS dengan alamat Pages yang diberikan GitHub.

Form hanya menyiapkan pesan WhatsApp, tidak menyimpan data pelanggan. Ilustrasi produk merupakan contoh, bukan dokumentasi produksi.

Paket ini belum diunggah atau dipublikasikan secara otomatis.
