# Middleware 🛠️

## Apa itu Middleware? 🤔

Middleware adalah fungsi khusus yang berada di antara permintaan (request) dari client dan respons (response) dari server. Middleware menjalankan tugas penting seperti memeriksa otorisasi pengguna, validasi data, atau mencatat log aktivitas.

### Tujuan 🎯

Folder ini berisi fungsi-fungsi middleware yang membantu menangani tugas-tugas spesifik, seperti:

- **Autentikasi:** Memastikan bahwa pengguna adalah benar sesuai identitasnya.
- **Validasi:** Memeriksa bahwa data yang masuk sudah benar dan aman.

### Struktur 🗂️

Folder ini berisi file-file middleware berikut:

- **`admin.ts`**: File ini memeriksa apakah pengguna memiliki hak admin dengan memverifikasi kredensial terhadap variabel lingkungan 🔑
- **`captcha.ts`**: File ini memastikan Google ReCAPTCHA v2 telah diselesaikan untuk mencegah serangan bot 🤖

### Cara Kerja Middleware 🔄

Setiap file middleware mengekspor fungsi yang dapat digunakan untuk:

1. **Validasi Permintaan:** Memastikan permintaan memenuhi kriteria tertentu sebelum diproses.
2. **Autentikasi Pengguna:** Memeriksa apakah pengguna memiliki izin untuk mengakses resource tertentu.
3. **Mencatat Log:** Merekam detail permintaan untuk debugging atau monitoring.

Jelajahi fungsi-fungsi middleware ini untuk melihat bagaimana mereka dapat membuat aplikasi Anda lebih aman dan andal! 🔍
