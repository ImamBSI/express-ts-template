# Folder Konfigurasi 🗂️

Folder ini berisi file-file konfigurasi penting untuk pengaturan aplikasi backend.

## sequelize.ts 🔧

File ini mengatur konfigurasi database untuk berbagai tahap pengembangan. File ini membantu aplikasi terhubung ke database sesuai dengan lingkungan yang digunakan, baik secara lokal, staging, maupun produksi.

### Variabel Lingkungan 🌱

Untuk menjaga keamanan informasi sensitif seperti kredensial database, kita menggunakan variabel lingkungan (environment variables). Sebelum menjalankan aplikasi, pastikan variabel berikut sudah diatur di lingkungan Anda:

- `DB_USERNAME`: Username Database Anda 🧑‍💻
- `DB_PASSWORD`: Password Database Anda 🔑
- `DB_NAME`: Nama database Database Anda 📦
- `DB_URL`: URL koneksi Database yang digunakan pada lingkungan staging dan produksi 🌐

### Pengaturan Konfigurasi ⚙️

Konfigurasi dibagi menjadi tiga bagian utama:

1. **Development:** Pengaturan saat Anda bekerja di komputer lokal. Menggunakan variabel lingkungan untuk mendapatkan username, password, dan nama database.

2. **Staging:** Pengaturan untuk lingkungan pengujian yang menyerupai produksi. Menggunakan variabel `DB_URL` untuk koneksi database dan memastikan koneksi aman dengan enkripsi SSL.

3. **Production:** Pengaturan untuk lingkungan produksi di mana aplikasi digunakan oleh pengguna sebenarnya. Seperti staging, menggunakan variabel `DB_URL` dan enkripsi SSL untuk koneksi yang aman.

Perbarui pengaturan dan variabel lingkungan ini sesuai kebutuhan proyek Anda. 🛠️
