# SIKOMANG GitHub Pages — Patch halaman legal & homescreen satu layar

## Isi
- `index.html` — homescreen dengan tautan footer menuju halaman legal lokal.
- `kebijakan-privasi.html` — halaman Kebijakan Privasi.
- `syarat-dan-ketentuan.html` — halaman Syarat dan Ketentuan.
- `css/styles.css` — stylesheet homescreen dan tambahan aturan satu layar.

## Cara memasang
1. Ekstrak ZIP.
2. Salin seluruh isi folder hasil ekstrak (bukan folder induknya) ke root repository `sikomangnv.github.io`.
3. Pilih Replace/Overwrite jika GitHub meminta konfirmasi.
4. Commit changes.
5. Tunggu GitHub Pages selesai deploy, lalu hard refresh `https://sikomangnv.github.io/` (Ctrl+F5).

## Catatan
- Perubahan hanya untuk homescreen GitHub Pages dan dua halaman legal. Tidak mengubah aplikasi SIKOMANG di Vercel/Supabase atau Blogger.
- Halaman dokumen legal tetap dapat discroll karena isinya panjang. Penguncian scroll vertikal hanya berlaku pada homescreen.
- Pada layar yang sangat pendek atau zoom browser besar, konten mungkin perlu dikecilkan oleh browser; periksa desktop dan HP setelah deploy.


## Patch V2 — pemulihan ukuran logo dan teks
Paket ini mempertahankan patch halaman legal lokal dan homescreen satu layar,
tetapi menghapus efek pengecilan ukuran logo/judul/deskripsi/teks pendukung
yang sebelumnya mengikuti tinggi layar. Salin seluruh isi ZIP ke root repo
`sikomangnv.github.io` (tanpa membuat subfolder), lalu pilih Replace/Overwrite.
Setelah Pages selesai deploy, buka dengan Ctrl+F5 atau jendela Incognito.
