1. Aplikasi Penyewaan Kendaraan merupakan aplikasi desktop berbasis Python yang menggunakan GUI Tkinter dan database SQLite. Aplikasi ini dirancang untuk menerapkan konsep Pemrograman Berorientasi Objek (Object Oriented Programming/OOP) secara nyata, khususnya pada pengelolaan data kendaraan, pelanggan, dan transaksi penyewaan. 

2. Tujuan dari pembuatan aplikasi:
   - Menerapkan konsep Object Oriented Programming dalam sebuah aplikasi nyata. 
   - Membuat sistem penyewaan kendaraan yang terintegrasi dengan database. 
   - Menyediakan fitur pengelolaan kendaraan, pelanggan, transaksi sewa, serta login admin. 
   - Menghasilkan aplikasi yang mudah digunakan dan memiliki struktur kode yang rapi. 

3. Daftar spesifikasi Aplikasi:


    <img width="396" height="388" alt="image" src="https://github.com/user-attachments/assets/0709571d-7093-4ede-aeff-94b5d96733de" />


4. Arsitektur Aplikasi:

   <img width="545" height="440" alt="image" src="https://github.com/user-attachments/assets/2f2cd4d0-5cd1-4cf1-9abb-ba32f88718ec" />



Aplikasi menggunakan arsitektur terpisah antara : 
  - Presentation Layer: GUI Tkinter (app.py) 
  - Business Logic Layer: Object OOP (models) 
  - Data Access Layer: DAO (dao.py) 
  - Database Layer: SQLite (database.py

5. Fitur Utama: 
Manajemen Data Kendaraan (CRUD): 
-	Menambahkan data kendaraan (Mobil dan Motor) 
-	Menampilkan daftar kendaraan 
-	Mengubah data kendaraan 
-	Menghapus data kendaraan 
Manajemen Data Pelanggan (CRUD): 
-	Menambahkan data pelanggan 
-	Menampilkan data pelanggan 
-	Mengubah data pelanggan 
-	Menghapus data pelanggan Transaksi Penyewaan Kendaraan: 
-	Memilih pelanggan dan kendaraan 
-	Menentukan tanggal dan durasi sewa 
-	Menentukan tanggal dan durasi sewa 
Perhitungan Biaya Otomatis (OOP & Polymorphism): 
-	Mobil: biaya sewa + asuransi tetap - Motor: diskon otomatis untuk sewa diatas 7 hari Penyimpanan Data Permanen: 
-	Semua data disimpan ke database SQLite Login Admin: 
-	Akses aplikasi dibatasi menggunakan akun admin Cetak Struk Transaksi: 
-	Menampilkan struk penyewaan 
-	Menyimpan struk dalam bentuk file .txt 

6.	Komponen Data:


   <img width="541" height="536" alt="image" src="https://github.com/user-attachments/assets/24012085-c0a5-4602-9d7f-80a8e8e8b4c7" />



7. Diagram Proses:
 <img width="814" height="831" alt="image" src="https://github.com/user-attachments/assets/ecb36a28-5c09-472c-896f-703fbdc59b87" />

Keterangan: 
1.	Inisialisasi Aplikasi (Start) 
-	Mulai: Program dijalankan dan melakukan inisialisasi awal. 
-	Login Admin: Sistem menampilkan form login (username & password). 
-	Validasi Login: Sistem memeriksa kredensial. Jika valid, admin masuk ke menu utama. 
-	Tampilkan Antarmuka Utama: GUI muncul dengan tiga tab utama: Kendaraan, Pelanggan, dan Transaksi Sewa. 
2.	Alur Tambah/Ubah/Hapus Kendaraan 
-	Tambah Kendaraan: Admin mengisi form (Tipe, Plat, Merk, Tarif/Hari). 
-	Validasi Data: Sistem mengecek format input dan kelengkapan. 
-	Simpan Kendaraan: Jika valid, data disimpan ke database dan tabel kendaraan diperbarui otomatis. 
-	Ubah Kendaraan: Admin memilih data di tabel, mengedit form, lalu menyimpan perubahan ke database. 
-	Hapus Kendaraan: Admin memilih data di tabel, sistem menampilkan konfirmasi, lalu menghapus data jika disetujui. 
-	Clear Form: Admin dapat mengosongkan form untuk input baru. 
3.	Alur Tambah/Ubah/Hapus Pelanggan 
-	Tambah Pelanggan: Admin mengisi form (Nama, Telp). 
-	Validasi Data: Sistem mengecek format input dan kelengkapan. 
-	Simpan Pelanggan: Jika valid, data disimpan ke database dan tabel pelanggan diperbarui otomatis. 
-	Ubah Pelanggan: Admin memilih data di tabel, mengedit form, lalu menyimpan perubahan ke database. 
-	Hapus Pelanggan: Admin memilih data di tabel, sistem menampilkan konfirmasi, lalu menghapus data jika disetujui. 
-	Clear Form: Admin dapat mengosongkan form untuk input baru. 
4.	Alur Transaksi Penyewaan Kendaraan 
-	Pilih Pelanggan & Kendaraan: Admin memilih data dari combo box. 
-	Isi Tanggal & Durasi: Admin menentukan tanggal sewa dan lama sewa (hari). 
-	Hitung Total Biaya: Sistem otomatis menghitung total biaya berdasarkan tarif/hari × durasi. 
-	Simpan Transaksi: Jika valid, data transaksi disimpan ke database dan tabel transaksi diperbarui. 
-	Cetak Struk: Admin memilih transaksi dan sistem mencetak struk sebagai bukti sewa. 
5.	Akhir Program (Finish) 
-	Selesai: Semua aksi pengguna telah diproses. 
-	Kondisi Siap/Tutup: Aplikasi kembali ke keadaan siap digunakan untuk transaksi berikutnya atau ditutup. 
 

 



