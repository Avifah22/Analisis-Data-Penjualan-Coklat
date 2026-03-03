# Analisis-Data-Penjualan-Coklat
Analisis menggunakan Python untuk mengetahui segmentasi  dan Power BI untuk visualisasi sales yang membutuhkan pengarahan serta strategi stok

🎯 Tujuan Analisis
Mengelompokkan data penjualan untuk menjawab dua tantangan utama:
1. Profil Sales: Mencari tahu siapa yang main di volume besar (grosir/murah), siapa yang main di margin tinggi (eksklusif/mahal), siapa yang bisa disebut imbang antara margin dan volume dan siapa yang butuh arahan atau pelatihan lebih lanjut
2. Geographical Insights: Negara mana yang menjadi "sweet spot" untuk jenis coklat tertentu.
 
 💡 Hasil
Setelah melakukan analisis data (EDA), hasil yang ditemukan adalah:
1. Segmentasi sales person berdasarkan performa
Cluster 2: Amount Tinggi (>10rb), Boxes Rendah-Sedang -> Premium High-Earners
Cluster 1: Amount Sedang, Boxes Paling Tinggi (>400) ->  High Volume Drivers
Cluster 0: Amount Sedang, Boxes Rendah -> Kelompok yang stabil, bisa mendapatkan pelatihan agr bisa masuk cluster 2
Cluster 4: Performers	Amount Rendah-Sedang, Boxes Sedang -> Cukup aktif dalam mengirimkan barang, bisa mendaptkan pelatihan agar masuk cluster 1
Cluster 3: Amount Rendah (<5rb), Boxes Paling Rendah-> yang membutuhkan pelatihan lebih lanjut agar bisa masuk cluster 2 atau 1
Geographical Insights : 3 Negara dengan pengiriman terbanyak adalah Australia, Canada dan UK. perlu diperhatika produk coklat apa saja yang banyak dikirim di negara tersebut guna memastikan stok mencukupi


📈 Evaluasi Model
1. Elbow Method: Hasil evaluasi menunjukkan penurunan inertia mulai melandai di K=3 dan K=5. Dipilihnya K=5 sebgai jumlah kluster optimal karena memberikan granulasi data yang lebih baik untuk strategi bisnis.
2. Silhouette Score:
a. Silhouette Score (K=3): 0.41 (Struktur data paling optimal secara statistik).
b. Silhouette Score (K=5): 0.36 (Struktur data yang dipilih untuk kebutuhan bisnis).
Dipilih K=5 karena memberikan segmentasi yang lebih mendalam untuk strategi operasional.

🛠️ Tech Stack & Workflow
- Pandas: Manipulasi data & cleaning.
- Matplotlib, Seaborn dan Power BI: Visualisasi data.
- K-Mean: Algoritma unsupervised machine learning yang digunakan untuk membuat cluster`.
- Scikit-Learn: Evaluasi model dan standarisasi skala menggunakan StandardScaler.

---
**Disclaimer:** Dataset ini bersifat publik dan diambil dari https://www.kaggle.com/datasets/saidaminsaidaxmadov/chocolate-sales
