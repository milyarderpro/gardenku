# Aturan Analisis Video Referensi — Gardenku
**Versi:** 1.1  
**Berlaku untuk:** `references/<creator>/analysis/<video-id>.md`  
**Tujuan:** Mengubah video asli menjadi catatan visual yang akurat dan bisa dipakai ulang oleh AI untuk mengembangkan konsep video kebun.

> Dokumen ini berisi **aturan kerja**, bukan hasil analisis video tertentu. Format berkas analisis baku tersedia di `templates/video-analysis.md`.

## 1. Kapan aturan ini digunakan?
Gunakan saat pengguna meminta AI menonton, mengamati, memecah shot, atau menganalisis **video referensi kebun**. **Jangan membuat ide atau prompt video** apabila pengguna hanya meminta analisis.

Baca `AGENTS.md`, lalu periksa media dan analisis yang tersedia untuk referensi tersebut. Contoh setelah migrasi:
- Video: `references/muyon/videos/muyon-01.mp4`
- Analisis: `references/muyon/analysis/muyon-01.md`
- Frame asli: `references/muyon/frames/muyon-01/`

Video Muyon berada di `references/muyon/videos/`. **Status terbaru** setiap video diperiksa melalui [`references/INDEX.md`](../references/INDEX.md) dan berkas analisis terkait; jangan menganggap semua video sudah atau belum dianalisis hanya dari nama folder.

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
7. **Video asli tidak boleh diedit, diganti, atau dihapus** hanya untuk melakukan analisis.

## 3. Urutan analisis

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

**Perbedaan gerak kamera:** pan = kamera berputar kiri/kanan; tilt = berputar atas/bawah; tracking = kamera berpindah posisi menyamping; push-in = posisi kamera mendekati objek; zoom = pembesaran optik/digital. Jangan menyebut semua gerak sebagai "kamera maju".

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


## 5. Workflow dari video sampai GitHub

### A. Terima dan cocokkan sumber

1. Mulai dari ID yang benar (misalnya `muyon-01`) dan cek [katalog](../references/INDEX.md), MP4 di repo, serta analisis yang sudah ada. **Jangan menimpa analisis terverifikasi tanpa memeriksa isi sebelumnya.**
2. Coba baca media asli. Jika konektor GitHub hanya menampilkan metadata atau menolak MP4 biner, gunakan **MP4 yang pengguna unggah ke chat** untuk pemeriksaan visual. **Tautan GitHub atau metadata bukan bukti bahwa video sudah ditonton.**
3. Bila sumber unggahan chat diklaim sama dengan MP4 repo, cocokan **ukuran byte dan SHA blob Git** bila alat mendukung. Catat hasilnya dalam analisis. Bila tidak bisa dicocokkan, tulis "belum terverifikasi"; jangan mengklaim keduanya identik. Jangan mengganti MP4 di repo hanya karena nama mirip.
4. Periksa durasi, resolusi, FPS, rasio aspek, urutan shot dan batas transisi dari sumber yang benar-benar tersedia. Beri label "perkiraan" jika batas shot tidak diukur frame demi frame. Bila hanya sebagian video bisa diperiksa, tulis **cakupan pemeriksaan** serta bagian yang belum bisa diamati.
5. **Audio terpisah dari metadata:** keberadaan audio track atau codec bukan bukti bahwa isi suaranya telah didengarkan. Catat "audio belum diperiksa" jika belum ada pemeriksaan auditori.

### B. Ekstrak frame JPG representatif

- **Default 2–3 JPG per video**, pilih frame yang berbeda dan paling informatif (biasanya dari shot berbeda). Ini target praktis, **bukan kuota wajib**: untuk 1 shot cukup 1 frame jika memadai; lebih dari 3 diperbolehkan jika dibutuhkan sebagai bukti atau diminta pengguna. Jika ada shot penting belum terwakili, catat secara jujur.
- **Utamakan resolusi video asli**, tanpa upscale atau generasi AI. Bila batas transfer memaksa ukuran lebih kecil, beri akhiran `-preview.jpg`; simpan **resolusi hasil upload yang sebenarnya**, bukan mengaku file resolusi penuh. Kompresi JPG masih berasal dari frame video asli, tetapi disebut **turunan/preview** bila diperkecil.
- Penamaan: `references/<creator>/frames/<id>/shot-01_2.1s.jpg` untuk frame sesuai resolusi sumber; `shot-01_2.1s-preview.jpg` untuk versi kecil. Gunakan `<shot-number>` dan timestamp **video referensi asli**, konsisten dengan Shot Breakdown. Hindari duplikat frame tanpa manfaat.
- **Tidak boleh** menaruh gambar generatif, ilustrasi, ataupun storyboard AI di folder `references/.../frames/`. Jangan memakai hasil pencarian gambar internet sebagai pengganti frame MP4.
- Setiap frame yang **berhasil tersimpan** harus terdaftar dalam **Frame Manifest** pada berkas analisis: shot, timestamp, path, resolusi unggahan, kategori `original-resolution` / `preview`, dan status verifikasi. Untuk frame yang gagal diunggah, tulis "belum diunggah", **tanpa tautan file yang tidak ada**.

### C. Upload dan pemeriksaan GitHub

Jika pengguna meminta menyimpan ke repo:

1. Siapkan `analysis/<id>.md` dari [template](../templates/video-analysis.md), lalu pilih frame yang benar-benar diekstrak.
2. Untuk konektor GitHub yang mendukungnya, unggah JPG biner sebagai **Git blob Base64** (mis. `create_blob` dengan `encoding: base64`), kemudian pasang SHA blob itu sebagai file JPG di `frames/<id>/` melalui tree/commit. **Jangan** memasukkan teks Base64 sebagai isi file `.jpg`.
3. **Verifikasi sebelum commit:** bandingkan SHA **Git blob** hasil unggah dengan SHA Git blob file lokal yang dikalkulasi dengan format Git (bukan SHA-256 biasa); periksa ukuran byte serta path dalam tree kandidat. Jika SHA/ukuran tidak cocok, **jangan commit** gambar itu. Perbaiki transfer atau laporkan kegagalan.
4. Commit pada **branch yang disetujui pengguna**; untuk perubahan aturan/template gunakan branch terpisah dan Pull Request sebelum merge. Sesudah push, periksa kembali SHA/path/ukuran di tree GitHub serta semua tautan Markdown yang dibuat. Bila memungkinkan, buka tampilan JPG agar gambar dapat dipastikan ter-render; jika tak bisa dibaca melalui konektor, nyatakan batas verifikasinya.
5. Jangan mengubah MP4 asli. Jika sebagian JPG gagal, **jangan mengklaim seluruh frame selesai**. Simpan yang sudah terverifikasi, tandai sisanya secara jujur, dan jangan buat link palsu.

**Perizinan:** repository publik bukan bukti izin mendistribusikan video atau frame. Catat sumber/izin yang diketahui, dan minta peninjauan hak penggunaan sebelum penyebaran lebih luas.

### D. Status dan sumber informasi utama

- `pending`: belum ada pemeriksaan visual memadai; jangan mengarang hasil.
- `draft`: ada hasil analisis AI dari bukti yang benar-benar diperiksa, **belum ditinjau pengguna**. Kekurangan audio atau frame masih boleh ada bila **dinyatakan dengan jelas**, tidak disamarkan.
- `reviewed`: sudah ditinjau dan masih bisa memerlukan koreksi.
- `approved`: disetujui eksplisit oleh pengguna untuk menjadi sumber referensi gaya/ide. **AI tidak boleh menaikkan sendiri status ke `approved`.**

**Satu sumber utama per jenis informasi:**
- **Analisis per video:** sumber utama bukti, shot, timestamp, ketidakpastian, **Frame Manifest**, dan status kerja pada file tersebut.
- **`references/INDEX.md`:** katalog utama yang menampilkan **status dan metadata ringkas** setiap video. Bila status/metadata berubah, sinkronkan baris INDEX pada commit yang sama.
- **README folder dan `styles/README.md`:** petunjuk penggunaan yang relatif tetap. **Jangan mengulang angka `draft`/`pending` atau jumlah JPG yang cepat berubah** di banyak README.
- Profile `styles/` baru boleh menyimpulkan pola berdasarkan bukti; utamakan analisis `approved`.

Laporan hasil harus membedakan **"analisis selesai"**, **"frame tersimpan"**, dan **"sudah ditinjau/disetujui"** sebagai tiga hal terpisah.

## 6. Pemeriksaan sebelum selesai
- [ ] Benar-benar mengakses video/frame asli, atau dengan jelas melaporkan jika tidak bisa.
- [ ] Setiap shot memiliki perkiraan timestamp, subjek, kamera, komposisi, dan layout.
- [ ] Cuaca, sumber air, manusia, hewan, suara dicatat sesuai bukti atau sebagai belum pasti/tidak terlihat.
- [ ] Ada ciri visual dan pelajaran yang bisa digunakan ulang.
- [ ] Metadata MP4 atau kecocokan sumber chat–repo diverifikasi, atau keterbatasan dinyatakan.
- [ ] Frame Manifest hanya menautkan JPG yang ada, dengan timestamp, resolusi sebenarnya, tipe preview/original dan status verifikasi.
- [ ] Bila upload diminta, SHA Git blob, byte, path, commit, dan tautan GitHub diperiksa; kegagalan dilaporkan apa adanya.
- [ ] Status pada berkas analisis dan `references/INDEX.md` konsisten; README tidak menjadi daftar status paralel.
- [ ] Tidak membuat ide maupun prompt sebelum diminta.

**Prioritas utama: analisis yang jujur, terstruktur, dan bisa dilacak kembali ke referensi aslinya.**
