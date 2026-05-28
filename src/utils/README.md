# Utilities 🛠️

## Apa itu Utilities? 🤔

Utilities adalah fungsi dan modul pembantu yang menjalankan tugas-tugas umum di seluruh aplikasi Anda. Utilities membantu berbagai operasi yang tidak langsung berkaitan dengan route API, namun sangat penting untuk fungsionalitas aplikasi secara keseluruhan.

### Tujuan 🎯

Folder `utils` berisi kode yang dapat digunakan kembali untuk:

- **Penanganan File:** Mengarsipkan file dan direktori.
- **Operasi Tanggal:** Memformat tanggal dan timestamp.
- **Penanganan Form:** Membuat dan memanipulasi data form.
- **Operasi JSON:** Transformasi dan manipulasi data JSON.
- **Logging:** Mencatat pesan dan error.
- **Pengiriman Email:** Mengirim email.
- **QR Code:** Membuat QR code.
- **Enkripsi:** Mengamankan data dengan enkripsi.
- **Manajemen Token:** Mengelola JSON Web Token (JWT).

### Struktur 🗂️

Folder ini biasanya berisi file-file berikut:

- **`archiver.ts`**: Untuk mengarsipkan file dan direktori.
- **`dateFormatter.ts`**: Untuk memformat tanggal dan timestamp.
- **`formData.ts`**: Untuk membuat dan memanipulasi data form.
- **`jsonTransformer.ts`**: Untuk transformasi data JSON.
- **`logger.ts`**: Untuk mencatat pesan dan error.
- **`mailer.ts`**: Untuk mengirim email.
- **`qrGenerator.ts`**: Untuk membuat QR code.
- **`quickEncrypt.ts`**: Untuk enkripsi dan dekripsi data.
- **`sendAttachment.ts`**: Untuk mengirim lampiran seperti file CSV.
- **`token.ts`**: Untuk membuat dan memverifikasi JWT.

### Modul dan Fungsi 📚

**Archiver**:

- `zipDirectory`: Mengompres direktori menjadi file ZIP.

**Date Formatter**:

- `dateForFilename`: Membuat string tanggal dengan format YYYY-MM-DD-HH-MM-SS untuk nama file.

**Form Data**:

- `buildFormData`: Membuat objek FormData dari objek JavaScript.
- `jsonToFormData`: Mengubah objek JSON menjadi FormData.

**JSON Transformer**:

- `getNestedValuesString`: Mengambil nilai-nilai nested dari objek JSON sebagai string.

**Logger**:

- `logger`: Menyediakan fungsi logging untuk pesan dan error.

**Mailer**:

- `inboundMailer`: Mengirim email dengan template dan lampiran.

**QR Generator**:

- `qrPNGFile`: Membuat QR code dalam bentuk file PNG.
- `qrSignedPNGFile`: Membuat QR code bertanda tangan dalam bentuk file PNG.

**Quick Encrypt**:

- `generate`: Membuat pasangan public-private key.
- `encrypt`: Mengenkripsi string menggunakan public key.
- `decrypt`: Mendekripsi string menggunakan private key.

**Send Attachment**:

- `sendCSV`: Mengirim file CSV sebagai lampiran email.

**Token**:

- `getJWT`: Membuat JSON Web Token (JWT) dari data.
- `verifyJWT`: Memeriksa validitas JWT.
- `getSignedJWT`: Membuat JWT bertanda tangan dari data.
- `verifySignedJWT`: Memverifikasi JWT bertanda tangan.

### Penggunaan 📖

Untuk menggunakan fungsi atau modul utility, Anda perlu:

1. **Import Modul:** Masukkan ke dalam file JavaScript Anda.
2. **Panggil Fungsi:** Gunakan fungsi yang tersedia sesuai kebutuhan.

Contoh:

```javascript
const { zipDirectory } = require('./utils/archiver');
zipDirectory('path/to/directory', 'path/to/archive.zip');
```
