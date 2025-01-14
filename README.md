# Tugas8-uas

## Membuat database akademik
![Screenshot (40)](https://github.com/user-attachments/assets/3c4a6d5f-297a-4457-83a9-38e803f2e68c)

## Memasukan data mahasiswa ke form mahasiswa
![Screenshot (41)](https://github.com/user-attachments/assets/66dd96eb-fbc1-4ca9-8a96-bf0cfdfc241e)

## Tampilan akan seperti ini jika data telah disimpan
![Screenshot (42)](https://github.com/user-attachments/assets/8aaa0a1f-edb6-4dd4-bb68-88209995c83a)

## Memasukan nilai mahasiswa
![Screenshot (43)](https://github.com/user-attachments/assets/74d93761-fd16-40a3-a9b2-f704f9e02ded)

## Tampilan akan seperti ini jika nilai berhasil disimpan
![Screenshot (44)](https://github.com/user-attachments/assets/38297412-657c-409b-b851-4ba878c8655e)

## Tampilan nilai yang sudah disimpan
![Screenshot (45)](https://github.com/user-attachments/assets/0c943fef-822e-4503-94de-659c50092363)

> Proyek ini adalah sebuah aplikasi yang dirancang untuk membantu dalam pengelolaan data mahasiswa dan nilai mereka. Aplikasi ini dibangun menggunakan bahasa pemrograman Java dan menerapkan arsitektur Model-View-Controller (MVC). Mari kita bahas lebih dalam mengenai komponen-komponen utama dari aplikasi ini.

### 1. Struktur Proyek
Aplikasi ini memiliki struktur yang terorganisir dengan baik, yang terdiri dari tiga komponen utama:
* Model: Bagian ini berfungsi untuk merepresentasikan data dan logika bisnis. Di sini terdapat kelas-kelas seperti Mahasiswa dan Nilai yang menyimpan informasi tentang mahasiswa dan nilai mereka.
* View: Ini adalah antarmuka pengguna yang berfungsi untuk menampilkan data kepada pengguna. Contohnya adalah FormMahasiswa dan FormNilai, yang memungkinkan pengguna untuk berinteraksi dengan data.
* Controller: Komponen ini bertindak sebagai penghubung antara model dan view. Kelas-kelas seperti MahasiswaController dan NilaiController mengatur alur data dan logika ketika pengguna berinteraksi dengan antarmuka.
  
### 2. Kelas Utama
Main.java: Kelas ini adalah titik awal dari aplikasi. Di sini, koneksi ke database dibuat, dan objek model serta view diinisialisasi. Controller juga diinstansiasi untuk menghubungkan model dan view, sehingga aplikasi dapat berfungsi dengan baik.

### 3. Model
* Mahasiswa.java: Kelas ini merepresentasikan entitas mahasiswa dengan atribut seperti ID, NIM, nama, jurusan, dan angkatan. Ini adalah struktur dasar yang menyimpan informasi penting tentang mahasiswa.
* Nilai.java: Kelas ini merepresentasikan entitas nilai, yang mencakup ID, ID mahasiswa, mata kuliah, semester, dan nilai. Ini membantu dalam menyimpan informasi akademis mahasiswa.
* MahasiswaModel.java: Kelas ini mengelola operasi database untuk mahasiswa, seperti mencari, menambah, memperbarui, dan menghapus data mahasiswa.
* NilaiModel.java: Kelas ini mengelola operasi database untuk nilai, termasuk mencari nilai berdasarkan ID mahasiswa.

### 4. View
* FormMahasiswa.java: Kelas ini menyediakan antarmuka pengguna untuk mengelola data mahasiswa. Pengguna dapat menambah, menghapus, dan melihat daftar mahasiswa dengan mudah.
* FormNilai.java: Kelas ini menyediakan antarmuka pengguna untuk mengelola data nilai mahasiswa. Pengguna dapat menambah, menghapus, dan melihat nilai yang terkait dengan mahasiswa tertentu.

### 5. Controller
* MahasiswaController.java: Kelas ini mengatur interaksi antara model mahasiswa dan view. Ia menangani event dari view, seperti menyimpan dan menghapus data mahasiswa, serta memperbarui tampilan tabel mahasiswa.
* NilaiController.java: Kelas ini mengatur interaksi antara model nilai dan view. Ia menangani event dari view untuk menyimpan dan menghapus nilai mahasiswa, serta memperbarui tampilan tabel nilai.

### 6. Database
* Database.java: Kelas ini bertanggung jawab untuk mengelola koneksi ke database MySQL. Ia menyediakan metode untuk mendapatkan koneksi yang dapat digunakan oleh model, sehingga aplikasi dapat berinteraksi dengan database.

### 7. Penggunaan
Aplikasi ini memungkinkan pengguna untuk:
* Menambah dan mengelola data mahasiswa dengan mudah.
* Melihat dan mengelola nilai mahasiswa secara efisien.
* Menggunakan antarmuka grafis yang intuitif untuk berinteraksi dengan data, sehingga pengguna tidak perlu berurusan dengan perintah-perintah kompleks.

### 8. File Konfigurasi
launch.json dan settings.json: File ini digunakan untuk konfigurasi proyek dalam lingkungan pengembangan, seperti pengaturan library dan konfigurasi peluncuran aplikasi. Ini membantu dalam memudahkan pengembangan dan pengujian aplikasi.

### Kesimpulan
> Proyek ini adalah aplikasi manajemen data mahasiswa yang terstruktur dengan baik, menggunakan prinsip-prinsip pemrograman berorientasi objek dan arsitektur MVC. Dengan memisahkan model, view, dan controller, aplikasi ini menjadi lebih mudah untuk dikembangkan dan dipelihara. Aplikasi ini tidak hanya membantu dalam pengelolaan data, tetapi juga memberikan pengalaman pengguna yang baik melalui antarmuka yang ramah pengguna.
