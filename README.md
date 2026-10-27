# Gardenku

Gardenku adalah pustaka referensi video kebun untuk membantu AI **menganalisis video**, **mempelajari gaya visual**, **mengembangkan ide baru**, dan **menyusun prompt video per shot**.

Dokumen ditulis dalam **bahasa Indonesia**; nama folder dan file teknis memakai **bahasa Inggris**.

## Struktur pustaka

| Lokasi | Fungsi |
|---|---|
| `AGENTS.md` | Petunjuk bagi AI yang bekerja dengan repository ini |
| `rules/` | Aturan analisis referensi, pembuatan ide, dan penulisan prompt (tahap 2) |
| `templates/` | Format dokumen standar (tahap 3) |
| `references/` | Referensi yang dikelompokkan menurut sumber/kreator |
| `references/<creator>/videos/` | Video asli dari kreator tersebut |
| `references/<creator>/analysis/` | Hasil analisis setiap video |
| `references/<creator>/frames/` | Gambar frame asli yang diekstrak dari video |
| `styles/` | Rangkuman karakter visual dari referensi yang sudah dianalisis |
| `projects/` | Konsep video baru, rencana shot, prompt, dan evaluasi |

Contoh pasangan berkas setelah migrasi:

- `references/muyon/videos/muyon-01.mp4`
- `references/muyon/analysis/muyon-01.md`
- `references/muyon/frames/muyon-01/`

Nama yang sama (`muyon-01`) menghubungkan video, analisis, dan frame.

## Status implementasi

**Tahap 1 — Penyiapan struktur:** branch kerja, folder dasar, README, dan petunjuk AI.

**Belum dilakukan pada tahap 1:**
- Pembuatan aturan dan template lengkap.
- Pemindahan 16 video Muyon.
- Pembuatan analisis dan ekstraksi frame.
- Pembuatan `references/INDEX.md` dan style profile.

**Video asli saat ini masih berada di:** `kebun01/video-ref/muyon-01.mp4` hingga `muyon-16.mp4`.

**Master prompt lama masih berada di:** `prompt/mp-v01.md`.

Jangan menganggap folder yang baru disiapkan sudah berisi analisis atau hasil pemindahan video.

## Tahapan berikutnya

1. Menulis `rules/analysis.md`, `rules/ideas.md`, dan `rules/prompts.md`.
2. Menyusun template analisis, konsep, dan prompt.
3. Memindahkan file video secara aman; membuat berkas analisis berstatus belum dikerjakan.
4. Menyiapkan indeks referensi dan pustaka gaya.
5. Memeriksa konsistensi file serta mengajukan Pull Request untuk ditinjau.

> Menyimpan dokumen di GitHub tidak otomatis melatih ulang model AI. AI harus diberikan akses dan diarahkan untuk membaca dokumen yang relevan.
