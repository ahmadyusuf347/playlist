# Playlist Yusuf - Android

Aplikasi Android (Capacitor) yang membungkus index.html Anda.

## Langkah wajib
1. Salin seluruh folder `asset` Anda (mp3, cover_mp3, lirik, PlaylistCover.webp)
   ke dalam `www/asset/`.

## Cara A - Android Studio (di komputer)
1. Pasang Node.js dan Android Studio.
2. Di folder proyek: `npm install` lalu `npx cap sync android`
3. `npx cap open android` -> tunggu Gradle selesai
4. Build > Build Bundle(s) / APK(s) > Build APK(s)
   Hasil: android/app/build/outputs/apk/debug/app-debug.apk

## Cara B - Tanpa Android Studio (GitHub Actions)
1. Upload proyek ini ke repo GitHub (branch `main`).
2. Buka tab Actions > "Build APK" > tunggu selesai.
3. Unduh artifact `playlist-yusuf-apk`, pindahkan ke HP, lalu install.
   (Aktifkan "Install dari sumber tidak dikenal".)

## Setelah mengubah index.html / asset
Edit di `www/`, lalu jalankan `npx cap sync android` dan build ulang.
