# 🎨 Modern Portfolio Website

Website portfolio modern yang dibangun dengan **HTML, CSS, dan JavaScript Native** tanpa framework atau library eksternal. Desain clean, modern, dan fully responsive.

## ✨ Features

### 🎯 Komponen Utama

- **Navigation Bar** - Sticky navbar dengan backdrop blur dan smooth scroll
- **Hero Section** - Animated hero dengan gradient background dan floating profile
- **About Section** - Deskripsi diri dengan list hobi dan minat
- **Skills Section** - 6+ skill cards dengan icon dan deskripsi
- **Contact Section** - Multiple contact methods dengan hover effects
- **Footer** - Copyright dan informasi tambahan

### 🚀 Fitur Modern

- ✅ Fully Responsive (Mobile, Tablet, Desktop)
- ✅ Smooth Scroll Navigation
- ✅ Scroll Animations (Fade in on scroll)
- ✅ Gradient Background dengan animated pattern
- ✅ Glass Morphism Effect pada navbar
- ✅ Hover Interactions & Micro-animations
- ✅ Modern Card Design
- ✅ SEO Friendly Structure
- ✅ Fast Loading (No dependencies)
- ✅ Cross-browser Compatible

---

## 📁 Struktur File

```
portfolio-website/
├── index.html          # File utama (all-in-one)
├── README.md          # Dokumentasi ini
└── assets/            # (Optional) Folder untuk gambar
    └── profile.jpg    # Foto profil Anda
    └── style.css    # File CSS
    └── script.js   # File JavaScript
```

**Note:** Website ini menggunakan single file HTML dengan CSS dan JavaScript embedded untuk kemudahan deployment.

---

## 🚀 Cara Menggunakan

### 1. Download / Clone

```bash
# Clone repository (jika menggunakan Git)
git clone https://github.com/ghulamch/PenugasanFantechDay1.git

# Atau download file index.html langsung
```

### 2. Personalisasi Konten

Buka `index.html` dan edit bagian-bagian berikut:

#### **Hero Section** (Baris ~230)
```html
<h1>Nama Anda</h1>  <!-- Ganti dengan nama Anda -->
<p>Web Developer & Designer | Passionate about...</p>  <!-- Ganti tagline -->
```

#### **Profile Image** (Baris ~227)
```html
<!-- Ganti emoji dengan foto asli -->
<div class="profile-img">👤</div>

<!-- Menjadi: -->
<img src="assets/profile.jpg" alt="Profile" class="profile-img">
```

#### **About Section** (Baris ~240)
```html
<p>
    Halo! Saya adalah seorang web developer...  <!-- Edit deskripsi Anda -->
</p>
```

#### **Hobi & Minat** (Baris ~250)
```html
<li><strong>💻</strong> Coding & Programming</li>
<!-- Tambah/edit sesuai hobi Anda -->
```

#### **Skills Section** (Baris ~265)
```html
<div class="skill-card">
    <div class="skill-icon">🌐</div>
    <h3>Web Development</h3>  <!-- Edit skill Anda -->
    <p>HTML, CSS, JavaScript...</p>
</div>
```

#### **Contact Section** (Baris ~310)
```html
<a href="mailto:your.email@example.com">your.email@example.com</a>
<!-- Ganti dengan email/kontak asli Anda -->
```

#### **Footer** (Baris ~340)
```html
<p>&copy; 2025 Nama Anda. All Rights Reserved.</p>
```

### 3. Jalankan Website

**Opsi A: Langsung buka di browser**
```bash
# Double-click index.html
# Atau klik kanan > Open with > Browser
```

**Opsi B: Gunakan Local Server (Recommended)**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (jika ada npx)
npx serve

# PHP
php -S localhost:8000
```

Kemudian buka: `http://localhost:8000`

---

## 🎨 Customization Guide

### Mengubah Warna Theme

Edit CSS variables di bagian `:root` (Baris ~13):

```css
:root {
    --primary: #6366f1;        /* Warna utama */
    --primary-dark: #4f46e5;   /* Warna primary lebih gelap */
    --secondary: #ec4899;      /* Warna aksen */
    --dark: #1e293b;           /* Warna teks gelap */
    --light: #f8fafc;          /* Background terang */
    --gray: #64748b;           /* Warna abu-abu */
    --gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}
```

**Contoh Theme Alternatif:**

```css
/* Blue Theme */
--primary: #3b82f6;
--gradient: linear-gradient(135deg, #3b82f6 0%, #1e40af 100%);

/* Green Theme */
--primary: #10b981;
--gradient: linear-gradient(135deg, #10b981 0%, #047857 100%);

/* Orange Theme */
--primary: #f97316;
--gradient: linear-gradient(135deg, #f97316 0%, #ea580c 100%);
```

### Menambah Section Baru

```html
<!-- Tambahkan section baru sebelum footer -->
<section id="projects" class="projects">
    <h2 class="section-title">My Projects</h2>
    <div class="projects-grid">
        <!-- Konten project Anda -->
    </div>
</section>
```

Jangan lupa tambahkan link di navbar:
```html
<li><a href="#projects">Projects</a></li>
```

### Mengubah Font

```css
body {
    font-family: 'Your-Font', 'Segoe UI', sans-serif;
}
```

Atau gunakan Google Fonts:
```html
<!-- Tambahkan di <head> -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">

<!-- Update CSS -->
<style>
body {
    font-family: 'Poppins', sans-serif;
}
</style>
```

---

## 📱 Responsive Breakpoints

Website ini responsive dengan breakpoint berikut:

| Device | Breakpoint | Layout |
|--------|-----------|---------|
| Mobile | ≤ 480px | Single column, compact spacing |
| Tablet | ≤ 768px | 2 columns, adjusted grid |
| Desktop | > 768px | Full multi-column layout |

---

## 🌐 Deployment

### Deploy ke GitHub Pages

1. **Buat repository baru di GitHub**
2. **Upload file `index.html`**
3. **Aktifkan GitHub Pages:**
   - Settings > Pages
   - Source: main branch
   - Save

Website akan live di: `https://username.github.io/repository-name/`

### Deploy ke Netlify

1. Drag & drop folder ke [Netlify Drop](https://app.netlify.com/drop)
2. Website langsung live!

### Deploy ke Vercel

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

### Deploy ke Hosting Tradisional

Upload `index.html` dan folder `assets/` ke public_html via FTP/cPanel.

---

## 🛠️ Troubleshooting

### Gambar tidak muncul
- Pastikan path gambar benar: `assets/profile.jpg`
- Check case-sensitive (Linux/Mac): `Profile.jpg` ≠ `profile.jpg`

### Animation tidak smooth
- Pastikan menggunakan browser modern (Chrome, Firefox, Safari, Edge)
- Clear browser cache: `Ctrl + Shift + R`

### Navbar tidak sticky
- Check apakah ada CSS conflicting
- Pastikan `position: fixed` tidak ter-override

### Layout berantakan di mobile
- Buka browser DevTools (F12)
- Test di different screen sizes
- Check responsive CSS di media queries

---


## 💡 Tips & Best Practices

### Content Writing
- **Be Authentic** - Tulis dengan gaya bahasa Anda sendiri
- **Keep it Concise** - Paragraf pendek lebih mudah dibaca
- **Use Action Words** - "Building", "Creating", "Developing"
- **Showcase Results** - Fokus pada achievement, bukan hanya task

### Design
- **Consistent Spacing** - Gunakan multiples of 8px (8, 16, 24, 32, 40)
- **Readable Font Size** - Minimum 16px untuk body text
- **Contrast Ratio** - Min 4.5:1 untuk accessibility
- **White Space** - Jangan takut ruang kosong, it's important!

---

## 🤝 Contributing

Punya ide untuk improve website ini? 

1. Fork repository
2. Buat branch baru (`git checkout -b feature/improvement`)
3. Commit changes (`git commit -m 'Add some feature'`)
4. Push ke branch (`git push origin feature/improvement`)
5. Buat Pull Request

---

## 📄 License

Website template ini **Free to Use** untuk personal dan commercial projects.

**Attribution appreciated but not required!** 😊

---

## 📞 Support

Butuh bantuan atau punya pertanyaan?

- 📧 Email: mail@ghulam.my.id
- 💬 LinkedIn: [Your Profile](https://linkedin.com/in/yourprofile)
- 🌐 Website Utama: https://ghulam.my.id

---

<div align="center">

**⭐ Star this repo if you found it helpful!**

Made with ❤️ and HTML

© 2025 Ghulam. All Rights Reserved.

</div>