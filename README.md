# HASIL
- **Pratikum 1**
![alt text](image.png)

# Penjelasan Maksud Langkah 4: Membuat data_layer.dart
berfungsi untuk mengelola beberapa model dalam satu tempat ekspor. Dengan membuat data_layer.dart,  hanya perlu melakukan satu kali impor untuk mengakses kedua model plan.dart dan task.dart.

# Alasan Penggunaan Variabel plan sebagai Konstanta pada Langkah 6
Variabel plan di langkah ini dibuat sebagai konstanta karena nilai-nilainya dianggap tidak akan berubah selama aplikasi berjalan. Dengan menetapkannya sebagai konstanta (const),  mendapatkan performa yang lebih baik dan memastikan nilai ini tidak sengaja diubah, sehingga kode menjadi lebih aman dan mudah dipelihara.

# Kegunaan Metode pada Langkah 11 dan 13 dalam Lifecycle State
- **Langkah 11 (Metode initState):** initState adalah bagian dari siklus hidup Flutter yang dipanggil satu kali ketika widget pertama kali dimuat. Pada langkah ini, scrollController ditambahkan dengan listener agar ketika pengguna menggulir halaman, fokus pada TextField atau input lain akan hilang. Hal ini meningkatkan UX dengan memastikan keyboard otomatis menyembunyikan ketika layar digulir.
- **Langkah 13 (Metode dispose):** dispose berguna untuk menghapus scrollController dari memori ketika widget sudah tidak digunakan. Tanpa metode ini, widget dapat mengalami kebocoran memori karena controller tetap berada dalam memori meskipun tidak digunakan lagi.