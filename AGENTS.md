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

**Aturan operasional utama — Opsi B+ v1.3 (Two-Phase + Document-First Save):** semua permintaan **analisis video dari chat** dijalankan dengan **Fase 1, tahap 1–5 saja**. AI boleh **membaca** repository untuk konteks, tetapi **tidak boleh membuat/mengubah file, branch, commit, JPG, PR atau INDEX di GitHub**. Buat analisis dan contact sheet sementara secara lokal, lakukan Evidence Cross-Check, **tampilkan hasil untuk direview**, lalu **BERHENTI**. Tunggu revisi atau perintah eksplisit **`save now`** (atau instruksi simpan lain yang sama jelasnya). **Baru setelah izin itu, kerjakan Fase 2, tahap 6–7:** simpan **versi analisis terbaru + INDEX langsung ke `main`**, tanpa upload JPG, lalu jalankan Dual Verification Gate untuk **analisis dan dokumen**. `save now` **tidak** bermakna `approved` atau izin merge. Ketentuan lengkap dan pengecualian hanya berada di [aturan analisis](rules/analysis.md).

1. **Analisis referensi (Fase 1):** baca [`rules/analysis.md`](rules/analysis.md) dan [`templates/video-analysis.md`](templates/video-analysis.md). Terima MP4 dari chat; MP4 asli tetap di PC pengguna. Lakukan **tahap 1–5 saja**: validasi, Shot Map dua-pass, analisis mendalam, buat **1 JPG contact sheet lokal per shot (target 3–6 panel adaptif)**, Evidence Cross-Check. **Berikan JPG individual yang dapat diunduh untuk pengguna arsipkan sendiri melalui repo lokal**; tampilkan hasil dan berhenti untuk review; **jangan menulis ke GitHub selama Fase 1** atau membuat ide/prompt sebelum diminta.
2. **Buat ide/konsep:** baca [`rules/ideas.md`](rules/ideas.md) dan [`references/INDEX.md`](references/INDEX.md). Gunakan analisis yang sudah terverifikasi; `styles/` hanya pendukung. Gunakan [template konsep](templates/video-concept.md) **jika konsep lengkap diminta atau sebuah ide sudah dipilih**, bukan untuk setiap ide singkat.
3. **Buat prompt Google Veo/Flow:** baca [`rules/prompts.md`](rules/prompts.md), konsep terpilih, dan [`templates/video-prompt.md`](templates/video-prompt.md). Default **satu continuous shot ~8 detik per prompt**, biasanya 2–3 shot berbeda jika membuat beberapa klip; ketentuan eksplisit pengguna tetap diutamakan.
4. **Referensi baru:** pada Fase 1 tentukan ID unik dan siapkan **draft lokal** saja, tanpa membuat berkas `pending` baru atau menambah INDEX. Setelah `save now`, buat/ubah **hanya** `analysis/<id>.md` dan INDEX **langsung di `main`**, dengan 10 bagian, Shot Map, Manifest path JPG dan kedua Gate. JPG dikelola pengguna melalui repo lokal, **bukan** diunggah AI. Jangan menimpa data `approved` tanpa instruksi.
5. **Perintah `save now` (Fase 2):** simpan hasil review terakhir berupa **Markdown analisis 10 bagian + pembaruan INDEX langsung ke `main`** dalam commit terkoordinasi dengan pengecekan HEAD/lease. **AI tidak perlu membuat branch, PR, ZIP, upload JPG atau menunggu file JPG muncul di GitHub.** Manifest tetap memuat nama/path standar JPG sebagai lokasi arsip yang akan dikelola pengguna; hindari hyperlink yang belum tersedia dan klaim upload palsu. Setelah commit, verifikasi **Gate A Visual Accuracy + Gate B Document & Repository Integrity**. **Gate B tidak memeriksa keberadaan JPG**, sehingga keseluruhan bisa PASS meskipun JPG belum di-push. `save now` bukan `approved`; lihat detail di [rules/analysis.md](rules/analysis.md).

## Prinsip singkat

- Bahasa isi: Indonesia; istilah teknis kamera Inggris diperbolehkan.
- Bedakan **[OBSERVASI]**, **[KONTEKS PENGGUNA]**, **[INTERPRETASI]**, dan **[BELUM PASTI]**.
- Video `pending` bukan referensi visual terverifikasi. Hindari menyebut sudah menonton jika hanya membaca nama file atau metadata GitHub. Keberadaan audio track tidak berarti suara sudah diperiksa.
- **Shot** = rekaman kontinu; **scene** = kesatuan adegan; **clip** = file atau potongan video.
- Manusia, hewan, hujan, kolam, dan sprinkler bukan elemen wajib.
- Hindari instruksi kamera maju terus jika kamera pan/tracking/detail lebih sesuai dengan subjek. **Bedakan pan/tracking/zoom berdasarkan MP4 bergerak**, bukan berdasarkan satu gambar diam.
- MP4 asli tetap di penyimpanan pengguna, bukan GitHub. Pengguna mengelola JPG melalui repo lokal. Jika MP4 hilang, hanya minta kembali bila memang perlu memverifikasi isi analisis; **jangan jadikan ketiadaan JPG remote sebagai penghalang penyimpanan dokumen**.
- Jangan mengubah atau menghapus media asli pengguna; penghapusan MP4 repo dalam migrasi ini adalah keputusan eksplisit pengguna.
- [`README.md`](README.md) adalah panduan awal untuk pengguna.
