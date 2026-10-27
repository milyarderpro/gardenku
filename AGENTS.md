# Gardenku — Panduan AI

Dokumen ini adalah **peta kerja untuk AI**, bukan pengganti aturan rinci, template, atau isi video referensi.

## Pembagian tanggung jawab dokumen

| Dokumen/folder | Sumber utama untuk |
|---|---|
| `AGENTS.md` | Memilih alur dan dokumen yang perlu dibaca |
| `rules/*.md` | **Aturan proses**: apa yang boleh, wajib, dan dilarang |
| `templates/*.md` | **Format hasil**: bagian dan kolom yang harus diisi |
| `references/<creator>/videos/` | Bukti media asli (jika benar-benar dapat diakses) |
| `references/<creator>/analysis/` | Temuan per video beserta status dan timestamp |
| `references/INDEX.md` | Lokasi file, status, dan pencarian referensi; **bukan bukti isi video** |
| `styles/` | Ringkasan pola visual yang dapat dilacak ke analisis terverifikasi |
| `projects/` | Konsep orisinal, prompt per shot, dan evaluasi hasil generate |
| `projects/legacy/` | Arsip historis; **bukan aturan aktif** |

**Jika petunjuk bersinggungan:** ikuti permintaan spesifik pengguna untuk tujuan/durasi/format selama aman; gunakan `rules/` untuk metode; gunakan `templates/` untuk struktur hasil; gunakan bukti asli untuk fakta tentang referensi. Jangan biarkan contoh template atau arsip lama menggantikan aturan aktif, dan **jangan mengarang bukti** saat video tidak bisa dibuka.

## Pilih alur sesuai permintaan

1. **Analisis referensi saja:** baca [`rules/analysis.md`](rules/analysis.md) dan [`templates/video-analysis.md`](templates/video-analysis.md); buka video/frame asli jika tersedia; tulis fakta dengan timestamp dan ketidakpastian. **Jangan membuat ide atau prompt** sebelum diminta.
2. **Buat ide/konsep:** baca [`rules/ideas.md`](rules/ideas.md) dan [`references/INDEX.md`](references/INDEX.md). Gunakan analisis yang sudah terverifikasi; `styles/` hanya pendukung. Gunakan [template konsep](templates/video-concept.md) **jika konsep lengkap diminta atau sebuah ide sudah dipilih**, bukan untuk setiap ide singkat.
3. **Buat prompt Google Veo/Flow:** baca [`rules/prompts.md`](rules/prompts.md), konsep terpilih, dan [`templates/video-prompt.md`](templates/video-prompt.md). Default **satu continuous shot ~8 detik per prompt**, biasanya 2–3 shot berbeda jika membuat beberapa klip; ketentuan eksplisit pengguna tetap diutamakan.
4. **Tambah referensi baru:** tentukan `<creator>` dengan nama folder Inggris lowercase-kebab-case; simpan `videos/<id>.mp4`, buat `analysis/<id>.md` berstatus `pending`, lalu perbarui `references/INDEX.md`. Folder `frames/<id>/` digunakan untuk frame JPG **yang benar-benar diekstrak**, bukan storyboard AI. Catat URL sumber/izin bila diketahui, jangan mengasumsikan izin dari fakta bahwa video ada di Facebook.
5. **Selesai menganalisis:** ubah status `pending` menjadi `draft` hanya setelah melihat sumber; status `reviewed` dan `approved` mengikuti [aturan analisis](rules/analysis.md). Perbarui kolom jenis kebun, cuaca, kamera, dan status pada katalog hanya berdasarkan temuan yang terbukti. Profile `styles/` baru dibuat bila mempunyai bukti.

## Prinsip singkat

- Bahasa isi: Indonesia; istilah teknis kamera Inggris diperbolehkan.
- Bedakan **[OBSERVASI]**, **[KONTEKS PENGGUNA]**, **[INTERPRETASI]**, dan **[BELUM PASTI]**.
- Video `pending` bukan referensi visual terverifikasi. Hindari menyebut sudah menonton jika hanya membaca nama file.
- **Shot** = rekaman kontinu; **scene** = kesatuan adegan; **clip** = file atau potongan video.
- Manusia, hewan, hujan, kolam, dan sprinkler bukan elemen wajib.
- Hindari instruksi kamera maju terus jika kamera pan/tracking/detail lebih sesuai dengan subjek.
- Jangan mengubah atau menghapus media asli tanpa perintah pengguna.
- [`README.md`](README.md) adalah panduan awal untuk pengguna.
