# Affiliate AI Studio - GitHub Cloud Build

## Membuat APK tanpa Android Studio
1. Buat repository GitHub bernama `affiliate-ai-studio-android`.
2. Ekstrak ZIP ini di komputer.
3. Di halaman repository GitHub, pilih **Add file > Upload files**.
4. Buka folder hasil ekstrak, pilih semua ISI folder (termasuk folder `.github`), lalu seret ke area upload GitHub. Jangan mengunggah folder ZIP sebagai satu file.
5. Tunggu unggahan selesai, isi pesan commit misalnya `Add Android app source`, lalu klik **Commit changes**.
6. Buka tab **Actions** pada repository. Workflow **Build Affiliate AI Studio APK** akan berjalan otomatis. Jika tidak, pilih workflow itu lalu klik **Run workflow**.
7. Setelah status hijau/Success, buka run yang terbaru, cari **Artifacts**, lalu unduh `Affiliate-AI-Studio-debug-APK`.
8. Ekstrak ZIP artifact tersebut. File di dalamnya bernama `app-debug.apk`.
9. Kirim APK ke Xiaomi 14T dan instal. Android mungkin meminta izin memasang aplikasi dari sumber tersebut.

## Isi dan batasan versi 1.0
- Aplikasi Android WebView, minSdk 23, targetSdk 35, compileSdk 35.
- Dashboard dark mode, preview video lokal, rentang preview, generator naskah template offline, simpan draft lokal.
- Ini bukan editor non-linear penuh. Belum ada pemotongan/encoding MP4, subtitle speech-to-text, AI cloud backend, atau jaminan bebas bug. APK harus diuji di perangkat sebelum dipakai rutin.
- Jangan memasukkan API key rahasia ke file HTML atau repository publik.
