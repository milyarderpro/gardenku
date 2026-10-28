# Aturan Analisis Video Referensi — Gardenku
**Versi:** 1.3 — Opsi B+ Two-Phase Workflow + Document-First Save (Analyze & Review → Save & Verify)  
**Berlaku untuk:** `references/<creator>/analysis/<video-id>.md`  
**Tujuan:** Mengubah video asli menjadi catatan visual yang akurat dan bisa dipakai ulang oleh AI untuk mengembangkan konsep video kebun.

> Dokumen ini berisi **aturan kerja**, bukan hasil analisis video tertentu. Format berkas analisis baku tersedia di `templates/video-analysis.md`.

## 1. Kapan aturan ini digunakan?
Gunakan saat pengguna meminta AI menonton, mengamati, memecah shot, atau menganalisis **video referensi kebun**. **Jangan membuat ide atau prompt video** apabila pengguna hanya meminta analisis.

Baca `AGENTS.md`, lalu cek [INDEX](../references/INDEX.md) dan file analisis yang ada. Sumber video **selalu MP4 unggahan chat dari pengguna** (aslinya disimpan pengguna di PC). GitHub **tidak menyimpan MP4**. **AI hanya menyimpan dokumen analisis dan INDEX; pengguna mengelola JPG melalui repository lokal secara terpisah.** Contoh:
- Input: pengguna mengunggah `muyon-01.mp4` di chat (nama input dapat berbeda).
- Analisis: `references/muyon/analysis/muyon-01.md`.
- JPG bukti: `references/muyon/frames/muyon-01/`.

Katalog mencatat **referensi**, bukan lokasi MP4 yang dapat diunduh. Saat membuka sesi baru, minta unggahan MP4 hanya bila belum tersedia/dapat dibaca di sesi tersebut.

## 2. Prinsip wajib
1. **Utamakan yang benar-benar terlihat atau terdengar.** Bila video tidak dapat dibuka, jelaskan keterbatasannya; jangan menyusun analisis lengkap seolah sudah menonton.
2. **Pisahkan sumber informasi:**
   - `[OBSERVASI]` — terlihat/terdengar pada video atau frame asli.
   - `[KONTEKS PENGGUNA]` — informasi yang disampaikan pengguna, misalnya "setelah hujan deras".
   - `[INTERPRETASI]` — perkiraan atau penilaian teknis AI.
   - `[BELUM PASTI]` — detail belum dapat diperiksa atau bukti kurang kuat.
3. **Cantumkan timestamp** untuk temuan penting. Gunakan kata "perkiraan" untuk batas shot/waktu yang tidak diukur secara presisi.
4. **Jangan menebak** nama tanaman, jenis buah, jam pengambilan gambar, identitas orang, alat kamera, ukuran lahan, jumlah shot, atau jenis suara tanpa bukti.
5. **Jaga konteks:** referensi kebun terbuka, pekarangan depan, backyard, rooftop, dan kebun dalam pot **bisa sangat berbeda**. Jangan memaksakan karakter kebun luas pada referensi lahan kecil.
6. **Hewan, manusia, kolam, alat, dan cuaca adalah elemen opsional**: periksa keberadaannya, tetapi tulis "tidak terlihat" bila tidak ada.
7. **MP4 asli disimpan di PC pengguna; jangan mengubah atau menghapus salinan pribadi.** AI tidak mengunggah MP4 maupun JPG ke GitHub; pengguna menyimpan JPG sendiri lewat repo lokal. JPG ekstraksi tetap karya turunan video; periksa hak penggunaan saat repo publik.

## 3. Urutan analisis

**Two-Pass Video Inspection wajib:** (1) *Pass 1 / Video Structure Mapping* telusuri seluruh timeline, sampling awal sekitar 0,5–1 detik lalu lebih rapat dekat cut/dissolve, buat Shot Map; (2) *Pass 2 / Deep Shot Analysis* periksa tiap shot dan gerak video asli dari awal hingga akhir. Interval sampling bukan pengganti melihat video bergerak. Waktu yang belum presisi wajib ditandai `perkiraan`.

### A. Identitas dan gambaran keseluruhan
Catat identitas sumber/kreator, nama video, lokasi file, durasi, resolusi, aspek rasio, dan FPS **jika dapat diverifikasi**. Catat tautan sumber asli dan izin penggunaan bila tersedia; bila tidak, tulis "belum diketahui".

Tuliskan ringkasan 3–5 kalimat mengenai:
- Jenis kebun dan perkiraan karakter ruang: kebun terbuka luas, front-yard kecil, backyard, pot, hydroponic, dan sebagainya.
- Tingkat kerimbunan, jenis tanaman dominan, keberadaan bedengan/lorong/trellis/kolam.
- Gaya kamera dan suasana utama.
- Apa yang membuat video menarik sejak detik awal (*visual hook*).

### B. Pecah menjadi shot
**Shot** = gambar kontinu di antara dua cut. **Scene** = kesatuan tempat/kejadian; dapat memuat beberapa shot. **Clip** = segmen/file digital. Jangan menyamakan ketiganya.

Untuk **setiap shot**, catat:
- Nomor shot, waktu mulai–akhir, dan durasi (tepat atau perkiraan).
- **Hero subject:** tanaman, buah, aktivitas, atau detail yang paling menonjol.
- Subjek pendukung dan apa yang terlihat di awal, tengah, akhir.
- **Camera movement:** static, pan left/right, tilt up/down, tracking lateral, push-in/dolly-in, pull-back, zoom; tulis gabungan hanya jika tampak nyata.
- **Framing dan angle:** wide/medium/close-up, jarak relatif, posisi kamera tinggi/rendah, arah pandang.
- **Komposisi:** foreground, middle ground, background; cara warna buah/daun dan elemen lain mengarahkan perhatian.
- **Garden layout:** bedengan, jalan setapak, batas bata/kayu/batu, pot, trellis, pohon buah, aliran air, kolam, rumah/pagar.
- Cuaca, kualitas cahaya, warna dan kondisi permukaan.
- Jenis transisi menuju shot berikut jika terlihat.

**Perbedaan gerak kamera:** pan = kamera berputar kiri/kanan; tilt = berputar atas/bawah; tracking = kamera berpindah posisi menyamping; push-in = posisi kamera mendekati objek; zoom = pembesaran optik/digital. Jangan menyebut semua gerak sebagai "kamera maju". **Verifikasi gerak dari MP4**, bukan dari JPG saja. Jika pan, tracking atau zoom sulit dibedakan, tulis `[INTERPRETASI]` dan tingkat keyakinannya. Catat perkembangan visual **awal → tengah → akhir** tiap shot.

### C. Detail lingkungan, cuaca, dan air
Periksa bila relevan:
- Kondisi waktu: pagi, siang, sore **hanya jika ada bukti**; langit mendung sendiri tidak membuktikan jam.
- Cahaya: hangat/dingin, langsung/tersebar, arah cahaya, bayangan, warna keseluruhan.
- Hujan: sebelum/setelah hujan, gerimis aktif, tetes di daun, permukaan basah, genangan, kabut.
- **Bedakan gerimis alami, sprinkler, selang, air terjun/kolam, dan percikan dari hewan.** Jika sumber air tidak jelas, tandai `[BELUM PASTI]`.
- Gerakan alam: daun, angin, air mengalir, riak kolam.

Jika pengguna menyebut "setelah hujan deras, masih gerimis", cantumkan sebagai `[KONTEKS PENGGUNA]` dan cari bukti visual yang mendukung; jangan mengklaim bahwa intensitas gerimis terukur jika tidak terlihat.

### D. Hewan, manusia, alat, dan aktivitas
Untuk objek yang **memang tampak**, catat: jenis umum, jumlah yang terlihat, posisi dalam frame, timestamp, gerakan, interaksi dengan kebun, serta peran visual (**utama / pendukung / latar**).

Contoh: ayam mematuk tanah di samping bedengan, bebek berenang di tepi kolam, ikan menghasilkan riak air, manusia memakai caping sedang memanen cabai, keranjang diletakkan di jalan. Ini adalah **contoh kategori**, bukan klaim mengenai referensi tertentu.

Jangan menebak identitas orang, hubungan keluarga, atau niat/emosi hewan. Catat penampilan umum hanya sebatas yang relevan secara visual.

### E. Audio, editing, dan ritme
Jika audio benar-benar dapat diperiksa, catat suara air/hujan/angin/burung/hewan/langkah, percakapan, musik, serta hubungannya dengan gambar. Jika tidak, tulis **"audio belum diperiksa"**. Bedakan suara asli video dengan musik tambahan bila memungkinkan.

Catat jumlah shot, kisaran durasi shot, pola urutan subjek, hard cut/dissolve (jika dapat diamati), dan tempo perubahan visual.

## 4. Kesimpulan untuk pustaka AI
Akhiri analisis dengan empat bagian:
1. **Karakter visual utama:** maksimal 5 ciri khas yang benar-benar terdukung.
2. **Teknik yang dapat digunakan kembali:** misalnya transisi fokus dari tomat dekat kamera menuju pohon pepaya di belakang, atau slow pan melintasi bedengan setelah hujan.
3. **Elemen khas tetapi tidak wajib ditiru:** misalnya manusia, bebek, kolam, atau jenis buah tertentu.
4. **Keterbatasan / ketidakpastian:** data mana yang masih memerlukan pemeriksaan.

Tambahkan **tag pencarian** bila faktanya didukung, misalnya `front-yard`, `open-field`, `after-rain`, `light-drizzle`, `slow-pan`, `bamboo-trellis`, `pond-fish`. Jangan membuat tag berdasarkan dugaan.



## 5. Workflow Opsi B+ — 7 tahap resmi

**Metode:** Evidence-Driven Video Analysis + Adaptive Per-Shot Contact Sheet + Dual Verification Gate. **Ketujuh tahap tetap berlaku, dibagi menjadi dua fase.** MP4 diterima lewat chat dan disimpan pengguna di PC. **Fase 1 menghasilkan JPG untuk pengguna; Fase 2 hanya menyimpan analisis Markdown dan INDEX langsung ke `main`.** Pengguna mengelola JPG melalui repo lokal. Bagian ini sumber aturan baku; AGENTS adalah navigasi dan template adalah format keluaran.

### Batas izin dua fase (WAJIB)

**FASE 1 — Analyze & Review (Tahap 1–5)**

- **Pemicu:** pengguna mengunggah MP4 dan meminta analisis. AI **boleh membaca** aturan, template, INDEX dan analisis lama dari repo, serta memproses MP4 dan membuat file JPG/contact sheet **sementara secara lokal** untuk diperlihatkan kepada pengguna.
- Kerjakan kelima tahap sampai **Evidence Cross-Check**. Tampilkan hasil analisis lengkap, Shot Map, **file JPG contact sheet asli per shot yang dapat diunduh secara individual**, catatan ketidakpastian, dan versi yang siap direview. Catat nama JPG, timestamp panel, dimensi, dan ukuran byte bila terukur agar pengguna dapat mengarsipkan **JPG yang sama** melalui repo lokal kapan saja. **Berhenti setelah Tahap 5** untuk menunggu umpan balik atau perintah simpan.
- **Larangan selama Fase 1:** tidak boleh menambah/mengubah/menghapus file GitHub, membuat `pending` baru, mengunggah JPG, memperbarui INDEX, membuat branch/commit/PR, atau mengubah status repo, **meskipun video baru belum ada dalam katalog**. Seluruh data Fase 1 adalah **draft lokal/percakapan**, bukan data yang sudah tersimpan pada repository.
- Pengguna boleh meminta revisi berulang. Perbarui **analisis dan contact sheet versi terbaru** sesuai bukti tanpa mengubah repository. **Review pengguna tidak otomatis membuat status `approved`**. Laporkan kesiapan Fase 1 secara deskriptif, **bukan** dengan Gate A/B/overall PASS.
- Pada Fase 1 **Gate A/B/overall berstatus `belum dijalankan`**. Evidence Cross-Check adalah pemeriksaan awal, **bukan** Dual Verification Gate resmi. Jika MP4 gagal dibaca, laporkan bahwa analisis belum bisa dilanjutkan; jangan mengarang dan jangan menulis status Gate resmi `FAIL` sebelum Fase 2.
- Usahakan tetap berada pada **chat yang sama** sampai disimpan: MP4, contact sheet, dan berkas sementara mungkin tidak bertahan pada sesi lain. Tidak boleh mengklaim artefak lokal tetap tersedia bila belum diperiksa.

**HUMAN REVIEW — STOP**: **`save now`** (tidak peka huruf besar/kecil) adalah perintah eksplisit untuk melewati batas menuju Fase 2 bagi **analisis video terakhir yang sedang direview dalam percakapan**. Kata umum seperti `lanjut`, `oke`, atau sekadar revisi **bukan** izin menyimpan. Jika ada beberapa video atau versi yang benar-benar ambigu, pastikan target sebelum menulis. Jika pengguna secara jelas meminta penyimpanan dengan kata lain, hormati instruksi eksplisitnya; jangan menafsirkan persetujuan umum sebagai izin.

**FASE 2 — Save & Verify (Tahap 6–7; Document-First Save)**

- **Pemicu:** `save now` atau perintah penyimpanan eksplisit setara setelah Fase 1. Gunakan **revisi analisis terakhir**, bukan draft lama.
- **Tahap 6:** simpan **hanya** `references/<creator>/analysis/<video-id>.md` (10 bagian lengkap, Shot Map, Contact Sheet Manifest) dan `references/INDEX.md` **langsung ke branch `main`**. Upayakan satu commit terkoordinasi. **Tidak membuat branch staging, PR, ZIP, atau mengunggah JPG.**
- **JPG sepenuhnya tanggung jawab pengguna:** pengguna menyimpan `shot-XX.jpg` melalui clone/repository lokal kapan saja. Manifest tetap memuat **nama/path baku JPG, timestamp dan dimensi** yang berasal dari Fase 1. **Ketiadaan JPG di GitHub tidak menunda penyimpanan analisis atau memengaruhi status Gate.** Path JPG berupa kode/lokasi arsip, bukan hyperlink aktif atau pernyataan bahwa file sudah ada di remote.
- **Keamanan commit langsung:** baca HEAD `main` dan konten file target/INDEX sebelum menulis; gunakan commit terkoordinasi dan pemeriksaan expected HEAD/lease tanpa force. Jika `main` berubah, hindari overwrite dan laporkan konflik. Setelah commit, baca ulang dokumen, INDEX, HEAD dan tautan Markdown **yang benar-benar ada**.
- **Tahap 7:** Gate A menguji akurasi analisis visual dari bukti Fase 1. Gate B menguji **integritas dokumen Markdown + INDEX dan commit di `main`**, **bukan** keberadaan, byte, SHA atau render JPG di GitHub.
- Jika Gate A dan B dokumen sama-sama **PASS**, **overall PASS** meskipun JPG belum dimasukkan pengguna. **Jangan menetapkan PARTIAL hanya karena JPG belum ada.** PASS berarti **analisis serta dokumen GitHub valid**, bukan bukti bahwa JPG sudah terunggah.
- Status hasil analisis AI tetap `draft` sampai pengguna secara eksplisit menyetujuinya; `save now` bukan `approved`.

### Pengelolaan JPG oleh pengguna (di luar penyimpanan AI)

- AI memberikan **JPG contact sheet asli yang dapat diunduh** pada Fase 1, dengan nama `shot-XX.jpg`, label timestamp dan susunan panel.
- AI **tidak mengunggah atau memverifikasi JPG di GitHub** pada Fase 2, serta tidak meminta pengguna upload lewat chat, tidak membuat ZIP, dan tidak menghalangi commit dokumen.
- Manifest final menyebut **lokasi arsip JPG standar**, misalnya `references/muyon/frames/muyon-02/shot-01.jpg` atau path relatif `../frames/muyon-02/shot-01.jpg` sebagai `code`, **tanpa tautan Markdown yang belum valid**. Saat pengguna menyalin JPG ke repo lokal dan melakukan push, path ini sudah cocok.
- Jangan membuat kolom `pending upload` untuk status analisis dan jangan mengarang bahwa JPG telah tersedia di remote. Ketiadaan file JPG saja **bukan** alasan Gate B PARTIAL/FAIL.

**Ringkasan:** `MP4 dari chat → Tahap 1–5 → review/revisi → STOP → "save now" → Tahap 6–7 → laporan Gate`.

### Tahap 1 — Video Input & Validation

- Tetapkan ID unik; periksa [INDEX](../references/INDEX.md) dan analisis sebelumnya. Gunakan MP4 yang **benar-benar dapat dibaca dari chat**; nama file atau metadata saja tidak membuktikan isi video.
- Catat nama input, tanggal pemeriksaan, durasi, FPS, resolusi, rasio aspek, ukuran byte/hash **jika tersedia**, serta cakupan yang berhasil diperiksa. **Jika berbeda, bedakan durasi kontainer, trek video, dan trek audio; jangan menghitung durasi gambar hanya dari durasi kontainer × FPS.** Jika **pengguna meminta analisis sekarang** tetapi input tidak dapat diakses, jangan mengarang temuan atau membuat frame palsu; nyatakan **Fase 1 belum dapat diselesaikan**. Gate A/B/overall **belum dijalankan** hingga perintah simpan dan proses verifikasi resmi. Dokumen administratif `pending` juga tetap memiliki Gate `belum dijalankan`.
- Audio: bedakan keberadaan audio track dari suara yang benar-benar didengar. Bila tidak diaudit, tulis `audio belum diperiksa`; tidak boleh mengarang audio.
- Jangan meminta upload ulang bila video sudah dapat diakses pada sesi ini.

### Tahap 2 — Video Structure Mapping (Pass 1)

- Telusuri **seluruh timeline** dengan sampling awal sekitar **0,5–1 detik** atau adaptif; deteksi jumlah shot kontinu, cut/dissolve, objek atau tempat yang berubah, dan bagian hitam.
- Periksa **lebih rapat** dekat batas transisi, bukan menebak batas presisi dari interval sampling. Susun **Shot Map** (ID, start–end, durasi, transisi, ketepatan waktu, cakupan), lalu periksa kembali pada Pass 2.
- Jika bagian video belum dapat diperiksa, sebutkan rentangnya; jangan menyatakan seluruh video telah ditinjau.

### Tahap 3 — Deep Shot Analysis (Pass 2)

- Periksa gerakan **MP4 asli** per shot: hero subject, tanaman/buah, susunan foreground/middle/background, kerapatan, bedengan/jalur/trellis/kolam, cuaca/cahaya, sumber air, hewan/manusia, aktivitas, transisi dan audio bila diperiksa.
- Jelaskan perkembangan **awal → tengah → akhir**, termasuk objek yang muncul/hilang dan perubahan komposisi. Bedakan pan, tilt, tracking, push-in, zoom dan gerakan objek; jika ambigu beri label `[INTERPRETASI]` atau `[BELUM PASTI]` plus tingkat keyakinan.
- Setiap klaim penting memiliki shot/timestamp dan dipisahkan menjadi `[OBSERVASI]`, `[KONTEKS PENGGUNA]`, `[INTERPRETASI]`, `[BELUM PASTI]`. Jangan menyamakan sprinkler/selang dengan hujan.

### Tahap 4 — Adaptive Per-Shot Contact Sheet

**Aturan utama: satu shot = satu JPG contact sheet `shot-XX.jpg`**, di `references/<creator>/frames/<video-id>/`. Setiap JPG berisi beberapa **panel frame sumber** berurutan, bukan JPG individual untuk setiap detik.

- **Target 3–6 panel per shot**, adaptif: shot pendek/statis boleh 2–3; shot panjang/kompleks bisa 6–10+ bila memang perlu. Jumlah **bukan kuota kaku**; satu shot satu JPG adalah format utama, dengan pengecualian `shot-XX-part-01.jpg` dll. hanya jika satu lembar terlalu padat untuk dibaca dan alasannya dicatat.
- Seleksi dari **awal, perkembangan, akhir**, serta perubahan kamera/objek/komposisi yang benar-benar informatif. Hindari hampir-duplikat, blur, dan frame di tengah dissolve (kecuali untuk bukti transisi).
- Urutkan panel menurut **timestamp sumber** dari kiri ke kanan, lalu atas ke bawah. Setiap panel diberi label waktu **di luar area gambar**, contoh `00:02.10`; layout enam panel vertikal lazimnya **3 kolom × 2 baris**.
- **Panel berasal dari MP4 asli**, tanpa generasi AI, upscale, perubahan objek, atau pemotongan yang menyesatkan. Pertahankan rasio aspek dan warna sumber. Target lebar tiap panel **480–720 px jika resolusi sumber/transfer memungkinkan** dan label mudah dibaca. **Target kualitas ini harus diuji, bukan diasumsikan berhasil**.
- **Perbedaan ukuran sumber vs contact sheet:** panel dapat diperkecil **secara wajar** dari resolusi frame asli untuk memenuhi target keterbacaan 480–720 px; ini tetap **`shot-XX.jpg` (contact sheet standar)** jika panel jelas, proporsi/isi tidak berubah, dan ukuran sumber, ukuran panel, serta kanvas dicatat. Contoh: sumber 720×1280 menjadi panel 540×960 **tidak otomatis** disebut preview. **Wajib gunakan `shot-XX-preview.jpg`** jika resolusi diturunkan **di bawah target keterbacaan** karena batas transfer/alat, atau hasil tidak cukup detail untuk analisis; catat penurunan mutu secara terbuka. Jangan meng-upscale atau mengklaim panel beresolusi sumber jika sudah diperkecil. Frame individual boleh dipakai **sementara secara lokal** tetapi tidak diunggah sebagai standar utama.
- **Contact Sheet Manifest** (satu baris per shot/JPG): Shot ID, **nama/path JPG standar**, semua timestamp panel, jumlah panel, dimensi kanvas/panel, kategori contact-sheet/preview, dan ukuran byte lokal bila tersedia. Path adalah **lokasi arsip yang ditetapkan pengguna**, bukan klaim file sudah terunggah. Tidak perlu SHA GitHub, status upload, atau verifikasi render remote. JPG diberikan pada Fase 1; dokumen Fase 2 cukup mencatat lokasinya.

### Tahap 5 — Evidence Cross-Check

- Cocokkan Shot Map, MP4 bergerak, laporan per shot, timestamp panel, contact sheet, dan tag. Pastikan semua shot penting tercakup, **perubahan awal–akhir benar**, serta klaim objek/gerakan sesuai bukti.
- Ambiguitas kamera diuji ulang melalui MP4, objek kecil melalui frame sumber resolusi lebih baik. Catat confidence; jangan menyimpulkan spesies/gerimis atau suara bila bukti tidak cukup.
- Bedakan `tidak terlihat`, `belum diperiksa`, dan `belum pasti`. Jangan menambah gambar AI atau tautan belum ada. **Setelah tahap ini, sajikan hasil untuk review, tunggu revisi atau `save now`, dan jangan menjalankan Tahap 6–7 tanpa izin.**

### Tahap 6 — Repository Save (hanya Markdown + INDEX)

**HANYA SETELAH `save now`/izin simpan eksplisit. AI tidak mengunggah JPG.**

- Simpan `references/<creator>/analysis/<id>.md` (10 bagian lengkap dengan Shot Map/Contact Sheet Manifest) dan `references/INDEX.md` **langsung ke `main`** dalam satu perubahan terkoordinasi.
- Tulis **nama/path baku JPG** di manifest tanpa menunggu file JPG hadir di GitHub; gunakan kode literal alih-alih hyperlink yang belum valid. Status analisis tidak bergantung pada JPG.
- Cek HEAD `main` sebelum commit; gunakan expected SHA/lease non-force. Sesudah commit, cek ulang HEAD, dokumen dan INDEX serta link Markdown yang benar-benar dibuat. Jika gagal, jangan mengklaim Gate B PASS.

### Tahap 7 — Dual Verification Gate (analisis dan dokumen)

**HANYA PADA FASE 2; selama Fase 1 Gate A/B/overall = `belum dijalankan`.**

**Gate A — Visual Accuracy** wajib memeriksa:
1. MP4 dan cakupan sumber benar-benar diperiksa; Pass 1 + Pass 2, Shot Map, serta batas ketidakpastian sudah dinyatakan.
2. Shot penting dan perubahan awal–tengah–akhir diwakili oleh hasil analisis dan panel JPG yang dibuat pada Fase 1.
3. Kamera, tanaman/buah, cuaca/air, aktivitas dan timestamp sesuai observasi; hal tak pasti diberi label.
4. Audio tidak dikarang jika tidak diperiksa.

**Gate B — Document & Repository Integrity** wajib memeriksa:
1. Dokumen Markdown **10 bagian** dan `references/INDEX.md` berhasil ditulis dan dibaca ulang pada **`main`**.
2. Shot Map, Contact Sheet Manifest, nama/path JPG, timestamp, metadata dan status katalog konsisten; tidak ada hyperlink Markdown yang dibuat namun rusak.
3. SHA commit dan HEAD `main` cocok; tidak menambahkan MP4. **File JPG bukan bagian pemeriksaan Gate B**, sebab pengguna mengelolanya sendiri melalui repo lokal.

**Hasil:** `belum dijalankan` selama Fase 1; `PASS` jika kriteria wajib masing-masing Gate terpenuhi; `PARTIAL` jika analisis/dokumen memiliki pemeriksaan yang belum selesai; `FAIL` bila sumber/isi direka atau dokumen gagal disimpan dengan benar. **Overall PASS** hanya jika Gate A dan B PASS, FAIL jika salah satu FAIL, selebihnya PARTIAL. **Tidak ada PARTIAL/FAIL karena JPG belum di-push.** `PASS` berarti **analisis dan penyimpanan dokumen berhasil**, bukan jaminan JPG tersedia di GitHub.

**Status terpisah dari Gate:** `pending` (belum dianalisis), `draft` (AI telah menganalisis tetapi belum disetujui), `reviewed` (ditinjau pengguna), `approved` (persetujuan **eksplisit** pengguna). Gate PASS **tidak membuat status otomatis approved**. INDEX adalah sumber status ringkas; README tidak menyalin angka status.

**Hak dan riwayat:** Repo publik tidak otomatis mengizinkan distribusi frame. MP4 yang dihapus dari tree Git masih mungkin ada dalam riwayat commit lama; pembersihan sejarah Git bukan bagian analisis rutin.

## 6. Pemeriksaan sebelum selesai

**Akhir Fase 1:** analisis + contact sheet lokal tersedia untuk review, **tanpa perubahan GitHub**. **Akhir Fase 2:** dokumen final dan INDEX di `main` diverifikasi, tanpa kewajiban unggah JPG.

- [ ] MP4/frame asli benar-benar diperiksa; tidak mengarang batas shot, gerak kamera, tanaman, cuaca, air atau audio.
- [ ] Shot Map Pass 1, Deep Shot Analysis Pass 2, bukti timestamp dan ketidakpastian lengkap.
- [ ] Fase 1 memberi **1 JPG contact sheet per shot** untuk pengguna, target panel 3–6 adaptif; STOP setelah Tahap 5.
- [ ] Fase 2 hanya setelah `save now`, memakai hasil review terbaru.
- [ ] Analisis **10 bagian** dan INDEX tersimpan **langsung di `main`**, dengan bukti commit/HEAD tanpa overwrite perubahan lain.
- [ ] Manifest memuat nama/path baku JPG, timestamp panel dan dimensi; tanpa tautan palsu atau klaim upload remote.
- [ ] Gate A untuk akurasi visual dan Gate B untuk **integritas dokumen**, overall konsisten.
- [ ] **Tidak perlu upload/cek JPG di GitHub; ketiadaannya bukan alasan PARTIAL.**
- [ ] Tidak menambah MP4 ke repo; status analisis/INDEX konsisten.
- [ ] Tidak membuat ide/prompt jika pengguna hanya meminta analisis.

**Prioritas utama: analisis yang jujur, terstruktur, dan bisa dilacak kembali ke referensi aslinya.**
