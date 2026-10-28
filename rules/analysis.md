# Aturan Analisis Video Referensi — Gardenku
**Versi:** 1.1 — Opsi B+ (Evidence-Driven + Per-Shot Contact Sheet)  
**Berlaku untuk:** `references/<creator>/analysis/<video-id>.md`  
**Tujuan:** Mengubah video asli menjadi catatan visual yang akurat dan bisa dipakai ulang oleh AI untuk mengembangkan konsep video kebun.

> Dokumen ini berisi **aturan kerja**, bukan hasil analisis video tertentu. Format berkas analisis baku tersedia di `templates/video-analysis.md`.

## 1. Kapan aturan ini digunakan?
Gunakan saat pengguna meminta AI menonton, mengamati, memecah shot, atau menganalisis **video referensi kebun**. **Jangan membuat ide atau prompt video** apabila pengguna hanya meminta analisis.

Baca `AGENTS.md`, lalu cek [INDEX](../references/INDEX.md) dan file analisis yang ada. Sumber video **selalu MP4 unggahan chat dari pengguna** (aslinya disimpan pengguna di PC). GitHub **tidak menyimpan MP4**; hanya analisis dan JPG ekstraksi. Contoh:
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
7. **MP4 asli disimpan di PC pengguna; jangan mengubah atau menghapus salinan pribadi.** Tidak perlu menyimpan/mengunggah MP4 ke GitHub. JPG yang diperoleh dengan ekstraksi tetap karya turunan dari video; periksa hak penggunaan saat repo publik.

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

**Metode:** Evidence-Driven Video Analysis + Adaptive Per-Shot Contact Sheet + Dual Verification Gate. MP4 **dikirim melalui chat dan disimpan pengguna di PC**, tidak diunggah ke GitHub. Repository hanya menyimpan analisis, JPG asli hasil ekstraksi (gabungan contact sheet), katalog, dan pengetahuan turunan. Bagian ini sumber **aturan baku**; AGENTS adalah navigasi dan template adalah format keluaran.

### Tahap 1 — Video Input & Validation

- Tetapkan ID unik; periksa [INDEX](../references/INDEX.md) dan analisis sebelumnya. Gunakan MP4 yang **benar-benar dapat dibaca dari chat**; nama file atau metadata saja tidak membuktikan isi video.
- Catat nama input, tanggal pemeriksaan, durasi, FPS, resolusi, rasio aspek, ukuran byte/hash **jika tersedia**, serta cakupan yang berhasil diperiksa. Jika input tidak bisa diakses, jangan mengarang temuan atau membuat frame palsu; Gate A menjadi `FAIL`.
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
- Jika terpaksa resolusi lebih kecil, nama wajib `shot-XX-preview.jpg`; cantumkan dimensi nyata dan dampaknya, jangan diam-diam menyebutnya kualitas penuh. Frame individual boleh dipakai **sementara secara lokal** untuk pemeriksaan, tetapi tidak diunggah sebagai standar utama.
- **Contact Sheet Manifest** (satu baris per shot/JPG): Shot ID, link JPG jika **benar-benar sudah ada**, **semua timestamp panel**, jumlah panel, dimensi kanvas dan panel, tipe contact-sheet/preview, SHA Git blob, byte, dan hasil verifikasi render/path. Jika belum diunggah, tulis `belum diunggah` **tanpa link palsu**.

### Tahap 5 — Evidence Cross-Check

- Cocokkan Shot Map, MP4 bergerak, laporan per shot, timestamp panel, contact sheet, dan tag. Pastikan semua shot penting tercakup, **perubahan awal–akhir benar**, serta klaim objek/gerakan sesuai bukti.
- Ambiguitas kamera diuji ulang melalui MP4, objek kecil melalui frame sumber resolusi lebih baik. Catat confidence; jangan menyimpulkan spesies/gerimis atau suara bila bukti tidak cukup.
- Bedakan `tidak terlihat`, `belum diperiksa`, dan `belum pasti`. Jangan menambah gambar AI atau tautan belum ada.

### Tahap 6 — Repository Save

- Siapkan `analysis/<id>.md` dengan **10 bagian template + Shot Map + Contact Sheet Manifest**, JPG terverifikasi, dan baris INDEX yang konsisten. Usahakan **satu commit terkoordinasi** pada branch yang disetujui pengguna.
- Kirim JPG sebagai **Git blob biner** (contoh Base64 dengan `encoding: base64`, bukan teks Base64 bernama JPG). **Sebelum commit:** uji format JPEG/dimensi/render lokal, cocokkan SHA Git blob sumber dengan SHA hasil upload, byte dan path. Jika berbeda, **jangan commit**.
- **Sesudah push:** periksa HEAD, tree, link Markdown, resolusi, jumlah gambar/panel, status INDEX, dan bahwa **tidak ada MP4 dalam tree repo**. Jika render jarak jauh tidak dapat diperiksa, nyatakan batasannya.
- Jangan hapus **legacy preview** sebelum contact sheet pengganti **terunggah dan diverifikasi**. Bila transfer gambar berkualitas tinggi gagal, simpan JPG lokal untuk pengguna dan tandai `belum diunggah` di manifest; **jangan mengklaim Gate B PASS**.

### Tahap 7 — Dual Verification Gate

**Gate A — Visual Accuracy** wajib memeriksa:
1. Sumber MP4 dan cakupan video benar-benar diperiksa, Pass 1 + Pass 2 serta Shot Map lengkap/ketidaklengkapannya dinyatakan.
2. Shot penting terwakili dan panel memperlihatkan perubahan signifikan, berurutan dengan timestamp yang benar.
3. Setiap klaim, kamera, buah/tanaman, cuaca/air, dan aktivitas memiliki bukti shot/timestamp serta confidence saat tidak pasti.
4. Audio dinyatakan sesuai cakupan (tidak otomatis gagal bila audio di luar permintaan analisis visual, tetapi tidak mengarang suara).

**Gate B — Repository Integrity** wajib memeriksa:
1. Contact sheet JPG **valid dan terbaca** dengan panel/timestamp sesuai Manifest, rasio/dimensi memadai; file dari MP4 asli, bukan gambar AI.
2. SHA Git blob, byte, path, jumlah file/panel, tautan, commit dan branch HEAD benar. Bila render pada GitHub tak dapat diperiksa, batasan dilaporkan.
3. Analisis **10 bagian**, Shot Map/Manifest dan INDEX konsisten; tidak ada MP4 di tree. Penggantian legacy JPG tidak menyisakan link rusak.

**Hasil:** `PASS` bila kriteria wajib sesuai cakupan terpenuhi; `PARTIAL` bila pemeriksaan/unggah/coverage masih kurang tetapi data yang ada valid; `FAIL` bila sumber tak bisa diperiksa, isi direka, gambar salah/rusak atau keberhasilan penyimpanan tidak dapat dipastikan. **Overall**: `PASS` hanya jika A dan B PASS; `FAIL` jika salah satu FAIL; sisanya `PARTIAL`. Simpan A/B/overall, alasan, dan bukti commit.

**Status terpisah dari Gate:** `pending` (belum dianalisis), `draft` (AI telah menganalisis tetapi belum disetujui), `reviewed` (ditinjau pengguna), `approved` (persetujuan **eksplisit** pengguna). Gate PASS **tidak membuat status otomatis approved**. INDEX adalah sumber status ringkas; README tidak menyalin angka status.

**Hak dan riwayat:** Repo publik tidak otomatis mengizinkan distribusi frame. MP4 yang dihapus dari tree Git masih mungkin ada dalam riwayat commit lama; pembersihan sejarah Git bukan bagian analisis rutin.

## 6. Pemeriksaan sebelum selesai
- [ ] Benar-benar mengakses video/frame asli, atau dengan jelas melaporkan jika tidak bisa.
- [ ] Setiap shot memiliki perkiraan timestamp, subjek, kamera, komposisi, dan layout.
- [ ] Cuaca, sumber air, manusia, hewan, suara dicatat sesuai bukti atau sebagai belum pasti/tidak terlihat.
- [ ] Ada ciri visual dan pelajaran yang bisa digunakan ulang.
- [ ] Sumber MP4 unggahan chat dan cakupan pemeriksaan dicatat; **tidak ada kewajiban MP4 di GitHub**.
- [ ] Shot Map (Pass 1) dan Deep Shot Analysis (Pass 2) mencakup video atau gap dicatat.
- [ ] Satu contact sheet JPG per shot berisi panel kronologis yang informatif dan label timestamp terbaca.
- [ ] Manifest memuat semua timestamp panel, dimensi, SHA Git blob, byte, path dan status upload nyata.
- [ ] Evidence Cross-Check memeriksa gerak kamera, objek, sumber air, dan perubahan visual terhadap MP4.
- [ ] Gate A Visual Accuracy dan Gate B Repository Integrity masing-masing dinyatakan PASS / PARTIAL / FAIL dan overall konsisten.
- [ ] Tidak ada MP4 di repo; INDEX/status/link cocok dan tidak ada klaim JPG yang belum diunggah.
- [ ] Tidak membuat ide maupun prompt sebelum diminta.

**Prioritas utama: analisis yang jujur, terstruktur, dan bisa dilacak kembali ke referensi aslinya.**
