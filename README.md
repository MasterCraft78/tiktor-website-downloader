# 🎵 TikTok Downloader - No Watermark

Download video dan gambar TikTok tanpa watermark secara gratis menggunakan API publik.

![TikTok Downloader](https://img.shields.io/badge/TikTok-Downloader-blue?logo=tiktok)
![No Watermark](https://img.shields.io/badge/No-Watermark-green)
![Free API](https://img.shields.io/badge/Free-API-orange)
![AI Powered](https://img.shields.io/badge/Made%20with-AI-purple)

## ✨ Fitur

- 🎬 **Download Video Tanpa Watermark** - Dapatkan video TikTok bersih tanpa logo
- 📺 **Pilih Resolusi Video** - Pilih kualitas HD, SD, atau Low sesuai kebutuhan
- 🖼️ **Support Gambar/Slide** - Download semua gambar dari postingan slide
- 🎵 **Download MP3 Audio** - Ekstrak audio dari video TikTok dalam format MP3
- ⚡ **Proses Cepat** - Menggunakan free API yang responsif
- 🆓 **100% Gratis** - Tidak perlu registrasi atau pembayaran
- 📱 **Responsive** - Bekerja di semua device (desktop, tablet, mobile)
- 🤖 **AI Powered** - Dibuat dengan bantuan AI

## 📁 Struktur File

```
/workspace
├── index.html          # Main website (HTML + CSS + JavaScript)
└── README.md           # Dokumentasi project
```

## 🚀 Cara Menggunakan

### Metode 1: Langsung Buka File
1. Buka file `index.html` di browser Anda (Chrome, Firefox, Safari, dll)
2. Copy URL video TikTok yang ingin didownload
3. Paste URL ke dalam form input
4. Klik tombol "Download Sekarang"
5. Pilih jenis download yang diinginkan (video no watermark, with watermark, audio, atau gambar)

### Metode 2: Host Secara Online
Anda bisa menghost website ini secara gratis di:
- **GitHub Pages**
- **Netlify**
- **Vercel**
- **Cloudflare Pages**

Contoh deploy ke GitHub Pages:
```bash
# Commit file ke repository
git add .
git commit -m "Add TikTok Downloader"
git push origin main
```

Kemudian aktifkan GitHub Pages di repository settings.

## 🔧 API yang Digunakan

Website ini menggunakan **TiklyDown API** (gratis):
- Base URL: `https://api.tiklydown.app/api/download`
- Method: GET
- Parameter: `url` (URL video TikTok)

### Contoh Request API
```javascript
fetch('https://api.tiklydown.app/api/download?url=https://www.tiktok.com/@user/video/123456789')
    .then(response => response.json())
    .then(data => console.log(data));
```

### Response Format
```json
{
    "status": 200,
    "msg": "Success",
    "data": {
        "id": "video_id",
        "title": "Video title",
        "cover": "thumbnail_url",
        "play": "no_watermark_video_url",
        "hdplay": "hd_no_watermark_video_url",
        "wmplay": "with_watermark_video_url",
        "music": "audio_url",
        "duration": 30,
        "author": {
            "username": "username",
            "nickname": "Display Name"
        },
        "playCount": 1000000,
        "diggCount": 50000,
        "images": [
            {"url": "image1.jpg"},
            {"url": "image2.jpg"}
        ]
    }
}
```

### Keterangan Field:
- `play` - URL video tanpa watermark (kualitas standar)
- `hdplay` - URL video tanpa watermark (kualitas HD)
- `wmplay` - URL video dengan watermark (kualitas rendah)
- `music` - URL audio/mp3 dari video
- `images` - Array berisi URL gambar (untuk postingan slide)

## 🛠️ Customization

### Mengganti API
Jika Anda ingin menggunakan API lain, edit bagian ini di `index.html`:

```javascript
// Line 293
const API_BASE = 'https://api.tiklydown.app/api/download';
```

Ganti dengan endpoint API pilihan Anda.

### Mengubah Tampilan
Edit CSS di bagian `<style>` dalam file `index.html` untuk menyesuaikan:
- Warna tema
- Font
- Layout
- Animasi

## ⚠️ Catatan Penting

1. **API Limitations**: Free API mungkin memiliki rate limit atau downtime
2. **CORS**: Beberapa browser mungkin memblokir request karena CORS policy
3. **Legal**: Pastikan Anda menggunakan downloader ini sesuai dengan Terms of Service TikTok
4. **Personal Use**: Gunakan hanya untuk keperluan pribadi, bukan komersial

## 🔒 Disclaimer

- Tool ini dibuat untuk tujuan edukasi dan pembelajaran
- Hormati hak cipta dan konten creator
- Jangan gunakan untuk mendownload konten ilegal
- Developer tidak bertanggung jawab atas penyalahgunaan tool ini

## 📄 License

Project ini dibuat dengan ❤️ menggunakan AI dan tersedia secara gratis.

## 🤝 Kontribusi

Feel free to fork, modify, dan improve project ini!

---

**Dibuat dengan ❤️ 🤖 oleh AI Assistant**
