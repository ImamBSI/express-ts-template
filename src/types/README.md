# Folder `types`

Folder ini berisi definisi tipe data (type definitions) dan interface yang digunakan di seluruh project ini. Dengan memisahkan tipe-tipe ke dalam folder khusus, kode menjadi lebih terstruktur, mudah dipelihara, dan meningkatkan konsistensi penggunaan tipe di berbagai modul.

Semua file di dalam folder ini ditulis menggunakan TypeScript (`.ts`) dan bertujuan untuk:
- Mendefinisikan tipe data custom, interface, dan tipe global yang dibutuhkan aplikasi.
- Memudahkan reusabilitas tipe di berbagai bagian project.
- Mengurangi duplikasi tipe dan meminimalisir potensi bug terkait tipe data.

Contoh isi folder ini bisa berupa:
- Interface untuk request/response API
- Tipe data untuk entitas database
- Enum dan union type untuk value tertentu

> **Catatan:** Jangan menuliskan implementasi logika di folder ini, hanya definisi tipe saja.
