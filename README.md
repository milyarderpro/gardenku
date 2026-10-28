# Gardenku

**Gardenku** adalah pustaka referensi video kebun untuk AI: mengamati video asli, menyimpan analisis yang dapat ditelusuri, mengembangkan ide baru, dan membuat prompt Google Veo/Flow per shot.

**Bahasa:** nama folder/file teknis memakai bahasa Inggris, isi dokumen dan prompt memakai bahasa Indonesia (istilah teknis kamera boleh berbahasa Inggris).

## Mulai dari sini

| Yang ingin dilakukan | Dokumen yang dibaca |
|---|---|
| Memahami aturan kerja AI | [AGENTS.md](AGENTS.md) |
| Mencari referensi | [references/INDEX.md](references/INDEX.md) |
| Menganalisis video | [Aturan analisis](rules/analysis.md) + [template analisis](templates/video-analysis.md) |
| Membuat ide atau konsep | [Aturan ide](rules/ideas.md) + [template konsep](templates/video-concept.md) |
| Membuat prompt Veo/Flow | [Aturan prompt](rules/prompts.md) + [template prompt](templates/video-prompt.md) |
| Mempelajari gaya visual | [styles/README.md](styles/README.md) |
| Menyimpan produksi dan hasil uji | [projects/README.md](projects/README.md) |

## Struktur folder

```text
gardenku/
├── README.md                 # Pengantar untuk pengguna
├── AGENTS.md                 # Navigasi dan prioritas kerja AI
├── rules/                    # Ketentuan bagaimana pekerjaan dilakukan
├── templates/                # Bentuk dokumen yang dihasilkan
├── references/               # Video, analisis, dan frame menurut sumber
│   ├── INDEX.md              # Katalog seluruh kreator
│   └── muyon/
│       ├── README.md
│       ├── analysis/         # hasil per video (Markdown + Frame Manifest)
│       └── frames/           # JPG ekstraksi asli, termasuk preview kecil
├── styles/                   # Rangkuman gaya berbasis bukti
└── projects/                 # Konsep, prompt, evaluasi, dan arsip
```

Satu kreator dapat memiliki berbagai jenis kebun (open-field, front-yard, backyard, rooftop, dan sebagainya). **Jenis kebun adalah metadata analisis, bukan subfolder tambahan.** ID seperti `muyon-01` menghubungkan video, analisis, dan folder frame.

## Referensi dan status terkini

- **Daftar referensi, metadata ringkas, dan status analisis terbaru:** [references/INDEX.md](references/INDEX.md).
- **Temuan per video, timestamp, dan JPG yang benar-benar tersimpan:** buka berkas dari [references/muyon/analysis/](references/muyon/analysis/); tiap analisis memuat Frame Manifest sesuai [template](templates/video-analysis.md).
- **Frame JPG asli hasil ekstraksi:** tersimpan di `references/<creator>/frames/<video-id>/` jika sudah diunggah. Status `draft` bukan berarti sudah disetujui.
- [Master prompt lama](projects/legacy/README.md) diarsipkan agar tidak bertentangan dengan aturan baru.
- URL Facebook asli dan izin penggunaan setiap video belum terverifikasi. **Repository ini publik:** hak untuk membagikan JPG juga perlu diperiksa. Penghapusan MP4 dari branch terbaru **tidak menghapus MP4 dari riwayat Git**; pembersihan riwayat memerlukan tindakan terpisah.

**Alur rutin:** pengguna mengunggah MP4 lewat chat → AI menganalisis sumber → mengekstrak 2–3 JPG pilihan → menyimpan Markdown dan JPG serta menyinkronkan katalog → menjalankan **Verification Gate**. **MP4 asli tetap di PC pengguna, tidak disimpan di GitHub.** Saat perlu mengoreksi gerakan/transisi di sesi lain, pengguna dapat mengirim ulang MP4 karena JPG tidak menggantikan video. [Aturan lengkap](rules/analysis.md). GitHub menyimpan pengetahuan, **bukan** melatih ulang model AI.
