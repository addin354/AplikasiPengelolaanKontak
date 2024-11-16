# Aplikasi Pengelolaan Kontak (Contact Management)
## Identitas

- Nama : Addin Husnan Nadhari
- Npm : 2210010037
- Kelas : 5B Nonreg Banjarmasin
  
## Deskripsi Proyek
Aplikasi **Pengelolaan Kontak** adalah aplikasi berbasis Java Swing yang digunakan untuk mengelola daftar kontak. Aplikasi ini memungkinkan pengguna untuk menambahkan, mengedit, menghapus, mencari, dan memfilter kontak berdasarkan kategori tertentu.

## Fitur Utama
- **Menambah Kontak**: Pengguna dapat menambahkan kontak baru dengan informasi seperti nama, nomor telepon, dan kategori.
- **Mengedit Kontak**: Kontak yang ada dapat diperbarui oleh pengguna.
- **Menghapus Kontak**: Pengguna dapat menghapus kontak yang tidak diperlukan lagi.
- **Mencari Kontak**: Fasilitas pencarian untuk menemukan kontak berdasarkan nama atau nomor telepon.
- **Filter Berdasarkan Kategori**: Kontak dapat difilter berdasarkan kategori (misalnya: Keluarga, Teman, Pekerjaan, dll.).
- **Antarmuka Tabel**: Semua data kontak ditampilkan dalam tabel interaktif.

## Teknologi yang Digunakan
- **Java SE**: Digunakan untuk membangun aplikasi.
- **Java Swing**: Library GUI untuk membuat antarmuka pengguna.
- **JDBC**: Digunakan untuk menghubungkan aplikasi dengan database.
- **SQLite**: Basis data ringan untuk menyimpan data kontak.

## Prasyarat
- **JDK**: Pastikan JDK (Java Development Kit) terinstal di komputer Anda.
- **SQLite Database**: File database SQLite untuk menyimpan data kontak.

## Instalasi
1. Clone atau unduh proyek ini ke komputer Anda.
2. Pastikan Anda memiliki database SQLite dengan nama `contacts.db`. Struktur tabel harus seperti berikut:
    ```sql
    CREATE TABLE contacts (
        id INTEGER PRIMARY KEY AUTOINCREMENT,
        nama TEXT NOT NULL,
        nomor_telepon TEXT NOT NULL,
        kategori TEXT NOT NULL
    );
    ```
3. Pastikan file database berada di lokasi yang sesuai dengan konfigurasi di kelas `DatabaseHelper`.

## Cara Menggunakan
1. Jalankan program dengan menjalankan file `PengelolaanKontakFrame` sebagai program utama.
2. Gunakan antarmuka untuk:
    - Menambahkan kontak dengan mengisi nama, nomor telepon, dan memilih kategori.
    - Mengedit kontak yang ada dengan memilih dari tabel, memperbarui informasi, lalu menekan tombol *Edit*.
    - Menghapus kontak yang dipilih dari tabel.
    - Mencari kontak berdasarkan nama atau nomor telepon.
    - Memfilter daftar kontak berdasarkan kategori dari menu dropdown.

## Struktur Proyek
- **`PengelolaanKontakFrame`**: Frame utama aplikasi yang berisi logika dan antarmuka.
- **`DatabaseHelper`**: Kelas utilitas untuk koneksi ke database SQLite.
- **GUI Components**: Tabel, tombol, dan komponen lain yang diatur menggunakan Java Swing.

