# ERGO-WEAR — GEMASTIK 2026

Versi ini mempertahankan **monitoring original** sebagai inti aplikasi, lalu menempatkan penjelasan proyek pada menu **Overview**.

## Struktur

- `src/App.jsx` — aplikasi React utama; logic monitoring original tetap dipertahankan.
- `src/main.jsx` — entry React.
- `src/styles.css` — base styling.
- `public/assets/ergowear-demo.mp4` — video demo alat.
- `package.json` — konfigurasi Vite/React.

## Perubahan UI terbaru

- Menu **Proyek** dihapus.
- Menu **Overview** menjadi halaman awal.
- Overview memuat: apa itu ERGO-WEAR, masalah, dasar/urgensi, solusi, closed-loop, perbandingan produk, dan video demo.
- Bagian masalah/dasar/solusi bersifat interaktif (tab/card).
- Alur MPU6050 → ESP32-S3 → Haptic → IoT dapat dibuka per tahap.
- Tombol Overview mengarah langsung ke monitoring original.
- Menu Dasbor, Riwayat, Pekerja, Alat, dan Pengaturan tetap dipertahankan.

## Jalankan lokal

```bash
npm install
npm run dev
```

## Build untuk hosting

```bash
npm run build
```

Output produksi berada di folder `dist/` dan dapat dideploy ke Vercel/Netlify/static hosting.

## Catatan

Video harus tetap berada di `public/assets/ergowear-demo.mp4` agar player di Overview dapat memuatnya.
