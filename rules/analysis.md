# Aturan Analisis Video Referensi — Gardenku
**Versi:** 1.0  
**Berlaku untuk:** `references/<creator>/analysis/<video-id>.md`  
**Tujuan:** Mengubah video asli menjadi catatan visual yang akurat dan bisa dipakai ulang oleh AI untuk mengembangkan konsep video kebun.

> Dokumen ini berisi **aturan kerja**, bukan hasil analisis video tertentu. Format berkas analisis baku akan berada di `templates/video-analysis.md` (Tahap 3).

## 1. Kapan aturan ini digunakan?
Gunakan saat pengguna meminta AI menonton, mengamati, memecah shot, atau menganalisis **video referensi kebun**. **Jangan membuat ide atau prompt video** apabila pengguna hanya meminta analisis.

Baca `AGENTS.md`, lalu periksa media dan analisis yang tersedia untuk referensi tersebut. Contoh setelah migrasi:
- Video: `references/muyon/videos/muyon-01.mp4`
- Analisis: `references/muyon/analysis/muyon-01.md`
- Frame asli: `references/muyon/frames/muyon-01/`

**Setelah migrasi Tahap 4**, video Muyon berada di `references/muyon/videos/`. Namun dokumen analisis awal berstatus `pending`; jangan menganggap isinya sudah dianalisis.

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

## 5. File, frames, dan status
- Gunakan nama ID yang sama: `muyon-01.mp4`, `muyon-01.md`, dan `frames/muyon-01/`.
- Frame JPG **harus berasal dari video asli**, disertai timestamp bila memungkinkan. Gambar yang dibuat AI adalah ilustrasi/storyboard, **bukan** frame referensi asli.
- Tautkan analisis ke lokasi video dan frame yang benar. Jika file masih berada di lokasi lama, gunakan path aktual saat itu.
- Status yang diperbolehkan:
  - `pending`: belum dianalisis.
  - `draft`: sudah dianalisis AI, belum diperiksa.
  - `reviewed`: sudah diperiksa tetapi mungkin masih perlu koreksi.
  - `approved`: disetujui untuk menjadi acuan pustaka gaya dan ide.
- Jangan menandai `approved` sendiri tanpa persetujuan yang jelas.

## 6. Pemeriksaan sebelum selesai
- [ ] Benar-benar mengakses video/frame asli, atau dengan jelas melaporkan jika tidak bisa.
- [ ] Setiap shot memiliki perkiraan timestamp, subjek, kamera, komposisi, dan layout.
- [ ] Cuaca, sumber air, manusia, hewan, suara dicatat sesuai bukti atau sebagai belum pasti/tidak terlihat.
- [ ] Ada ciri visual dan pelajaran yang bisa digunakan ulang.
- [ ] Nama, path, tautan frame, dan status analisis konsisten.
- [ ] Tidak membuat ide maupun prompt sebelum diminta.

**Prioritas utama: analisis yang jujur, terstruktur, dan bisa dilacak kembali ke referensi aslinya.**
