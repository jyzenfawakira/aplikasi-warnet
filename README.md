# Aplikasi-Warnet
## Kelompok 8:
### -Arya Bintang Akbari
### -Jibril Fawaz Alfirdaus
### -Justin Arya Barraq Logawi

Pada sistem Xreovos Net, digunakan beberapa trigger untuk mengotomatisasi proses dalam database. Trigger pertama adalah trg_tambah_jam, yang berjalan setelah terjadi penambahan data pada tabel log_tambah_waktu. Trigger ini berfungsi untuk memperbarui durasi total dan total pembayaran pada tabel transaksi ketika customer menambah waktu penggunaan komputer, tanpa membuat transaksi baru.

Trigger kedua adalah trg_pc_dipakai, yang berjalan setelah data transaksi baru dibuat. Trigger ini berfungsi untuk mengubah status komputer pada tabel pc menjadi “dipakai”, sehingga sistem secara otomatis menandai bahwa komputer tersebut sedang digunakan.

Selanjutnya, terdapat trigger trg_pc_selesai yang berjalan setelah terjadi pembaruan data pada tabel transaksi. Jika status transaksi diubah menjadi “selesai”, maka trigger ini akan mengubah status komputer kembali menjadi “kosong”, sehingga komputer tersebut dapat digunakan kembali oleh customer lain.

Trigger terakhir adalah trg_log_pembayaran, yang berjalan setelah data pembayaran ditambahkan ke dalam tabel pembayaran. Trigger ini berfungsi untuk mencatat aktivitas pembayaran ke dalam tabel log_tambah_waktu sebagai bagian dari monitoring aktivitas dalam sistem.

Secara keseluruhan, penggunaan trigger pada sistem ini bertujuan untuk mengurangi proses manual, menjaga konsistensi data, serta memastikan setiap perubahan data langsung diikuti oleh proses lain yang berkaitan secara otomatis.

Ada 4 trigger terdiri dari :
1. trg_tambah_jam di tabel log_tambah_waktu, untuk menambah durasi dan total biaya di transaksi saat user tambah waktu
2. trg_pc_dipakai di tabel transaksi, untuk mengubah status PC menjadi "dipakai" saat transaksi dibuat
3. trg_pc_selesai di tabel transaksi, untuk mengubah status PC menjadi "kosong" saat transaksi selesai
4. trg_log_pembayaran di tabel pembayaran, untuk mencatat aktivitas pembayaran ke log
