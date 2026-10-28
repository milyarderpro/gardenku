# Aturan Analisis Video Referensi — Gardenku
**Versi:** 1.1  
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



## 5. Workflow Chat → Analisis → JPG → Repository

### A. Terima dan periksa MP4 dari chat

1. Tentukan ID referensi unik dan cek [INDEX](../references/INDEX.md) serta file analisis lama. MP4 asli **disimpan di PC pengguna**, bukan di repo. Unggahan chat dapat dipakai sebagai bukti hanya jika kontennya benar-benar bisa diperiksa.
2. Jika file belum tersedia atau tidak bisa dibaca, **jangan mengarang isi video**. Jelaskan batas akses, pertahankan status `pending` untuk referensi baru, dan jangan membuat frame palsu. Tidak perlu meminta video lagi bila sudah tersedia dan dapat diakses dalam sesi itu.
3. Catat nama input MP4 dan, bila terverifikasi, durasi, FPS, resolusi, ukuran byte atau checksum file. **Jangan mewajibkan pencocokan SHA dengan GitHub**, sebab MP4 memang tidak lagi ada di repo. Catat URL asli dan izin publikasi hanya jika diketahui.
4. Periksa video shot demi shot. Timestamp dan batas transisi yang belum presisi harus ditandai sebagai **perkiraan**. Jika hanya sebagian video terlihat, sebut bagian yang belum diperiksa. Metadata/codec/track audio **bukan bukti bahwa suara telah didengarkan**; tulis `audio belum diperiksa` bila perlu.
5. Siapkan file analisis memakai [template](../templates/video-analysis.md) dengan pemisahan `[OBSERVASI]`, `[KONTEKS PENGGUNA]`, `[INTERPRETASI]`, dan `[BELUM PASTI]`. Jangan membuat ide atau prompt jika hanya diminta analisis.

### B. Pilih dan ekstrak frame JPG

- **Default 2–3 JPG representatif per video**, biasanya dari shot yang berbeda; **bukan 2–3 JPG untuk setiap shot**. Jika video hanya memuat satu shot, satu frame boleh cukup; lebih dari tiga diperbolehkan bila perlu membuktikan beberapa momen atau pengguna meminta. Catat jika shot penting belum terwakili.
- Frame **harus diekstrak dari MP4 asli yang diperiksa**, bukan gambar AI, storyboard, atau hasil pencarian internet. Pilih momen yang jelas dan tidak sedang blur/transisi.
- Prioritaskan **resolusi asli dan rasio aspek yang sama**; tanpa upscale atau mempercantik gambar sehingga berubah dari bukti. Jika terpaksa mengecilkan untuk transfer, gunakan akhiran `-preview.jpg` dan tulis resolusi sesungguhnya; jangan menyebut preview sebagai frame resolusi penuh.
- Nama: `frames/<id>/shot-01_2.1s.jpg` atau `shot-01_2.1s-preview.jpg`; nomor shot dan timestamp merujuk **video sumber**. Hindari JPG duplikat yang tidak menambah informasi.
- **Frame Manifest** harus memuat shot, timestamp, path JPG, resolusi hasil unggahan, tipe (`original-resolution` / `preview`), dan hasil verifikasi. JPG yang belum diunggah dicatat sebagai `belum diunggah` **tanpa tautan palsu**.

### C. Simpan dokumen dan JPG di GitHub

1. Siapkan hasil analisis terlebih dahulu. Upload frame JPG yang dipilih dengan fitur GitHub binary blob/Base64 bila tersedia. Input `encoding: base64` mengirim **isi JPEG biner**, bukan teks Base64 yang salah diberi nama `.jpg`.
2. Cocokkan **SHA Git blob** hasil upload dengan SHA Git blob dari file lokal yang benar (hash Git blob, bukan SHA-256 biasa). Cek ukuran byte JPEG, path/nama file, dan tipe file/kemampuan membuka JPEG secara lokal. **Jika tidak cocok, jangan masukkan blob itu ke commit.**
3. Bangun tree/commit yang memuat file `analysis/<id>.md`, JPG yang lolos verifikasi, dan baris `references/INDEX.md` yang diperbarui, **sebisa mungkin dalam satu commit terkoordinasi**. Tidak boleh menautkan JPG yang belum tersedia. Jangan mengunggah MP4 ke repo.
4. Push ke branch yang disetujui pengguna. Verifikasi ulang branch HEAD, jumlah berkas, SHA/byte/path JPG, tautan relatif, status INDEX vs analisis, serta kelengkapan 10 bagian template. Jika dapat mengakses tampilan gambar GitHub, cek gambar ter-render; bila konektor hanya mendukung metadata biner, nyatakan keterbatasan itu.
5. Jika sebagian upload JPG gagal, jangan mencatat seolah seluruh gambar berhasil. Simpan hanya JPG yang terbukti valid; tandai yang belum tersimpan di manifest, dan laporkan apa yang perlu diperbaiki. **Jangan mengubah status menjadi `approved` dengan sendirinya.**

### D. Verification Gate dan arti status

**Gate dijalankan terakhir**, setelah push ke GitHub. Catat hasilnya dalam bagian Quality Checklist dan ringkas pada laporan pengguna.

| Hasil Gate | Syarat |
|---|---|
| **PASS** | Video benar-benar diperiksa; analisis 10 bagian dan shot/timestamp berbasis bukti; target frame yang dipilih tersedia atau pengecualian jumlah dijelaskan; JPG lolos pemeriksaan biner dan path; tautan & INDEX konsisten; commit/HEAD terverifikasi; keterbatasan audio/cuaca dicatat; **tidak ada MP4 di repo** |
| **PARTIAL** | Analisis valid tetapi ada frame pilihan gagal diunggah, pemeriksaan biner/link/commit belum lengkap, atau ada aspek penting yang harus dikoreksi; kekurangannya disebut spesifik |
| **FAIL** | Isi sumber tidak dapat diperiksa, data dikarang, file salah/rusak, atau tidak dapat memastikan hasil tersimpan. Jangan mengklaim proses telah berhasil |

**Status analisis berbeda dari hasil Gate:**
- `pending`: video belum diperiksa secara memadai.
- `draft`: AI telah memeriksa bukti dan menulis analisis; **belum disetujui pengguna**. Status ini masih mungkin memiliki Gate `PARTIAL` jika upload JPG belum lengkap.
- `reviewed`: ditinjau pengguna, tetapi mungkin masih perlu koreksi.
- `approved`: **disetujui jelas oleh pengguna** untuk menjadi rujukan gaya dan ide; AI tidak boleh menaikkan sendiri.

**Lokasi informasi utama:** `analysis/<id>.md` memuat bukti, sumber MP4 chat, timestamp, Frame Manifest, dan hasil Gate; [INDEX](../references/INDEX.md) memuat metadata dan **status terbaru per ID**. README adalah petunjuk tetap—**jangan duplikasi jumlah video, status, atau frame**. Prosedur ini berlaku juga ketika sebagian tahap gagal: laporkan hasil sebenarnya tanpa memaksakan PASS.

**Izin dan jejak historis:** repo publik bukan izin redistribusi JPG. **Menghapus MP4 dari tree/branch tidak menghapus objeknya dari commit Git lama.** Pengubahan riwayat Git untuk menghapus objek lama memerlukan proyek tersendiri dan tidak menjadi bagian analisis rutin.

## 6. Pemeriksaan sebelum selesai
- [ ] Benar-benar mengakses video/frame asli, atau dengan jelas melaporkan jika tidak bisa.
- [ ] Setiap shot memiliki perkiraan timestamp, subjek, kamera, komposisi, dan layout.
- [ ] Cuaca, sumber air, manusia, hewan, suara dicatat sesuai bukti atau sebagai belum pasti/tidak terlihat.
- [ ] Ada ciri visual dan pelajaran yang bisa digunakan ulang.
- [ ] Sumber MP4 unggahan chat dan cakupan pemeriksaan dicatat; **tidak ada kewajiban MP4 di GitHub**.
- [ ] Frame Manifest hanya menautkan JPG yang ada, dengan timestamp, resolusi sebenarnya, tipe preview/original dan bukti verifikasi.
- [ ] SHA Git blob/byte/path JPG, tautan, commit, dan branch HEAD diverifikasi; kekurangan dinyatakan.
- [ ] Status analisis dan `references/INDEX.md` sama; README tidak memuat status paralel.
- [ ] Hasil **Verification Gate: PASS / PARTIAL / FAIL** dicatat dan dijelaskan; video MP4 tidak ikut tersimpan di repo.
- [ ] Tidak membuat ide maupun prompt sebelum diminta.

**Prioritas utama: analisis yang jujur, terstruktur, dan bisa dilacak kembali ke referensi aslinya.**
