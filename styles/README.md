# Style Library — Gardenku

Folder ini merupakan **perpustakaan rangkuman gaya visual** yang diambil dari hasil analisis referensi. Berbeda dari `references/` yang menyimpan video dan catatan per video, `styles/` merangkum **pola yang dapat diterapkan ulang** untuk membuat konsep baru.

**Status saat ini: belum ada style profile yang terverifikasi.** Seluruh 16 dokumen analisis Muyon masih `pending`. Oleh karena itu, **jangan membuat klaim** bahwa semua video Muyon merupakan kebun terbuka, selalu hujan, atau menggunakan slow pan.

## Apa yang dapat menjadi style profile?

Profile sebaiknya memiliki **satu fokus yang jelas** dan memakai nama file Inggris lowercase-kebab-case:

| Aspek | Contoh nama di masa depan | Yang dirangkum |
|---|---|---|
| Jenis / skala kebun | `open-field.md`, `front-yard.md` | Ukuran relatif, bedengan, pot, trellis, hubungan rumah/jalan, kepadatan tanaman |
| Cuaca / atmosfer | `after-rain.md`, `morning-light.md` | Cahaya, basahnya daun/tanah, genangan, gerimis alami, mood |
| Gaya kamera | `slow-pan.md`, `lateral-tracking.md` | Framing, movement, focal point, kecepatan, ritme shot |
| Penataan visual spesifik | `fruit-closeups.md` | Cara buah/tanaman dijadikan hero subject dan mengisi foreground/middle/background |

Ini **contoh nama file**, bukan profile yang sudah dianalisis atau dibuat.

## Alur pembuatan style profile

1. Cari referensi di [`references/INDEX.md`](../references/INDEX.md).
2. Baca file analisis dan, bila perlu, video/frame aslinya; utamakan `approved`.
3. Temukan ciri yang **benar-benar berulang atau sengaja menjadi fokus**. Jangan menyimpulkan sebuah pola dari label kreator saja.
4. Tulis kesimpulan dan **sertakan bukti** berupa ID video, nomor shot, dan timestamp; pisahkan observasi dari interpretasi.
5. Beri status `draft` sampai dilakukan peninjauan; **jangan menetapkan `approved` tanpa persetujuan jelas**.
6. Saat profile sudah layak, gunakan sebagai panduan ide bersama `rules/ideas.md` dan sebagai panduan prompt bersama `rules/prompts.md`. Detail setiap referensi tetap menjadi sumber utama.

## Kerangka untuk profile gaya baru

Salin kerangka berikut ke berkas baru **hanya setelah memiliki referensi yang relevan**:

```markdown
# Style Profile — [Nama Gaya]

- Status: draft
- Fokus: [jenis kebun / cuaca / kamera / elemen visual]
- Terakhir ditinjau: [tanggal atau belum]

## Deskripsi Singkat
[Kesimpulan berbasis bukti, bukan daftar harapan.]

## Ciri Visual
- [Ciri utama + kondisi kapan berlaku]
- [...]

## Camera & Composition
- [Movement, framing, visual hook, ritme]

## Garden Layout & Atmosphere
- [Penataan tanaman, struktur, cahaya, cuaca jika relevan]

## Supporting References
| ID video | Shot / timestamp | Bukti yang mendukung |
|---|---|---|
| [id] | [shot & waktu] | [temuan terverifikasi] |

## Creative Adaptation
- [Hal yang dapat diadaptasi untuk konsep baru]
- [Hal yang jangan dipaksakan, misalnya kolam di pekarangan sempit]

## Uncertainty
- [Keterbatasan, data yang belum diperiksa]
```

## Prinsip penjagaan kualitas

- **Tidak ada style universal untuk semua kreator.** Satu kreator bisa mempunyai kebun terbuka, front yard, atau konsep lain.
- **Jenis kebun berbeda dari cuaca dan gerakan kamera.** Sebuah front yard bisa bernuansa selepas hujan dengan slow pan.
- Manusia, ayam, bebek, ikan, dan kolam **opsional**; jangan menjadikannya elemen wajib tanpa dasar.
- **Jangan menganggap gambar storyboard AI sebagai frame video asli.**
- Jika hasil analisis direvisi, evaluasi ulang profile yang merujuk kepadanya.
- Simpan pengetahuan di file, tetapi ingat AI harus diberi akses dan membaca file itu; ini **bukan pelatihan ulang model**.
