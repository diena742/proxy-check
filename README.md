# 🚀 Proxy Checker & Auto-Updater

![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![GitHub last commit](https://img.shields.io/github/last-commit/username/repo)

Sebuah tools Python untuk mengecek validitas proxy dengan auto-update dari sumber terpercaya.

## 📦 Fitur Utama

- 🔄 Auto-update daftar proxy dari GitHub
- ⚡ Multi-threading untuk pengecekan cepat
- 📊 Tampilan hasil dalam format tabel
- 🎨 Warna terminal untuk readability
- 💾 Auto-save hasil ke file terpisah
- 📈 Statistik lengkap hasil pengecekan

## 🛠️ Instalasi

1. Clone repository:
```bash
git clone https://github.com/diena742/proxy-check.git
cd proxy-check
```

## Install dependencies:
- pip install -r requirements.txt

## 🚀Jalankan script:
- python proxy_checker.py

## Ubah parameter di proxy-check.py sesuai kebutuhan:
# Threading
MAX_THREADS = 10  # Jumlah maksimal thread
TIMEOUT = 5      # Timeout dalam detik

# File Output
LIVE_FILE = "live_proxies.txt"
DEAD_FILE = "dead_proxies.txt"

## 📂Struktur File

proxy-checker/
├── proxy_checker.py    # Main script
├── requirements.txt    # Dependencies
├── config.py           # Configuration
├── proxy/              # Folder penyimpanan proxy
│   ├── http.txt
│   └── socks5.txt
└── results/            # Hasil pengecekan
    ├── live_proxies.txt
    └── dead_proxies.txt

## 📊 Contoh Output

https://via.placeholder.com/600x200?text=Proxy+Checker+Output+Preview

## 🤝 Berkontribusi

Pull requests dipersilakan. Untuk perubahan besar, buka issue terlebih dahulu.

Fork project
- Buat branch fitur (git checkout -b fitur/namafitur)
- Commit changes (git commit -m 'Tambahkan fitur')
- Push branch (git push origin fitur/namafitur)
- Buat Pull Request

## 📜 Lisensi

Distributed under MIT License. Lihat LICENSE untuk lebih detail.

## PENUTUP

Dibuat dengan ❤️ oleh [diena742] - GitHub Profile
