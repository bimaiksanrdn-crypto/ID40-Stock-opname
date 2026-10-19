ID40 CYBERPUNK STOCK OPNAME — PWA

ISI FOLDER
- index.html: web app
- manifest.json: nama/ikon aplikasi
- service-worker.js: cache shell aplikasi
- icons/: ikon 192 dan 512 px

CARA PAKAI
1. Upload SEMUA isi folder ini ke hosting statis yang menyediakan HTTPS. Jangan upload hanya index.html.
2. Buka URL hosting di Chrome Android.
3. Pilih menu ⋮ > Install app / Tambahkan ke layar utama.
4. Login dengan akun Supabase yang sudah ada.

PENTING
- PWA perlu URL HTTPS agar bisa di-install dengan benar; membuka file lokal (file://) saja tidak cukup.
- Aplikasi ini tetap memakai Supabase online dan modul CDN, jadi fitur database/login memerlukan internet. Service worker ini cache kerangka aplikasi saja, bukan data opname offline.
- Jangan publikasikan anon/service key yang memiliki hak istimewa. Pastikan RLS Supabase aktif dan policy sudah sesuai.
