# Simple LMS - Django & PostgreSQL with Docker

Proyek ini adalah inisialisasi awal untuk sistem Simple LMS menggunakan framework Django dan database PostgreSQL, yang seluruhnya berjalan di dalam container Docker.

## 🎯 Learning Objectives

- Containerization aplikasi Python/Django menggunakan Dockerfile.
- Orchestration service Web dan Database menggunakan Docker Compose.
- Konfigurasi koneksi database PostgreSQL pada Django.
- Implementasi environment variables untuk keamanan konfigurasi.

## 📂 Project Structure

simple-lms/
├── config/ # Folder konfigurasi utama Django
│ ├── settings.py
│ ├── urls.py
│ └── wsgi.py
├── manage.py # Entry point Django
├── Dockerfile # Instruksi build image Python
├── docker-compose.yml # Definisi services (Web & DB)
├── requirements.txt # Daftar library Python
└── README.md # Dokumentasi proyek
