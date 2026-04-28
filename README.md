# Simple LMS - Django & PostgreSQL with Docker

Proyek ini adalah implementasi pengembangan environment menggunakan Docker untuk membangun sistem Simple LMS berbasis Django. Proyek ini mencakup pengaturan containerization, konfigurasi database PostgreSQL, dan manajemen variabel lingkungan.

## 🎯 Learning Objectives

- Memahami containerization dengan Docker.
- Mampu membuat Dockerfile dan docker-compose.yml yang efisien.
- Setup Django project dengan best practices.
- Konfigurasi koneksi PostgreSQL di dalam Docker.

## 📦 Deliverables & Project Structure

Struktur folder proyek ini mengikuti standar best practice Django di dalam Docker:

```text
simple-lms/
├── config/             # Folder konfigurasi utama Django
│   ├── settings.py     # Konfigurasi database & apps
│   ├── urls.py         # Routing URL utama
│   └── wsgi.py         # Entry point web server
├── manage.py           # Command-line utility Django
├── Dockerfile          # Instruksi build image Python/Django
├── docker-compose.yml  # Definisi services (Web & Database)
├── requirements.txt    # Daftar library Python (Django, Psycopg2)
└── README.md           # Dokumentasi lengkap proyek
🚀 Cara Menjalankan Proyek
Ikuti langkah-langkah berikut untuk menjalankan proyek di lingkungan lokal Anda:
1. Persiapan: Pastikan Docker Desktop sudah aktif di komputer Anda.
2. Build Image: Bangun image aplikasi dari Dockerfile:
docker-compose build
3. Jalankan Service: Jalankan container Django dan PostgreSQL secara background:
docker-compose up -d
4. Migrasi Database: Sinkronkan skema database Django ke PostgreSQL:
docker-compose exec web python manage.py migrate
5. Akses Aplikasi: Buka browser dan akses: http://localhost:8000

⚙️ Environment Variables Configuration
Proyek ini menggunakan variabel lingkungan untuk keamanan dan fleksibilitas konfigurasi di dalam docker-compose.yml:

DB_NAME: lms_db
DB_USER: lms_user
DB_PASSWORD: lms_password
DB_HOST: db
DB_PORT: 5432

👨‍💻 Penulis
Aditya Reyhan Aji Pratama Teknik Informatika - Universitas Dian Nuswantoro
```
