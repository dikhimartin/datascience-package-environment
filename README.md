# Data Science Package Environment

## Deskripsi
Repositori ini menyediakan konfigurasi dan lingkungan yang diperlukan untuk proyek **Data Science** dengan menggunakan **Conda** untuk mengelola paket dan dependensi. Lingkungan ini mencakup pustaka untuk analisis data, visualisasi, dan machine learning. Pengguna dapat mengunduh dan menginstal lingkungan ini menggunakan file `environment.yml` untuk memulai proyek dengan dependensi yang konsisten dan dapat direproduksi.

## Fitur
- **Jupyter Lab** untuk eksplorasi data interaktif
- **Pandas**, **NumPy**, **Matplotlib** untuk analisis dan visualisasi data
- **Scikit-learn** untuk model machine learning dasar
- **DuckDB** untuk analisis data berbasis SQL
- **PyGWalker** untuk visualisasi data interaktif

## Prasyarat
Pastikan **Miniconda** atau **Anaconda** telah terinstal pada sistem Anda.

## Instalasi

1. **Clone repositori ini:**
   ```bash
   git clone https://github.com/username/datascience-package-environment.git
   cd datascience-package-environment
   ```

2. **Buat environment Conda dari file `environment.yml`:**
   ```bash
   conda env create -f environment.yml
   ```

3. **Aktifkan environment Conda:**
   ```bash
   conda activate datascience_package
   ```

4. **Instal Jupyter Lab jika belum terinstal:**
   ```bash
   conda install -c conda-forge jupyterlab
   ```

5. **Menjalankan Jupyter Lab:**
   ```bash
   jupyter lab
   ```

   Jika menggunakan Visual Studio Code, pastikan ekstensi Python dan Jupyter sudah terpasang, kemudian pilih kernel `datascience_package` untuk menjalankan notebook.

## Menjalankan Project

Setelah environment aktif, Anda dapat membuka file `main.ipynb` untuk menjalankan beberapa langkah analisis data dan memverifikasi bahwa semua pustaka berfungsi dengan baik. Notebook ini berisi contoh penggunaan pustaka utama, termasuk visualisasi data dan pembuatan model machine learning sederhana.

## Troubleshooting

Jika Anda mengalami masalah saat menjalankan environment atau Jupyter Lab, coba langkah berikut:
- **Pastikan kernel yang tepat dipilih di Jupyter Lab atau VSCode** (kernel `datascience_package`).
- **Jupyter Lab tidak berjalan?** Coba instal ulang dengan:
  ```bash
  conda install -c conda-forge jupyterlab
  ```
- **Kesalahan saat mengaktifkan environment:** Jika mendapatkan pesan error seperti `CondaError: Run 'conda init' before 'conda activate'`, jalankan:
  ```bash
  conda init
  ```

## Struktur Repositori

```
datascience-package-environment/
├── environment.yml         # Konfigurasi environment Conda
├── main.ipynb              # Notebook utama untuk analisis data
└── README.md               # Dokumentasi proyek
```

## Kontribusi

Jika Anda ingin berkontribusi pada proyek ini, silakan buka *issue* atau buat *pull request*. Kami menyambut baik kontribusi dari semua pihak.

## Lisensi
Proyek ini dilisensikan di bawah [MIT License](LICENSE).