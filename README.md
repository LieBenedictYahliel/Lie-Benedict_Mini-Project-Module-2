#  Analisis Faktor Penentu Rating Produk di E-Commerce

## Deskripsi Singkat
Mini project ini mengeksplorasi bagaimana harga, diskon, brand, dan kategori produk memengaruhi rating pelanggan di e-commerce untuk menghasilkan insight strategis berbasis data.

---

## Latar Belakang
Dalam lingkungan digital yang kompetitif, pemahaman terhadap perilaku konsumen menjadi krusial bagi keberlangsungan bisnis. Salah satu indikator utama persepsi pelanggan adalah **rating produk**. Meski sering diasumsikan bahwa harga tinggi mencerminkan kualitas tinggi, studi ini menunjukkan bahwa persepsi tersebut juga dipengaruhi oleh **besarnya diskon**, **kategori produk**, serta **reputasi brand**.

Dengan meningkatnya ekspektasi konsumen dan kompleksitas strategi pemasaran digital, proyek ini bertujuan untuk mengidentifikasi pola nyata yang memengaruhi rating konsumen terhadap produk.

---

## Tujuan & Rumusan Masalah
1. Bagaimana pengaruh **diskon besar** terhadap **rating produk**?
2. Brand mana yang menunjukkan **rata-rata rating tertinggi dan terendah**?
3. Apakah terdapat **produk dengan rating tinggi namun harga sangat murah**?
4. Kategori mana yang memiliki **stok rendah akibat permintaan tinggi**?

---

## Sumber & Pengambilan Data
Dataset diperoleh dari platform e-commerce besar menggunakan **API scraping** dan mencakup informasi berikut:
- Nama & kategori produk
- Harga asli, diskon, dan harga akhir
- Brand
- Rating & jumlah ulasan
- Jumlah stok tersedia

Data dikonversi ke dalam format tabular dan dianalisis menggunakan Python dengan library utama seperti `pandas`, `seaborn`, dan `matplotlib`.

---

## Pembersihan & Transformasi Data
Beberapa proses preprocessing yang dilakukan:
- Menghapus duplikasi dan nilai kosong
- Konversi kolom harga dan diskon menjadi numerik
- Ekstraksi nama brand dari nama produk
- Segmentasi harga dan stok menjadi kategori rendah, sedang, tinggi
- Normalisasi format rating dan kategorisasi nama produk

---

## Hasil Analisis & Insight

### Korelasi Harga dan Rating
- Terdapat korelasi positif lemah (**+0.16**) antara harga dan rating.
- Produk mahal cenderung sedikit lebih tinggi rating-nya, namun tidak signifikan secara statistik.

### Diskon dan Persepsi Kualitas
- Korelasi negatif lemah (**−0.20**) antara diskon dan rating.
- Produk dengan diskon besar cenderung mendapat rating sedikit lebih rendah — kemungkinan karena ekspektasi tinggi yang tidak terpenuhi.

### Brand dengan Rating Tertinggi dan Terendah
- **Knoll (4.88)**, **Velvet Touch (4.64)**, dan **FreshCo (4.46)** mendominasi brand dengan rating tertinggi.
- **Essence (2.56)** dan **Glamour Beauty (2.86)** termasuk yang terendah dan memerlukan evaluasi kualitas menyeluruh.

### Produk Murah, Rating Tinggi
- Produk dengan **harga Rp2.490** dan **rating 4.93** menjadi bukti bahwa **harga murah bukan hambatan untuk rating tinggi**.
- Fenomena ini umum ditemukan pada produk kebutuhan dasar.

### Permintaan vs Kategori
- **Kategori groceries** memiliki stok terendah → mengindikasikan permintaan tinggi dan rotasi cepat.
- **Kategori beauty** memiliki stok tertinggi → menunjukkan permintaan lebih lambat akibat siklus pembelian yang panjang.

---

## Rekomendasi Strategis

1. **Gabungkan Harga dan Kualitas**  
   Harga tinggi saja tidak cukup. Fokus pada kualitas produk dan pengalaman pengguna untuk membangun loyalitas.

2. **Evaluasi Produk Diskon**  
   Diskon besar harus disertai dengan kontrol kualitas dan ekspektasi pelanggan yang realistis.

3. **Promosikan Produk Value-for-Money**  
   Produk murah dan berkualitas tinggi terbukti memperoleh rating sangat baik. Ini bisa menjadi flagship brand Anda.

4. **Audit Kinerja Brand Secara Berkala**  
   Gunakan brand unggulan sebagai benchmark dan analisis penyebab rendahnya rating pada brand bermasalah.

5. **Fokus pada Kategori Groceries**  
   Sebagai kategori dengan permintaan tinggi, groceries cocok dijadikan prioritas dalam stok dan promosi.

6. **Rancang Promosi Berdasarkan Perilaku**  
   Gunakan data untuk menentukan strategi promosi yang disesuaikan dengan karakteristik masing-masing kategori produk.

7. **Gunakan Rating sebagai Feedback Loop**  
   Jangan hanya menjadikan rating sebagai hasil, tetapi juga sebagai input strategis untuk inovasi produk dan layanan.

---

## Kesimpulan

- **Harga dan diskon berpengaruh terhadap rating**, meski korelasinya tidak kuat, namun penting secara strategis.
- **Brand merupakan penentu utama persepsi kualitas**, dan perannya sangat signifikan dalam membangun kepercayaan pelanggan.
- **Produk murah berkualitas tinggi mendapat rating tertinggi**, membuktikan bahwa konsumen menghargai value for money.
- **Kategori groceries menunjukkan pola permintaan tertinggi**, menjadikannya sektor penting untuk pengelolaan stok dan strategi promosi.
- **Analisis multivariat seperti ini diperlukan untuk pengambilan keputusan bisnis berbasis data** yang lebih tepat sasaran dan berdampak.

---

## 📎 Penutup
Proyek ini membuktikan bahwa **data analytics dapat mengungkap insight yang tidak selalu intuitif**, dan dapat digunakan sebagai landasan objektif untuk pengambilan keputusan dalam strategi produk dan pemasaran.
