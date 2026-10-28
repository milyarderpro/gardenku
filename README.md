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
│       ├── videos/           # muyon-01.mp4 ... muyon-16.mp4
│       ├── analysis/         # muyon-01.md ... muyon-16.md
│       └── frames/           # JPG asli bila sudah diekstrak
├── styles/                   # Rangkuman gaya berbasis bukti
└── projects/                 # Konsep, prompt, evaluasi, dan arsip
```

Satu kreator dapat memiliki berbagai jenis kebun (open-field, front-yard, backyard, rooftop, dan sebagainya). **Jenis kebun adalah metadata analisis, bukan subfolder tambahan.** ID seperti `muyon-01` menghubungkan video, analisis, dan folder frame.

## Referensi dan status terkini

- **Daftar video, metadata ringkas, dan status analisis terbaru:** [references/INDEX.md](references/INDEX.md).
- **Temuan per video, timestamp, dan JPG yang benar-benar tersimpan:** buka berkas dari [references/muyon/analysis/](references/muyon/analysis/); tiap analisis memuat Frame Manifest sesuai [template](templates/video-analysis.md).
- **Frame JPG asli hasil ekstraksi:** tersimpan di `references/<creator>/frames/<video-id>/` jika sudah diunggah. Status `draft` bukan berarti sudah disetujui.
- [Master prompt lama](projects/legacy/README.md) diarsipkan agar tidak bertentangan dengan aturan baru.
- URL Facebook asli dan izin penggunaan setiap video belum terverifikasi. **Repository ini publik; periksa izin/hak distribusi sebelum memperluas penggunaan atau membagikan video.**

**Alur rutin:** terima video yang bisa diperiksa (termasuk unggahan chat), analisis berdasarkan bukti, pilih frame JPG penting, verifikasi unggahan GitHub, lalu sinkronkan katalog. Prosedur lengkap ada di [rules/analysis.md](rules/analysis.md). Menyimpan file di GitHub **tidak** otomatis melatih ulang model AI; model harus diberi akses dan membaca file yang relevan.
