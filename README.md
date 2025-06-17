## 🌐 Project Cloud Computing

Ini adalah project Docker sederhana untuk deployment web statis menggunakan image `nginx:alpine`.

### 📁 Struktur File:
- `index.html` — Halaman utama website.
- `foto.jpg.jpeg` — Gambar yang ditampilkan di halaman.
- `nusa.webp` — Gambar tambahan dalam format WebP.

### 🐳 Dockerfile
Base image: `nginx:alpine`

```dockerfile
FROM nginx:alpine
COPY index.html /usr/share/nginx/html/index.html
COPY foto.jpg.jpeg /usr/share/nginx/html/foto.jpg.jpeg
COPY nusa.webp /usr/share/nginx/html/nusa.webp
