Berikut pembaruan README dengan perubahan pada bagian **Fitur Utama** dan **Teknologi yang Digunakan**:

---

# Proyek Analisis Data: Dataset Publik E-Commerce 📊

Proyek ini adalah dashboard interaktif yang dikembangkan menggunakan **Streamlit** untuk menganalisis dataset e-commerce publik. Dashboard ini memungkinkan pengguna untuk menjawab pertanyaan bisnis kunci terkait sebaran penjual berdasarkan lokasi geografis dan visualisasi data yang terkait.

## Detail Proyek
- **Nama:** Indra Mauludani Efendi
- **Email:** [indramauludani09@gmail.com](mailto:indramauludani09@gmail.com)
- **ID Dicoding:** indramauludani14
- **Streamlit:** https://indramauludaniefendi.streamlit.app/

### Pertanyaan Bisnis
1. Apakah terdapat hubungan antara harga produk (price) dan biaya pengiriman (freight_value)?
2. Bagaimana distribusi metode pembayaran yang digunakan oleh pelanggan, dan apakah metode pembayaran tertentu cenderung digunakan untuk transaksi dengan nilai yang lebih tinggi?

## Fitur Utama
- **Analisis Korelasi Harga dan Biaya Pengiriman**: Menggunakan *heatmap* untuk menampilkan korelasi antara harga produk dan biaya pengiriman.
- **Distribusi Metode Pembayaran**: Menggunakan *bar chart* untuk menganalisis frekuensi penggunaan metode pembayaran dan nilai transaksi yang terkait dengan setiap metode.
- **Pembersihan Data Otomatis**: Sistem otomatis untuk deteksi duplikat dan penghapusan data yang hilang.
- **Filter Interaktif**: Pengguna dapat memfilter data berdasarkan berbagai parameter seperti metode pembayaran, harga produk, dan biaya pengiriman.
- **Visualisasi Dinamis**: Pengguna dapat menjelajahi data dalam berbagai format visual seperti bar chart, histogram, dan heatmap yang diperbarui secara dinamis sesuai filter yang diterapkan.

## Tahapan Proyek
1. **Identifikasi Pertanyaan Bisnis**:
   Saya memulai dengan menentukan dua pertanyaan bisnis utama, yaitu hubungan antara harga produk dan biaya pengiriman serta distribusi metode pembayaran yang digunakan oleh pelanggan. Pertanyaan ini akan memandu arah analisis.

2. **Pengumpulan Dataset**:
   Saya mengumpulkan dua dataset utama: `order_items_dataset.csv` yang berisi detail produk dan pengiriman, serta `order_payments_dataset.csv` yang memuat informasi metode pembayaran pelanggan. 

3. **Pembersihan Data**:
   Pada tahap ini, saya membersihkan data dengan menghapus duplikat dan menangani nilai yang hilang. Langkah ini memastikan data yang digunakan untuk analisis lebih akurat dan tidak bias.

4. **Analisis Korelasi**:
   Analisis korelasi dilakukan untuk mengidentifikasi hubungan antara harga produk (`price`) dan biaya pengiriman (`freight_value`). Hasilnya menunjukkan korelasi positif sebesar **0.41**, menunjukkan bahwa produk yang lebih mahal cenderung memiliki biaya pengiriman yang lebih tinggi.

5. **Distribusi Metode Pembayaran**:
   Analisis distribusi metode pembayaran menunjukkan bahwa **kartu kredit** adalah metode yang paling banyak digunakan, terutama untuk transaksi bernilai tinggi. Temuan ini penting untuk memandu strategi promosi perusahaan.

6. **Visualisasi dan Dashboard Interaktif**:
   Saya membangun dashboard interaktif menggunakan **Streamlit** untuk memungkinkan pengguna berinteraksi dengan visualisasi data dan hasil analisis, sehingga pengguna dapat mengeksplorasi lebih dalam berdasarkan kota, kode pos, dan korelasi variabel.

7. **Insight dan Implementasi**:
   Dari hasil analisis, ditemukan bahwa produk mahal cenderung memiliki biaya pengiriman lebih besar, dan kartu kredit adalah metode pembayaran yang paling banyak digunakan untuk transaksi bernilai tinggi. Temuan ini dapat membantu dalam strategi promosi dan pengiriman perusahaan.

## Teknologi yang Digunakan
- **Streamlit**: Framework untuk membuat aplikasi web interaktif berbasis data.
- **Pandas**: Library untuk manipulasi data, pembersihan, dan analisis dataset.
- **Seaborn & Matplotlib**: Library visualisasi data untuk membuat grafik dan plot yang interaktif.
- **NumPy**: Digunakan untuk perhitungan numerik yang mendukung analisis korelasi.
- **Python**: Bahasa pemrograman utama yang digunakan untuk seluruh proyek.

## Setup Environment

### Menggunakan Anaconda
1. Buat environment baru dengan Python 3.9:
   ```bash
   conda create --name proyek_ecommerce python=3.9
   ```
2. Aktifkan environment:
   ```bash
   conda activate proyek_ecommerce
   ```
3. Install dependencies yang diperlukan:
   ```bash
   pip install -r requirements.txt
   ```

### Menggunakan Shell/Terminal
1. Buat folder proyek:
   ```bash
   mkdir proyek_ecommerce
   cd proyek_ecommerce
   ```
2. Inisialisasi virtual environment menggunakan **venv**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Unix/macOS
   venv\Scripts\activate  # Windows
   ```
3. Install dependencies dari file `requirements.txt`:
   ```bash
   pip install -r requirements.txt
   ```

## Menjalankan Aplikasi Streamlit
Setelah semua dependensi terinstall, Anda bisa menjalankan aplikasi dengan perintah berikut:

```bash
streamlit run dashboard.py
```

Aplikasi akan berjalan di browser dan bisa diakses melalui URL yang ditampilkan (biasanya `http://localhost:8501`).

## Struktur Direktori
```plaintext
proyek_ecommerce/
│
├── Dashboard.py             # File utama aplikasi Streamlit
├── README.md              # File ini
├── requirements.txt       # Daftar dependensi Python
└── order_items_dataset.csv   # Folder untuk menyimpan dataset (opsional)
└── order_payments_dataset.csv   # Folder untuk menyimpan dataset (opsional)
└── Proyek_Analisis_Data
```

## Lisensi
Proyek ini tidak memiliki lisensi dan digunakan untuk keperluan edukasi.

---
