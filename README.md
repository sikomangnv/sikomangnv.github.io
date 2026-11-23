# Migrasi Homescreen SIKOMANG ke GitHub Pages (versi paralel)

Paket ini adalah konversi awal dari XML Blogger yang diberikan. Blogger tetap berjalan dan tidak perlu dihapus atau diubah. Aplikasi utama tetap berada di https://sikomangnv.vercel.app/.

## Isi paket
- `index.html` — homescreen SIKOMANG yang dikonversi dari struktur homepage XML.
- `css/styles.css` — aturan CSS dari `<b:skin>` asli, dipertahankan; fragmen HTML yang terselip di blok CSS dibuang karena bukan aturan CSS.

## Cara uji di GitHub Pages
1. Buat repository GitHub, misalnya `sikomang-homescreen`.
2. Upload seluruh isi folder ini ke root repository.
3. Buka **Settings → Pages**.
4. Pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu Save.
5. Setelah GitHub Pages menerbitkan situs, buka URL yang diberikan GitHub dan bandingkan di desktop serta HP dengan Blogger.

## Item yang masih perlu dilengkapi sebelum dianggap final
1. Ganti `https://LINK-DOKUMENTASI-ANDA` dengan URL dokumentasi yang benar.
2. Ganti domain contoh `GANTI-DENGAN-URL-BLOGGER-ANDA.blogspot.com` pada tautan Kebijakan Privasi dan Syarat & Ketentuan. Setelah konten asli kedua halaman diberikan/diekspor, tautan dapat diarahkan ke file statis GitHub agar semua halaman ikut pindah.
3. Gambar/logo/background sementara tetap memakai URL `blogger.googleusercontent.com` yang sama seperti XML sumber. Ini menjaga tampilan dan menghindari perubahan aset saat tahap pertama. Aset dapat disalin ke folder `assets/` kemudian jika diinginkan.

## Batasan konversi
- Kode khusus Blogger (`b:if`, `b:section`, `Blog1`, `data:post.body`, komentar Blogger) tidak dipakai pada halaman statis GitHub.
- Pengalihan `?m=0` khusus Blogger dihilangkan; layout responsif CSS asli tetap dipakai.
- Tidak ada perubahan pada backend, database, autentikasi, atau aplikasi SIKOMANG di Vercel.
