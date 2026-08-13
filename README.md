# ERGO-WEAR GEMASTIK FINAL

Versi ini mempertahankan **logic dan monitoring dari `ergowear-dashboard.jsx` original sebagai fondasi utama**, lalu menambahkan Product Overview cinematic, closed-loop system visualization, dan video demo.

## Fitur original yang dipertahankan
- Live posture monitoring dan simulasi sudut
- Zona Aman / Waspada / Bahaya
- Durasi deviasi dan threshold
- Risk score
- Event timeline
- Riwayat dan tren
- Perbandingan pekerja
- Spesifikasi alat
- Ringkasan proyek
- Pengaturan threshold
- Export CSV / laporan yang sudah ada di source original
- Device illustration

## Tambahan visual
- Product Overview cinematic
- Closed-loop BNO055 → ESP32-S3 → Haptic → IoT
- Video demo alat
- CTA menuju dashboard asli

## Menjalankan
```bash
npm install
npm run dev
```
Buka URL localhost yang diberikan Vite.

## Build hosting
```bash
npm run build
```
Folder hasil build: `dist/`

## Catatan
`public/assets/ergowear-demo.mp4` adalah video demo. Jangan mengubah path tanpa memperbarui source video di `OverviewTab`.
Tailwind dimuat melalui CDN di `index.html`; saat deploy, koneksi internet diperlukan agar utility classes tampil seperti desain.
