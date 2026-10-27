# Gardenku

Gardenku adalah pustaka referensi video kebun untuk membantu AI **menganalisis video**, **mempelajari gaya visual**, **mengembangkan ide baru**, dan **menyusun prompt video per shot**.

Dokumen ditulis dalam **bahasa Indonesia**; nama folder dan file teknis memakai **bahasa Inggris**.

## Struktur pustaka

| Lokasi | Fungsi |
|---|---|
| `AGENTS.md` | Petunjuk bagi AI yang bekerja dengan repository ini |
| `rules/` | Aturan analisis referensi, pembuatan ide, dan penulisan prompt (selesai Tahap 2) |
| `templates/` | Format dokumen standar (selesai Tahap 3) |
| `references/` | Referensi yang dikelompokkan menurut sumber/kreator; [katalog utama](references/INDEX.md) |
| `references/<creator>/videos/` | Video asli dari kreator tersebut |
| `references/<creator>/analysis/` | Hasil analisis setiap video |
| `references/<creator>/frames/` | Gambar frame asli yang diekstrak dari video |
| `styles/` | [Style Library](styles/README.md): rangkuman berbasis analisis yang sudah diverifikasi |
| `projects/` | Konsep video baru, rencana shot, prompt, evaluasi, dan [arsip lama](projects/legacy/README.md) |

Contoh pasangan berkas setelah migrasi Tahap 4:

- `references/muyon/videos/muyon-01.mp4`
- `references/muyon/analysis/muyon-01.md`
- `references/muyon/frames/muyon-01/`

Nama yang sama (`muyon-01`) menghubungkan video, analisis, dan frame.

## Status implementasi

**Tahap 1–5 selesai pada branch kerja:** struktur folder, aturan AI, tiga template, migrasi 16 MP4 Muyon, katalog referensi, persiapan Style Library, dan pengarsipan master prompt lama. Semua berkas analisis masih **`pending`**, belum ada isi analisis video yang terverifikasi.

- Video: `references/muyon/videos/muyon-01.mp4` sampai `muyon-16.mp4`.
- Analisis: `references/muyon/analysis/muyon-01.md` sampai `muyon-16.md`.
- Frame JPG: **belum diekstrak**; `references/muyon/frames/` masih disiapkan.
- Katalog: [`references/INDEX.md`](references/INDEX.md) berisi 16 referensi dan tautan file yang benar.
- Style Library: [`styles/README.md`](styles/README.md) berisi aturan membuat profile, **belum** berisi profile terverifikasi.
- Arsip prompt lama: `projects/legacy/mp-v01.md` (isi file tetap identik).

**Tahap berikutnya:** verifikasi menyeluruh dan Pull Request untuk ditinjau (Tahap 6). **Tidak dilakukan pada Tahap 5.**

> Menyimpan dokumen di GitHub tidak otomatis melatih ulang model AI. AI harus diberikan akses dan diarahkan untuk membaca dokumen yang relevan.
