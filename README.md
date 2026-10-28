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
├── references/               # Analisis dan contact sheet JPG menurut sumber; tanpa MP4
│   ├── INDEX.md              # Katalog seluruh kreator
│   └── muyon/
│       ├── README.md
│       ├── analysis/         # hasil per video (Shot Map + Contact Sheet Manifest)
│       └── frames/           # satu JPG contact sheet multi-panel untuk setiap shot
├── styles/                   # Rangkuman gaya berbasis bukti
└── projects/                 # Konsep, prompt, evaluasi, dan arsip
```

Satu kreator dapat memiliki berbagai jenis kebun (open-field, front-yard, backyard, rooftop, dan sebagainya). **Jenis kebun adalah metadata analisis, bukan subfolder tambahan.** ID seperti `muyon-01` menghubungkan video, analisis, dan folder frame.

## Referensi dan status terkini

- **Daftar referensi, metadata ringkas, dan status analisis terbaru:** [references/INDEX.md](references/INDEX.md).
- **Temuan per video, timestamp dan path JPG standar:** buka berkas dari [references/muyon/analysis/](references/muyon/analysis/); tiap analisis memuat Shot Map dan Contact Sheet Manifest sesuai [template](templates/video-analysis.md).
- **Contact sheet JPG:** diberikan AI pada Fase 1; pengguna menyimpannya sendiri melalui repository lokal ke `references/<creator>/frames/<video-id>/`. Penyimpanan analisis tidak menunggu JPG di GitHub. Status `draft` bukan berarti disetujui.
- [Master prompt lama](projects/legacy/README.md) diarsipkan agar tidak bertentangan dengan aturan baru.
- URL Facebook asli dan izin penggunaan setiap video belum terverifikasi. **Repository ini publik:** hak untuk membagikan JPG juga perlu diperiksa. Penghapusan MP4 dari branch terbaru **tidak menghapus MP4 dari riwayat Git**; pembersihan riwayat memerlukan tindakan terpisah.

## Opsi B+ v1.3 — Two-Phase, Document-First Save

**Fase 1 — Analyze & Review (tahap 1–5):** unggah MP4 lewat chat → validasi → Shot Map (Pass 1) → Deep Shot Analysis (Pass 2) → contact sheet JPG per shot (target 3–6 panel adaptif) → Evidence Cross-Check. AI menampilkan hasil analisis dan **memberikan JPG individual untuk diunduh**. **STOP** sampai pengguna mengetik `save now`; tidak ada penulisan GitHub selama Fase 1.

**Fase 2 — Save & Verify (tahap 6–7):** setelah `save now`, AI menyimpan **Markdown analisis lengkap dan `references/INDEX.md` langsung ke `main`**, tanpa branch/PR dan **tanpa mengunggah JPG**. Contact Sheet Manifest mencatat nama/path JPG yang akan kamu simpan sendiri melalui repo lokal. Gate A memeriksa akurasi analisis; Gate B memeriksa **dokumen dan INDEX** yang benar-benar tersimpan. **Keduanya bisa PASS walaupun JPG belum dimasukkan ke GitHub**. Tidak otomatis menjadi `approved`.

MP4 asli tetap di PC pengguna, tidak disimpan di GitHub. Artefak sementara Fase 1 mungkin tidak tersedia jika berpindah percakapan; jangan menganggap file tersimpan permanen. [Aturan lengkap](rules/analysis.md). GitHub menyimpan pengetahuan, **bukan** melatih ulang model AI.
