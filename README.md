# 🎨 Website Portofolio Pribadi

Website portofolio modern dengan tema dark elegant + gold accent.

---

## 📁 Struktur File

```
portfolio-web/
├── index.html       ← Halaman utama
├── style.css        ← Semua styling / tampilan
├── script.js        ← Interaktivitas & animasi
├── README.md        ← Panduan ini
└── assets/          ← Letakkan foto & file di sini
    ├── foto-saya.jpg       ← Foto profesional kamu
    ├── CV-NamaKamu.pdf     ← File CV kamu
    ├── project-1.jpg       ← Screenshot proyek 1
    ├── project-2.jpg       ← Screenshot proyek 2
    └── project-3.jpg       ← Screenshot proyek 3
```

---

## 🚀 Cara Membuka di VSCode

1. **Buka folder** `portfolio-web` di VSCode
2. **Install ekstensi** "Live Server" (oleh Ritwick Dey)
   - Klik ikon Extensions (Ctrl+Shift+X)
   - Cari "Live Server" → Install
3. **Klik kanan** `index.html` → **"Open with Live Server"**
4. Browser otomatis terbuka di `http://127.0.0.1:5500`

---

## ✏️ Cara Kustomisasi

### Ganti Informasi Pribadi
Buka `index.html` dan cari komentar `<!-- Ganti ... -->` atau ganti teks:

| Yang Diganti | Lokasi |
|---|---|
| `[Nama Kamu]` | Hero section, nav, footer |
| `UI/UX Designer` | Hero role (diketik otomatis) |
| Deskripsi bio | Paragraf di `.hero__bio` |
| Email, LinkedIn, GitHub | Link di hero socials & contact |
| Nomor WhatsApp | `wa.me/628123456789` → ganti angkanya |

### Tambah Foto Profesional
1. Siapkan foto ukuran **400×500px** atau **3:4 ratio**
2. Simpan sebagai `assets/foto-saya.jpg`
3. Foto langsung muncul otomatis!

### Tambah CV PDF
1. Simpan file CV sebagai `assets/CV-NamaKamu.pdf`
2. Pastikan nama file sama dengan yang ada di HTML:
   ```html
   <a href="assets/CV-NamaKamu.pdf" download>
   ```

### Tambah Screenshot Proyek
1. Simpan gambar sebagai `assets/project-1.jpg`, `project-2.jpg`, dst.
2. Ukuran ideal: **800×500px** atau rasio **16:9**

### Ganti Role yang "Diketik"
Buka `script.js`, cari array `roles`:
```js
const roles = [
  'UI/UX Designer',
  'Frontend Developer',
  'Creative Thinker',
  // Tambah atau ubah sesuai keahlian kamu
];
```

### Ubah Warna Tema
Buka `style.css`, cari `:root` di bagian atas:
```css
:root {
  --gold:    #C9973B;   /* Ganti warna aksen utama */
  --dark-900: #0D0D0F;  /* Ganti warna background */
}
```

---

## 📧 Aktifkan Form Kontak

Saat ini form kontak dalam **mode demo** (tidak benar-benar mengirim email).

### Cara Aktifkan dengan Formspree (Gratis):
1. Daftar di [formspree.io](https://formspree.io)
2. Buat form baru → salin endpoint (contoh: `https://formspree.io/f/xpzgkrqw`)
3. Buka `script.js`, cari komentar `OPSI A: Formspree`
4. Hapus komentar `/* ... */` di blok Formspree
5. Ganti URL dengan endpoint kamu
6. Hapus blok `DEMO MODE` di bawahnya

---

## 📱 Fitur Website

- ✅ Responsive (HP, tablet, desktop)
- ✅ Navigasi sticky dengan highlight aktif
- ✅ Efek cursor glow
- ✅ Animasi reveal saat scroll
- ✅ Animasi skill bar
- ✅ Teks "diketik" otomatis (typed animation)
- ✅ Filter proyek by kategori
- ✅ Form kontak siap integrasi
- ✅ Mobile hamburger menu
- ✅ Placeholder jika foto belum ada
- ✅ Dark elegant theme + gold accent

---

## 🌐 Deploy ke Internet (Gratis)

### Vercel (Rekomendasi):
1. Push folder ke GitHub
2. Daftar [vercel.com](https://vercel.com) → Import repo
3. Deploy otomatis → dapat link `namakamu.vercel.app`

### Netlify:
1. Daftar [netlify.com](https://netlify.com)
2. Drag & drop folder `portfolio-web` ke dashboard
3. Selesai!

### GitHub Pages:
1. Push ke repo GitHub
2. Settings → Pages → Source: main branch
3. Akses di `username.github.io/nama-repo`

---

## 🐛 Troubleshooting

**Font tidak muncul?**
→ Pastikan terhubung internet saat pertama kali membuka (Google Fonts)

**Foto tidak muncul?**
→ Pastikan nama file sama persis (case-sensitive) dan berada di folder `assets/`

**Live Server tidak ditemukan?**
→ Install dari VSCode Extensions: cari "Live Server" by Ritwick Dey

---

Dibuat dengan ❤️ — Selamat berkreasi!
