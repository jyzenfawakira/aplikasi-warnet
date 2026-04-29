# Aplikasi-Warnet
Ada 4 trigger terdiri dari :
1. trg_tambah_jam di tabel log_tambah_waktu, untuk menambah durasi dan total biaya di transaksi saat user tambah waktu
2. trg_pc_dipakai di tabel transaksi, untuk mengubah status PC menjadi "dipakai" saat transaksi dibuat
3. trg_pc_selesai di tabel transaksi, untuk mengubah status PC menjadi "kosong" saat transaksi selesai
4. trg_log_pembayaran di tabel pembayaran, untuk mencatat aktivitas pembayaran ke log
