# References — Pustaka Analisis dan Frame

Folder ini menyimpan **pengetahuan hasil analisis** video referensi kebun, bukan file MP4. Video asli dikirim pengguna melalui chat untuk dianalisis dan **disimpan secara pribadi di PC pengguna**. AI menyimpan analisis Markdown dan INDEX; pengguna menyimpan JPG ekstraksi sendiri melalui repo lokal.

Cari referensi, status, dan metadata ringkas di [INDEX](INDEX.md). Hasil, Shot Map, dan Contact Sheet Manifest setiap video yang sudah dianalisis menjadi sumber rincian utama; README tidak mengulang angka status yang cepat berubah.

## Menambahkan atau menganalisis referensi — Two-Phase

**Fase 1 — Analyze & Review (tahap 1–5; TANPA penulisan GitHub):**

1. Tentukan koleksi/kreator, ID unik lowercase-kebab-case, dan baca [INDEX](INDEX.md) serta analisis lama. **Untuk ID baru, jangan membuat file `pending` maupun baris INDEX di GitHub pada fase ini.** Susun hanya rencana/draft lokal.
2. Ketika pengguna mengunggah MP4 lewat chat, periksa video yang benar-benar dapat diakses. Analisis berdasarkan [rules/analysis.md](../rules/analysis.md) dan [template](../templates/video-analysis.md): Shot Map, Deep Shot Analysis, dan Evidence Cross-Check. MP4 asli tetap di PC pengguna.
3. Buat **1 contact sheet JPG per shot** secara lokal, dengan target **3–6 panel kronologis adaptif** dan timestamp. Beri nama `shot-XX.jpg`; versi di bawah ambang kualitas memakai `shot-XX-preview.jpg` sesuai aturan utama, bukan sekadar karena panel diperkecil wajar.
4. Tampilkan hasil analisis, Shot Map, Contact Sheet Manifest sementara, dan **file JPG individual yang dapat diunduh untuk disimpan pengguna lewat repo lokal**. Catat `Fase 1 — menunggu review/save now` dan Gate A/B/overall `belum dijalankan`. **Jangan upload JPG, mengubah status, membuat branch/commit/PR, atau memperbarui INDEX.** Revisi hanya artefak lokal sampai pengguna mengizinkan penyimpanan.

**Fase 2 — Save & Verify (tahap 6–7; setelah `save now`):**

5. Gunakan **versi analisis terakhir**; simpan **hanya** `<creator>/analysis/<id>.md` (10 bagian, Shot Map dan Contact Sheet Manifest) beserta [INDEX](INDEX.md) **langsung ke branch `main`** dalam commit terkoordinasi. Verifikasi HEAD sebelum/sesudah penulisan untuk menghindari overwrite konflik. **Jangan buat branch/PR untuk penyimpanan analisis rutin; AI tidak mengunggah JPG atau ZIP.**
6. Manifest mencantumkan **nama/path standar JPG** sebagai lokasi arsip yang akan dikelola pengguna; tidak perlu tautan aktif, status `pending JPG`, SHA GitHub atau verifikasi JPG remote. **Gate A = akurasi visual**, **Gate B = integritas dokumen + INDEX**. Jika keduanya PASS, overall PASS meskipun pengguna belum memasukkan JPG ke repo. Ketiadaan JPG bukan alasan PARTIAL. Status hasil AI biasanya `draft`; `save now` bukan `approved`.

**Aturan global:** `references/INDEX.md` menjadi katalog/status **untuk analisis Markdown yang benar-benar disimpan**; catatan Fase 1 tidak dimasukkan ke INDEX. JPG ditangani pengguna dan tidak memengaruhi status analisis. Detail penentuan resolusi, shot, panel, dan hasil Gate tetap ada pada [aturan utama](../rules/analysis.md); jangan menduplikasi rules teknis di README.

**Jangan menyimpan storyboard AI atau gambar hasil pencarian sebagai frame referensi.** Repositori publik bukan bukti izin mendistribusikan JPG atau video. Penghapusan MP4 dari tree Git terbaru **tidak membersihkan riwayat Git lama**.
