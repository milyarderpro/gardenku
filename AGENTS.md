# Gardenku — Panduan AI

Dokumen ini adalah **peta kerja untuk AI**, bukan pengganti aturan rinci, template, atau isi video referensi.

## Pembagian tanggung jawab dokumen

| Dokumen/folder | Sumber utama untuk |
|---|---|
| `AGENTS.md` | Memilih alur dan dokumen yang perlu dibaca |
| `rules/*.md` | **Aturan proses**: apa yang boleh, wajib, dan dilarang |
| `templates/*.md` | **Format hasil**: bagian dan kolom yang harus diisi |
| MP4 unggahan pengguna di chat | **Sumber visual utama** untuk sesi analisis; disimpan pengguna di PC, **tidak masuk repo** |
| `references/<creator>/analysis/` | Temuan per video beserta status dan timestamp |
| `references/INDEX.md` | Lokasi file, status, dan pencarian referensi; **bukan bukti isi video** |
| `styles/` | Ringkasan pola visual yang dapat dilacak ke analisis terverifikasi |
| `projects/` | Konsep orisinal, prompt per shot, dan evaluasi hasil generate |
| `projects/legacy/` | Arsip historis; **bukan aturan aktif** |

**Jika petunjuk bersinggungan:** ikuti permintaan spesifik pengguna untuk tujuan/durasi/format selama aman; gunakan `rules/` untuk metode; gunakan `templates/` untuk struktur hasil; gunakan bukti asli untuk fakta tentang referensi. Jangan biarkan contoh template atau arsip lama menggantikan aturan aktif, dan **jangan mengarang bukti** saat video tidak bisa dibuka.

## Pilih alur sesuai permintaan

1. **Analisis referensi saja:** baca [`rules/analysis.md`](rules/analysis.md) dan [`templates/video-analysis.md`](templates/video-analysis.md). **Terima MP4 dari chat**, jangan mencari MP4 aktif di GitHub; MP4 asli disimpan di PC pengguna. Jika tidak bisa mengakses isi video, nyatakan keterbatasan dan jangan mengarang observasi. Tulis timestamp, sumber, ketidakpastian; pilih 2–3 frame JPG representatif secara default. **Jangan membuat ide atau prompt** sebelum diminta.
2. **Buat ide/konsep:** baca [`rules/ideas.md`](rules/ideas.md) dan [`references/INDEX.md`](references/INDEX.md). Gunakan analisis yang sudah terverifikasi; `styles/` hanya pendukung. Gunakan [template konsep](templates/video-concept.md) **jika konsep lengkap diminta atau sebuah ide sudah dipilih**, bukan untuk setiap ide singkat.
3. **Buat prompt Google Veo/Flow:** baca [`rules/prompts.md`](rules/prompts.md), konsep terpilih, dan [`templates/video-prompt.md`](templates/video-prompt.md). Default **satu continuous shot ~8 detik per prompt**, biasanya 2–3 shot berbeda jika membuat beberapa klip; ketentuan eksplisit pengguna tetap diutamakan.
4. **Tambah referensi baru:** tentukan `<creator>` dan ID unik berbahasa Inggris lowercase-kebab-case, buat `analysis/<id>.md` dengan status `pending`, lalu tambahkan baris di `references/INDEX.md`. **Jangan upload MP4 ke repo.** Saat MP4 diterima via chat dan diperiksa, isi analisis dari bukti. Gunakan `frames/<id>/` hanya untuk JPG yang benar-benar diekstrak dari MP4, bukan storyboard AI. Catat sumber/izin bila diketahui.
5. **Simpan dan Verification Gate:** siapkan analisis Markdown dan JPG asli dalam commit yang terkoordinasi; verifikasi isi/ukuran/SHA blob gambar serta tautan, lalu sinkronkan baris [INDEX](references/INDEX.md). Laporkan **PASS / PARTIAL / FAIL** sesuai [aturan analisis](rules/analysis.md); jangan klaim tersimpan jika gagal. `draft` berarti sudah dianalisis AI tetapi belum disetujui; `approved` memerlukan persetujuan pengguna. **Jangan salin angka status/frame ke README lain.**

## Prinsip singkat

- Bahasa isi: Indonesia; istilah teknis kamera Inggris diperbolehkan.
- Bedakan **[OBSERVASI]**, **[KONTEKS PENGGUNA]**, **[INTERPRETASI]**, dan **[BELUM PASTI]**.
- Video `pending` bukan referensi visual terverifikasi. Hindari menyebut sudah menonton jika hanya membaca nama file atau metadata GitHub. Keberadaan audio track tidak berarti suara sudah diperiksa.
- **Shot** = rekaman kontinu; **scene** = kesatuan adegan; **clip** = file atau potongan video.
- Manusia, hewan, hujan, kolam, dan sprinkler bukan elemen wajib.
- Hindari instruksi kamera maju terus jika kamera pan/tracking/detail lebih sesuai dengan subjek.
- MP4 asli tetap di penyimpanan pengguna, bukan GitHub; jangan meminta pengguna mengunggah ulang jika MP4 sudah tersedia dan dapat dibaca dalam sesi ini.
- Jangan mengubah atau menghapus media asli pengguna; penghapusan MP4 repo dalam migrasi ini adalah keputusan eksplisit pengguna.
- [`README.md`](README.md) adalah panduan awal untuk pengguna.
