# References — Pustaka Analisis dan Frame

Folder ini menyimpan **pengetahuan hasil analisis** video referensi kebun, bukan file MP4. Video asli dikirim pengguna melalui chat untuk dianalisis dan **disimpan secara pribadi di PC pengguna**. GitHub menyimpan catatan Markdown dan JPG hasil ekstraksi yang terverifikasi.

Cari referensi, status, dan metadata ringkas di [INDEX](INDEX.md). Hasil, Shot Map, dan Contact Sheet Manifest setiap video yang sudah dianalisis menjadi sumber rincian utama; README tidak mengulang angka status yang cepat berubah.

## Menambahkan atau menganalisis referensi — Two-Phase

**Fase 1 — Analyze & Review (tahap 1–5; TANPA penulisan GitHub):**

1. Tentukan koleksi/kreator, ID unik lowercase-kebab-case, dan baca [INDEX](INDEX.md) serta analisis lama. **Untuk ID baru, jangan membuat file `pending` maupun baris INDEX di GitHub pada fase ini.** Susun hanya rencana/draft lokal.
2. Ketika pengguna mengunggah MP4 lewat chat, periksa video yang benar-benar dapat diakses. Analisis berdasarkan [rules/analysis.md](../rules/analysis.md) dan [template](../templates/video-analysis.md): Shot Map, Deep Shot Analysis, dan Evidence Cross-Check. MP4 asli tetap di PC pengguna.
3. Buat **1 contact sheet JPG per shot** secara lokal, dengan target **3–6 panel kronologis adaptif** dan timestamp. Beri nama `shot-XX.jpg`; versi di bawah ambang kualitas memakai `shot-XX-preview.jpg` sesuai aturan utama, bukan sekadar karena panel diperkecil wajar.
4. Tampilkan hasil analisis, Shot Map, Contact Sheet Manifest **sementara**, dan **file JPG individual yang dapat diunduh** kepada pengguna untuk ditinjau dan digunakan lagi pada Fase 2. Catat `Fase 1 — menunggu review/save now` dan Gate A/B/overall `belum dijalankan`. **Jangan upload JPG, mengubah status, membuat branch/commit/PR, atau memperbarui INDEX.** Revisi hanya artefak lokal sampai pengguna mengizinkan penyimpanan.

**Fase 2 — Save & Verify (tahap 6–7; HANYA setelah `save now`/instruksi simpan eksplisit):**

5. Gunakan **versi analisis terakhir** yang sudah direview dan **JPG individual yang telah tersedia untuk diunduh dari Fase 1**. **Jika konektor gagal mengunggah JPG**, gunakan branch staging khusus dan berikan **instruksi path tujuan + checksum dari Manifest Fase 1**. Pengguna mengunggah **JPG yang sama**, tanpa ZIP atau ekspor ulang, ke **branch staging** (bukan `main`). AI kemudian mencocokkan semua nama/path, jumlah, SHA Git blob dan byte. Jika kurang/salah, berhenti dan minta perbaikan; **jangan commit Markdown/INDEX yang menautkan file belum ada**. Referensi baru dan INDEX hanya dibuat dalam Fase 2.
6. Jika JPG sudah lolos pemeriksaan, commit analisis + [INDEX](INDEX.md) secara terkoordinasi **ke branch staging yang sama**, isi Contact Sheet Manifest dengan link nyata, kemudian buka PR tanpa merge otomatis. Verifikasi HEAD, link dan semua JPG, lalu jalankan **Gate A Visual Accuracy** dan **Gate B Repository Integrity** resmi. Jika pengguna belum upload, status `menunggu upload manual`; konfirmasi upload melanjutkan Fase 2 tanpa `save now` ulang. Status hasil AI umumnya `draft`; `save now` bukan `approved` atau izin merge. Detail standar berada di [aturan utama](../rules/analysis.md).

**Aturan global:** `references/INDEX.md` menjadi katalog/status **hanya untuk berkas yang benar-benar disimpan**; catatan Fase 1 tidak dimasukkan ke INDEX. Detail penentuan resolusi, shot, panel, dan hasil Gate tetap ada pada [aturan utama](../rules/analysis.md); jangan menduplikasi rules teknis di README.

**Jangan menyimpan storyboard AI atau gambar hasil pencarian sebagai frame referensi.** Repositori publik bukan bukti izin mendistribusikan JPG atau video. Penghapusan MP4 dari tree Git terbaru **tidak membersihkan riwayat Git lama**.
