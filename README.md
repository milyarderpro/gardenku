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

## Kondisi data sekarang

- **16 video Muyon** telah tersedia di `references/muyon/videos/`.
- **16 dokumen analisis** tersedia di `references/muyon/analysis/`, semuanya masih **`pending`** (belum dianalisis).
- Belum ada frame JPG asli atau style profile yang didukung analisis terverifikasi.
- [Master prompt lama](projects/legacy/README.md) diarsipkan agar tidak bertentangan dengan aturan baru.
- URL Facebook asli dan izin penggunaan setiap video belum terverifikasi. **Repository ini publik; periksa izin/hak distribusi sebelum memperluas penggunaan atau membagikan video.**

**Langkah kerja berikutnya:** analisis referensi satu per satu, ekstrak frame asli bila tersedia alat yang mendukung, lalu perbarui katalog dan gaya visual berdasarkan bukti. Menyimpan file di GitHub **tidak** otomatis melatih ulang model AI; model harus diberi akses dan membaca file yang relevan.
