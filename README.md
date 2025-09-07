# 🚀 EFI Hackintosh Lenovo ThinkPad T440P (Haswell)

EFI ini dibuat khusus untuk laptop **Lenovo ThinkPad T440P** dengan prosesor **Intel Haswell (4th Gen)**. Mendukung macOS **Catalina**, **Big Sur**, dan **Ventura**.

---

## ✅ Sistem Operasi yang Didukung

| Versi macOS     | Status          | Keterangan                                                                  |
|-----------------|-----------------|----------------------------------------------------------------------------|
| Catalina (10.15)| ✅ Native       | Berjalan langsung tanpa patch tambahan.                                    |
| Big Sur (11)    | ✅ Native       | Berjalan langsung, tanpa perlu OpenCore Legacy Patcher.                    |
| Ventura (13)    | ⚠️ Patch Diperlukan | Harus menggunakan **OpenCore Legacy Patcher** agar iGPU tidak terdeteksi 5MB.|

---

## ⚠️ Penting untuk Ventura

Untuk macOS Ventura, wajib melakukan patch dengan **OpenCore Legacy Patcher (OCLP)** setelah instalasi.  
Jika tidak, iGPU akan terdeteksi hanya 5MB yang menyebabkan grafis bermasalah.

**Langkah singkat:**

1. Install Ventura menggunakan EFI ini.
2. Setelah boot ke macOS, download dan jalankan **OCLP**.
3. Lakukan patch post-install untuk seri Haswell.
4. Restart.

---

---

## 💻 Spesifikasi yang Didukung

- Laptop: Lenovo ThinkPad T440P
- CPU: Intel Haswell (Core i5/i7 4th Gen)
- iGPU: Intel HD Graphics 4600
- Audio: Realtek ALC292
- Wi-Fi: Ganti ke kartu kompatibel (misal DW1560 atau BCM94360)

---

## ⚙️ Fitur Yang Berfungsi

- Audio  
- Wi-Fi (dengan kartu kompatibel)  
- iGPU Acceleration (setelah patch OCLP untuk Ventura)  
- Battery status  
- Trackpad  
- Brightness  
- Sleep/Wake  

---

## ❗ Catatan

- Jangan update OpenCore tanpa menyesuaikan konfigurasi.  
- Folder Ventura-Build berisi varian untuk seri tertentu, cek dokumentasi dalam folder.  
- Gunakan ProperTree untuk modifikasi `config.plist` jika perlu.  
- Selalu backup EFI sebelum melakukan perubahan.

---

## 🛠️ Tools Rekomendasi

- [OpenCore Legacy Patcher (OCLP)](https://dortania.github.io/OpenCore-Legacy-Patcher/)  
- [ProperTree](https://github.com/corpnewt/ProperTree)  
- [Hackintool](https://github.com/headkaze/Hackintool)  

---

## 🙏 Terima kasih kepada

- Tim OpenCore  
- Komunitas Hackintosh Indonesia  
- Dokumentasi Dortania  

---

*EFI ini hanya untuk keperluan edukasi dan eksperimen, bukan untuk dijual.*
