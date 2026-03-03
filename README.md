# Analisis-Data-Penjualan-Coklat
Analisis menggunakan Python untuk mengetahui segmentasi  dan Power BI untuk visualisasi sales yang membutuhkan pengarahan serta strategi stok

🎯 Tujuan Analisis
Mengelompokkan data penjualan untuk menjawab dua tantangan utama:
Profil Sales: Mencari tahu siapa yang main di volume besar (grosir/murah), siapa yang main di margin tinggi (eksklusif/mahal), siapa yang bisa disebut imbang antara margin dan volume dan siapa yang butuh arahan atau pelatihan lebih lanjut
Geographical Insights: Negara mana yang menjadi "sweet spot" untuk jenis coklat tertentu.

📈 Evaluasi Model
Elbow Method: Hasil evaluasi menunjukkan penurunan inertia mulai melandai di K=3 dan K=5. Dipilihnya K=5 sebgai jumlah kluster optimal karena memberikan granulasi data yang lebih baik untuk strategi bisnis.
Silhouette Score:
a. Silhouette Score (K=3): 0.41 (Struktur data paling optimal secara statistik).
b. Silhouette Score (K=5): 0.36 (Struktur data yang dipilih untuk kebutuhan bisnis).
Dipilih K=5 karena memberikan segmentasi yang lebih mendalam untuk strategi operasional. 

