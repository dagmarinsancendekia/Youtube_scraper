# YouTube Scraper

Aplikasi Python untuk scraping data video dari YouTube.com menggunakan Selenium, BeautifulSoup, Pandas, dan OpenPyXL.

## Deskripsi

Aplikasi ini memungkinkan pengguna untuk mencari video di YouTube dan mengekstrak data seperti judul video, channel, jumlah views, dan tanggal upload. Data kemudian disimpan dalam format Excel yang mudah dibaca.

## Fitur

- Pencarian video berdasarkan kata kunci
- Ekstraksi data video: judul, channel, views, tanggal upload
- Penyimpanan data ke file Excel dengan format yang rapi
- Dukungan multi-halaman
- Mode headless untuk performa yang lebih baik

## Persyaratan

- Python 3.6+
- Google Chrome browser
- ChromeDriver (otomatis dikelola oleh Selenium)
- Modul Python: selenium, beautifulsoup4, pandas, openpyxl

## Instalasi

1. Clone atau download repository ini.
2. Install dependencies:

   ```
   pip install selenium beautifulsoup4 pandas openpyxl
   ```

3. Pastikan Chrome browser terinstall.

## Penggunaan

### GUI Mode (Recommended)

1. Jalankan script dengan double-click file `run_youtube_scraper.bat` atau jalankan:

   ```
   python youtube_scraper.py
   ```

2. GUI akan terbuka. Masukkan kata kunci pencarian dan jumlah halaman.
3. Klik "Scrape" untuk mulai scraping. Data akan ditampilkan di tabel.
4. Klik "Save to Excel" untuk menyimpan data ke file `youtube_data.xlsx`.

### CLI Mode (Fallback)

Jika Tkinter tidak tersedia, script akan fallback ke mode CLI:

1. Jalankan script:

   ```
   python youtube_scraper.py
   ```

2. Masukkan kata kunci pencarian YouTube saat diminta.
3. Masukkan jumlah halaman yang ingin di-scrape.
4. Tunggu proses scraping selesai.
5. Data akan disimpan ke file `youtube_data.xlsx`.

## Output

File Excel akan berisi kolom:
- Title
- Channel
- Views
- Upload Date

Data diformat dengan header yang jelas dan lebar kolom yang disesuaikan untuk kemudahan membaca.

## Catatan

- Scraping mungkin melanggar terms of service YouTube. Gunakan dengan bijak.
- Struktur HTML YouTube dapat berubah, sehingga script mungkin perlu disesuaikan.
- Untuk performa yang lebih baik, gunakan mode headless.

## Lisensi

MIT License
