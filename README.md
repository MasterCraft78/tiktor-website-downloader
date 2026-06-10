# 🎵 TikTok Downloader - No Watermark

Website downloader video dan gambar TikTok tanpa watermark dengan dukungan **13 FREE API** dan fitur **AI Image Upscaler**.

![TikTok Downloader](https://img.shields.io/badge/TikTok-Downloader-fe2c55?style=for-the-badge&logo=tiktok)
![API Count](https://img.shields.io/badge/APIs-13%20Free-25f4ee?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

## ✨ Fitur Utama

### 🎬 Download Video
- ✅ **Support Semua Resolusi**: 4K, 2K, HD, SD
- ✅ **Tanpa Watermark**: Download video bersih
- ✅ **Multi API System**: 13 API gratis sebagai fallback
- ✅ **Auto Detect**: Mendeteksi resolusi tersedia

### 🎵 Download Audio
- ✅ **MP3 Extract**: Download audio terpisah dari video
- ✅ **High Quality**: Kualitas audio terbaik

### 🖼️ Download Gambar & Upscale AI
- ✅ **Slide Images**: Download semua gambar dari postingan slide
- ✅ **AI Waifu2x**: Upscale menggunakan Waifu2x gratis
- ✅ **2x Zoom**: Client-side bicubic scaling
- ✅ **HD Filter**: Contrast & saturation boost

### 📱 UI/UX Modern
- ✅ **TikTok Style**: Desain mirip aplikasi TikTok
- ✅ **Responsive**: Mobile, Tablet, Desktop
- ✅ **Dark Mode**: Tampilan gelap nyaman di mata
- ✅ **Tutorial**: Panduan lengkap cara penggunaan

## 🔗 Daftar 13 Free API

Website ini menggunakan sistem multi-API untuk memastikan ketersediaan:

| # | API Name | Type | Status |
|---|----------|------|--------|
| 1 | TiklyDown | Direct | ✅ Primary |
| 2 | TikWM | Direct | ✅ Backup 1 |
| 3 | LoveTik | Direct | ✅ Backup 2 |
| 4 | TikAPI | Direct | ✅ Backup 3 |
| 5 | SSSTik | Proxy | ✅ Fallback |
| 6 | SnapTik | Proxy | ✅ Fallback |
| 7 | TikMate | Proxy | ✅ Fallback |
| 8 | SaveTT | Proxy | ✅ Fallback |
| 9 | TikDownload | Proxy | ✅ Fallback |
| 10 | GoCoo | Proxy | ✅ Fallback |
| 11 | ExpertsPHP | Proxy | ✅ Fallback |
| 12 | AllSave | Proxy | ✅ Fallback |
| 13 | FastDl | Proxy | ✅ Fallback |

*Catatan: API yang menggunakan proxy melalui `corsproxy.io` untuk mengatasi CORS browser.*

## 🚀 Cara Menggunakan

### Metode 1: Langsung di Browser
1. Buka file `index.html` di browser (Chrome, Firefox, Edge, Safari)
2. Copy link video TikTok dari aplikasi
3. Paste link di kolom input (atau klik tombol paste)
4. Klik **"Download Sekarang"**
5. Tunggu proses fetching dari API
6. Pilih resolusi yang diinginkan (4K/2K/HD/SD)
7. Klik **"Download Video"** atau **"Download MP3"**

### Metode 2: Upload Gambar untuk Upscale
1. Untuk postingan slide gambar, grid preview akan muncul
2. Pilih metode upscale:
   - **✨ AI Waifu**: Membuka Waifu2x.jp untuk upscale AI gratis
   - **🔍 2x Zoom**: Preview dengan zoom 2x instan
   - **💎 HD Filter**: Preview dengan filter HD instan
3. Klik kanan pada gambar hasil upscale → **"Save Image As"**

## 📁 Struktur File

```
/workspace
├── index.html      # Main website (HTML + CSS + JS)
└── README.md       # Dokumentasi ini
```

## 🛠️ Teknologi

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Font**: DM Sans (Google Fonts)
- **Icons**: Font Awesome 6
- **APIs**: 13 Free TikTok APIs
- **Proxy**: corsproxy.io (untuk bypass CORS)
- **Upscale**: Waifu2x (External), Client-side filters

## ⚙️ Cara Kerja Multi-API

```javascript
// Alur proses:
1. User input URL TikTok
2. Loop melalui 13 API secara berurutan
3. Timeout 8 detik per API
4. Jika API 1 gagal → coba API 2
5. Jika berhasil → normalize data → tampilkan hasil
6. Jika semua gagal → tampilkan error
```

## 🎨 Customization

### Mengubah Warna Tema
Edit variabel CSS di `<style>`:

```css
:root {
    --tik-black: #010101;      /* Background utama */
    --tik-red: #fe2c55;        /* Warna merah TikTok */
    --tik-cyan: #25f4ee;       /* Warna cyan TikTok */
}
```

### Menambah API Baru
Tambahkan ke array `API_LIST` di JavaScript:

```javascript
const API_LIST = [
    // ... existing APIs
    { name: "NewAPI", url: "https://newapi.com/download?url={URL}" }
];
```

## ⚠️ Catatan Penting

1. **CORS Issues**: Beberapa API mungkin diblokir oleh browser karena CORS. Website menggunakan `corsproxy.io` sebagai solusi.
2. **Private Accounts**: Video dari akun private tidak bisa didownload.
3. **API Limits**: API gratis memiliki limit request. Jika gagal, tunggu beberapa saat.
4. **Educational Use**: Tool ini untuk tujuan edukasi. Hormati hak cipta konten creator.

## 🐛 Troubleshooting

| Masalah | Solusi |
|---------|--------|
| Download tidak mulai | Klik kanan video → "Save Video As" |
| Semua API gagal | Cek koneksi internet, pastikan link publik |
| CORS Error | Gunakan browser dengan disable CORS atau extension |
| Video blur | Pilih resolusi HD/2K/4K jika tersedia |

## 📄 License

MIT License - Dibuat dengan ❤️ menggunakan AI

## 🙏 Credits

- **TiklyDown API**
- **TikWM API**
- **LoveTik API**
- **Waifu2x** untuk image upscaling
- **Font Awesome** untuk icons
- **Google Fonts** untuk typography

---

**Dibuat dengan 🤖 AI Assistant | 100% FREE & OPEN SOURCE**
