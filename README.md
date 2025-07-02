Proxy Checker & Auto-Updater
https://img.shields.io/badge/python-3.6%252B-blue
https://img.shields.io/badge/license-MIT-green

Sebuah script Python untuk mengecek dan memvalidasi proxy dari berbagai sumber, dengan fitur auto-update dari GitHub.

Fitur Utama
✅ Auto-update daftar proxy dari GitHub mudachyo/proxy-list

⚡ Multi-threading untuk pengecekan cepat (10 thread default)

📊 Tampilan tabel yang rapi menggunakan tabulate

🎨 Warna terminal untuk memudahkan pembacaan hasil

💾 Penyimpanan otomatis hasil live/dead proxy

🔄 Pengecekan perubahan sebelum memulai proses

📂 Manajemen file otomatis dengan backup

Instalasi
Clone repository ini:

bash
git clone https://github.com/[username]/proxy-checker.git
cd proxy-checker
Install dependencies:

bash
pip install -r requirements.txt
Penggunaan
Jalankan script:

bash
python proxy_checker.py
Konfigurasi
Anda bisa mengubah parameter di dalam script sesuai kebutuhan:

python
# --- Konfigurasi ---
PROXY_FOLDER = "proxy"          # Folder penyimpanan file proxy
LIVE_PROXIES_FILE = "live_proxies.txt"  # File output proxy live
DEAD_PROXIES_FILE = "dead_proxies.txt"  # File output proxy dead
TEST_URL = "http://www.google.com"      # URL untuk testing proxy
TIMEOUT = 10                    # Timeout dalam detik
MAX_THREADS = 10                # Jumlah thread maksimum
BATCH_SIZE = 10                 # Proxy per batch
BATCH_DELAY = 5                 # Delay antar batch
Output
Script akan menghasilkan:

live_proxies.txt - Berisi daftar proxy yang aktif dengan format:

text
IP:Port,Country,City,Speed,Type
dead_proxies.txt - Berisi daftar proxy yang tidak aktif

Contoh Output di Terminal
text
+-----------------+--------+-------------------+----------+--------+---------+
| IP Address      |   Port | Country, City     | Speed    | Type   | Status  |
+=================+========+===================+==========+========+=========+
| 192.168.1.1    |   8080 | United States, NY | 1.23s    | http   | Live    |
| 10.0.0.1       |   3128 | Germany, Berlin   | 2.45s    | SOCKS5 | Live    |
| 172.16.0.1     |   8888 | N/A               | N/A      | N/A    | Dead    |
+-----------------+--------+-------------------+----------+--------+---------+
Berkontribusi
Pull request dipersilakan. Untuk perubahan besar, buka issue terlebih dahulu untuk mendiskusikan apa yang ingin Anda ubah.

Lisensi
MIT

Dibuat dengan ❤️ oleh [diena742] - GitHub Profile
