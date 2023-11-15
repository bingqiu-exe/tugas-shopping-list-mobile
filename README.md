# shopping-list-mobile

# tugas 7

1. Apa perbedaan utama antara stateless dan stateful widget dalam konteks pengembangan aplikasi Flutter?
stateless widget adalah widget yang dibuild dengan konfigurasi yang telah diinisiasi sejak awal dan tidak akan pernah berubah sedangkan stateful widget adalah widget yang dapat berubah-ubah secara dinamis.

2. Sebutkan seluruh widget yang kamu gunakan untuk menyelesaikan tugas ini dan jelaskan fungsinya masing-masing.
- lihat item: untuk memunculkan snackbar dengan tulisan "Kamu telah menekan tombol Lihat Item"
- tambah item: untuk memunculkan snackbar dengan tulisan "Kamu telah menekan tombol Tambah Item"
- logout: untuk memunculkan snackbar dengan tulisan "Kamu telah menekan tombol Logout"

3. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial)
- Membuat proyek Flutter dengan nama "shopping_list"
- Mengatur tema warna aplikasi menjadi indigo.
- Mengubah widget di menu.dart dari stateful menjadi stateless.
- Menambahkan teks dan card untuk menampilkan barang-barang yang dijual.
- Menambahkan tipe data "ShopItem" untuk mendefinisikan barang-barang yang dijual.
- Menambahkan list "items" yang berisi barang-barang yang dijual.
- Menggunakan widget "GridView" untuk menampilkan card-card barang.
- Membuat widget stateless "ShopCard" untuk menampilkan setiap card dengan ikon dan teks yang sesuai.
- Menambahkan responsivitas ketika card diklik dan menampilkan pesan "SnackBar" sebagai pemberitahuan.
- Menambahkan list "colors" yang berisi warna - warna untuk widget.


# tugas 8

1. Jelaskan perbedaan antara Navigator.push() dan Navigator.pushReplacement(), disertai dengan contoh mengenai penggunaan kedua metode tersebut yang tepat!
Navigator.push() digunakan untuk menambahkan rute baru ke dalam navigasi, sementara Navigator.pushReplacement() digunakan untuk menggantikan rute yang sudah ada dengan yang baru dalam navigasi.
Contoh penggunaan fungsi Navigator.push() adalah Navigator.push(context, MaterialPageRoute(builder: (context) => const ConstellationPage())); fungsi ini digunakan ketika kita ingin menambahkan suatu rute ke dalam tumpukan rute.
Contoh dari Navigator.pushReplacement() adalah Navigator.push(context, MaterialPageRoute(builder: (context) => const ConstellationPage())); ini dapat digunakan ketika kita ingin memberi tahu pengguna tentang suatu rute yang belum diperbarui dalam waktu yang lama.

2. Jelaskan masing-masing layout widget pada Flutter dan konteks penggunaannya masing-masing!
layout widget terdiri dari:
- Container: Sebuah widget yang digunakan untuk memodifikasi ukuran dan gaya dari widget lain.
- Column: Sebuah widget yang digunakan untuk pengaturan vertikal dari widget.
- Expanded: Sebuah widget yang digunakan untuk menampilkan rentang kosong dalam tata letak widget.
- Stack: Sebuah widget yang digunakan untuk menumpuk widget lainnya.

3. Sebutkan apa saja elemen input pada form yang kamu pakai pada tugas kali ini dan jelaskan mengapa kamu menggunakan elemen input tersebut!
TextFormField adalah sebuah widget Flutter yang digunakan untuk membuat sebuah kolom formulir yang terintegrasi dengan widget Form.
Tujuan dari tugas ini adalah untuk membuat sebuah kolom formulir dengan label menggunakan TextFormField.

4. Bagaimana penerapan clean architecture pada aplikasi Flutter?
Dalam praktiknya, Clean Architecture pada Flutter dapat diimplementasikan dengan memecah kode menjadi beberapa paket, seperti domain, data, dan presentasi. Setiap paket memiliki tanggung jawab unik yang bervariasi sesuai dengan lapisan yang digunakan.

5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step! (bukan hanya sekadar mengikuti tutorial)
Menambahkan Drawer Menu Untuk Navigasi:
- Buka proyek Flutter yang sudah dibuat sebelumnya.
- Buat berkas baru left_drawer.dart dalam direktori widgets.
- Tambahkan kode untuk membuat drawer menu dengan navigasi ke halaman-halaman tertentu.
- Impor halaman-halaman yang akan dimasukkan ke dalam navigasi drawer.
- Tambahkan routing untuk halaman-halaman tersebut di bagian "TODO: Bagian routing".
- Hias drawer dengan menambahkan drawer header di "TODO: Bagian drawer header".
- Implementasikan drawer pada halaman yang ingin ditambahkan drawer.
- Jalankan program untuk melihat hasilnya.
Menambahkan Form dan Elemen Input:
- Buat berkas baru shoplist_form.dart dalam direktori lib.
- Tambahkan form sederhana dengan input field untuk nama produk, harga, dan deskripsi.
- Gunakan widget Form, TextFormField, dan ElevatedButton.
- Implementasikan validasi input, handling perubahan nilai, dan penanganan tombol "Save".
- Munculkan pop-up dialog ketika tombol "Save" ditekan.
- Tambahkan fitur untuk mereset form setelah disimpan.
- Jalankan program dan gunakan form untuk melihat hasilnya.
Memunculkan Data:
- Modifikasi fungsi onPressed untuk menampilkan pop-up dialog dengan data yang telah diisi.
- Implementasikan widget AlertDialog untuk menampilkan data yang telah diisi.
- Gunakan widget TextFormField untuk menerima input nama, harga, dan deskripsi.
- Jalankan program dan lihat hasilnya.
Menambahkan Fitur Navigasi pada Tombol
- Tambahkan fitur navigasi pada tombol di dalam widget ShopItem pada menu.dart.
- Gunakan Navigator.push untuk melakukan navigasi ke halaman lain.
- Gunakan MaterialPageRoute yang mencakup halaman tujuan.
- Jalankan program dan gunakan tombol untuk melihat hasilnya.
Refactoring File
- Pindahkan widget ShopItem ke berkas shop_card.dart dalam direktori widgets.
- Buat folder baru screens dalam direktori lib.
- Pindahkan halaman-halaman yang sudah dibuat sebelumnya ke dalam folder screens.
- Sesuaikan import dan path berkas sesuai perubahan struktur direktori.