# BOP - Best of Product
> Sistem Informasi Manajemen Magang Berbasis Web

![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## Tentang Proyek
Sistem ini menggantikan pengelolaan magang manual berbasis Google Spreadsheet 
di Program Studi Universitas Amikom Yogyakarta. Menyediakan platform multi-role 
(Mahasiswa, Dosen, Admin Prodi, Mitra) dengan workflow approval, monitoring 
real-time, dan pelaporan bulanan terstruktur.

## Fitur Utama
- **Mahasiswa** — lihat lowongan, daftar magang, submit laporan bulanan
- **Mitra Perusahaan** — input lowongan, review laporan mahasiswa
- **Admin Prodi** — approval lowongan, seleksi mahasiswa, monitoring dashboard
- **Dosen Pembimbing** — approval laporan, input nilai akhir

## Tech Stack
| Layer | Teknologi |
|-------|-----------|
| Frontend | React.js / Next.js |
| Backend | Node.js / Laravel |
| Database | MySQL / PostgreSQL |
| Auth | JWT |
| Deployment | Docker / Vercel |

## Struktur Branch
| Branch | Fungsi |
|--------|--------|
| `main` | Produksi, protected |
| `develop` | Integrasi harian |
| `feature/*` | Pengembangan fitur baru |
| `fix/*` | Perbaikan bug development |
| `release/*` | Persiapan rilis versi |
| `hotfix/*` | Perbaikan darurat produksi |
| `docs/*` | Dokumentasi teknis |

Alur: `feature/*` → `develop` → `release/*` → `main`

## Instalasi

# Clone repo
git clone https://github.com/username/bop.git
cd bop

# Install dependencies
npm install

# Setup environment
cp .env.example .env
# isi konfigurasi database di .env

# Jalankan migrasi
npm run migrate

# Jalankan aplikasi
npm run dev

## Struktur Folder
├── src/
│   ├── components/     # Komponen UI
│   ├── pages/          # Halaman per role
│   ├── api/            # Endpoint backend
│   └── utils/          # Helper functions
├── docs/               # Dokumentasi tambahan
├── tests/              # Test files
├── .env.example
└── README.md

## Cara Kontribusi
1. Checkout ke `develop`
2. Buat branch baru: `git checkout -b feature/nama-fitur`
3. Commit perubahan: `git commit -m "feat: deskripsi singkat"`
4. Push dan buat Pull Request ke `develop`

## 👥 Tim Pengembang

**Universitas Amikom Yogyakarta — 2025/2026**

| No | Nama | NIM | Peran | Tanggung Jawab |
|----|------|-----|-------|----------------|
| 1 | Alfan Shobron Jamal | 23.11.5438 | Product Owner | Menentukan arah produk, prioritas fitur, kebutuhan user |
| 2 | Nadia Muthia Jaya | 23.11.5424 | Scrum Master | Memastikan proses kerja tim, mengelola hambatan |
| 3 | Rizki Setyanugrah L | 23.11.5390 | Developer UI/UX | Desain tampilan, alur pengguna, prototype |
| 4 | Muhammad Naufal Yazid Akbar | 23.11.5870 | Developer Front End | Implementasi UI, integrasi ke backend |
| 5 | Raehan Wijaya | 23.11.5431 | Developer Back End | Server, database, logika aplikasi |
| 6 | Roy Devgantara Purba | 23.11.5565 | Developer Back End | Server, database, logika aplikasi |
