# Hasil Analisa

### Langkah 1:
Code ini digunakan untuk:
1. Mengimpor pustaka yang diperlukan: NumPy (untuk operasi matematika), Pandas (untuk mengelola data), dan Matplotlib (untuk membuat grafik).
2. Membaca data dari file CSV yang bernama `Order_details(masked).csv` dan menyimpannya dalam variabel `Order_Details` untuk dianalisis lebih lanjut.
Dengan ini, bisa mulai menganalisis data pesanan yang ada di dalam file tersebut.

### Langkah 2:
Code tersebut bertujuan untuk menganalisis waktu transaksi. 
1. Mengonversi Tanggal: Kolom "Transaction Date" diubah menjadi format waktu (datetime) agar bisa diproses lebih lanjut.
2. Ekstraksi Jam: Dari kolom waktu tersebut, hanya jamnya yang diambil dan disimpan di kolom baru "Hour."
Dengan data jam transaksi, bisa menganalisis kapan transaksi paling banyak terjadi, misalnya pada jam-jam tertentu, untuk mengetahui pola transaksi atau jam puncak transaksi.

### Langkah 3:
Code ini digunakan untuk menemukan jam-jam dengan jumlah pesanan terbanyak dalam sehari:
1. `timemost1`: Menyimpan daftar jam yang memiliki pesanan terbanyak (dari 24 jam).
2. `timemost2`: Menyimpan jumlah pesanan pada jam-jam yang ada di `timemost1`.
Dengan data ini, bisa tahu jam mana yang paling sibuk dan menyesuaikan strategi operasional sesuai dengan waktu puncak pesanan.

### Langkah 4:
Berdasarkan tabel, pembelian terbanyak terjadi jam 12 siang dan 11 malam, masing-masing 51 pembelian. Aktivitas juga tinggi di malam hari, terutama jam 7-9 malam. Sebaliknya, dini hari (jam 2-5 pagi) sangat sepi dengan hanya 1-3 pembelian. Fokus promosi sebaiknya pada siang dan malam hari untuk hasil maksimal.

### Langkah 5: 
Code ini digunakan untuk menganalisis jumlah pesanan yang terjadi pada setiap jam dalam sehari. 
1. Menghitung jumlah pesanan per jam: Menggunakan `value_counts()` untuk menghitung seberapa sering setiap jam muncul dalam data pesanan.
2. Membuat daftar jam: Menyiapkan daftar dari jam 0 hingga 23 (jam sehari penuh).
3. Menyortir data: Mengurutkan jumlah pesanan berdasarkan jam agar data lebih mudah dibaca.
4. Mengonversi ke list dan DataFrame: Mengubah data yang sudah diurutkan menjadi format list dan kemudian ke dalam DataFrame untuk analisis lebih lanjut.
Hasilnya, bisa melihat pola pesanan berdasarkan waktu, seperti jam-jam sibuk dan jam sepi.

### Langkah 6:
Berdasarkan grafik Sales Happening Per Hour (Spread Throughout The Week), pembelian paling banyak terjadi sekitar jam 10 pagi, sedangkan antara jam 12 malam hingga 5 pagi sangat sedikit. Aktivitas pembelian mulai ramai dari pagi, menurun siang hari, lalu meningkat lagi di sore hingga malam. Untuk meningkatkan penjualan, sebaiknya fokus pada waktu-waktu ramai (jam 10 pagi dan 3 sore sampai 8 malam). Selain itu, tawarkan diskon atau promo khusus di jam-jam sepi untuk menarik pembeli. Memahami alasan pembelian ramai di jam tertentu juga bisa membantu membuat strategi pemasaran yang lebih baik.

