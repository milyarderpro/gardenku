# Panduan AI — Gardenku

## Tujuan

Gunakan repository ini sebagai **pustaka referensi video kebun**: pelajari karakter visual video, kembangkan ide baru, dan susun prompt video saat diminta.

## Prinsip utama

1. Gunakan **bahasa Indonesia** untuk analisis, ide, dan prompt; istilah teknis videografi boleh berbahasa Inggris.
2. **Jangan mengarang** isi video, jenis tanaman, jumlah shot, cuaca, suara, atau objek yang belum terlihat/terverifikasi.
3. Bedakan **observasi video**, **informasi dari pengguna**, dan **interpretasi AI**.
4. Bedakan **shot** (rekaman kontinu), **scene** (kesatuan adegan), dan **clip** (segmen video digital).
5. Bila pengguna meminta **analisis saja**, jangan langsung membuat ide atau prompt.
6. Manusia, ayam, bebek, ikan, kolam, gerimis, atau objek lain adalah unsur **opsional**; catat jika memang terlihat dan relevan.
7. Pembuatan video baru biasanya memakai **2–3 prompt independen**, masing-masing untuk **satu continuous shot sekitar 8 detik**, kecuali pengguna meminta ketentuan berbeda. Jangan memaksakan gerak kamera maju terus.
8. Jangan mengubah atau menghapus video asli tanpa instruksi eksplisit.

## Lokasi informasi

- **Aturan analisis:** `rules/analysis.md`.
- **Aturan ide:** `rules/ideas.md`.
- **Aturan prompt:** `rules/prompts.md`.
- **Template:** `templates/video-analysis.md`, `templates/video-concept.md`, dan `templates/video-prompt.md`.
- **Koleksi referensi:** `references/<creator>/`.
- **Katalog referensi:** `references/INDEX.md` (akan dibuat pada tahap berikutnya).
- **Gaya visual:** `styles/` (setelah tersedia analisis referensi).
- **Produksi ide dan prompt:** `projects/`.

Ketika file aturan atau template **belum ada**, jangan berpura-pura telah membacanya. Laporkan keterbatasannya dan gunakan konteks yang memang tersedia.

## Penamaan file

Pada setiap kreator, gunakan satu ID video yang sama untuk semua bahan:

- `videos/muyon-01.mp4`
- `analysis/muyon-01.md`
- `frames/muyon-01/`

Indeks harus menunjuk ke dokumen analisis yang benar. Jangan menandai analisis sebagai selesai sebelum video diperiksa.

## Status saat ini

**Tahap 1–4 selesai di branch kerja.** Enam belas video Muyon sudah berada di `references/muyon/videos/`; 16 kerangka `references/muyon/analysis/` masih `pending`. Frame JPG belum diekstrak. Master prompt lama tetap di `prompt/mp-v01.md`. Jangan menyimpulkan video sudah dianalisis hanya dari keberadaan file kerangka.

Lihat `README.md` untuk gambaran proyek dan status pekerjaan.
