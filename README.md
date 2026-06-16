# 🤖 WhatsApp Bot Auto-Reject Call

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg?style=flat-square)
![NodeJS](https://img.shields.io/badge/node.js->=20.0.0-brightgreen.svg?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Ubuntu%20%7C%20Debian-lightgrey.svg?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green.svg?style=flat-square)

Bot WhatsApp ringan dan responsif yang dirancang khusus untuk menolak panggilan masuk (Telepon & Video Call) secara otomatis. Sangat cocok untuk toko online, admin PPOB, atau nomor bisnis agar operasional chat tidak terganggu oleh panggilan yang tidak diinginkan.

---

## ✨ Fitur Unggulan

- 📞 **Auto-Reject Panggilan:** Langsung menolak/mematikan telepon dan video call yang masuk dalam hitungan detik.
- 💬 **Auto-Reply Cerdas:** Mengirimkan pesan balasan otomatis kepada penelepon untuk mengarahkan mereka agar mengirim pesan via chat.
- ⚡ **Ringan & Cepat:** Menggunakan *library* Baileys yang sangat ringan dan hemat memori (RAM).
- 🔄 **Aktif 24/7:** Terintegrasi dengan **PM2**, bot akan terus berjalan di *background* VPS Anda tanpa henti (otomatis menyala ulang jika VPS direstart).
- 🔒 **Login Tanpa Ribet:** Login menggunakan **Pairing Code** langsung di terminal, tidak perlu pusing *scan* QR Code.

---

## 🚀 Instalasi VPS Satu Kali Klik (One-Click Deploy)

Anda tidak perlu *setting* manual satu per satu! Cukup siapkan VPS dengan OS **Ubuntu** atau **Debian**, lalu *copy* dan *paste* perintah di bawah ini ke terminal SSH VPS Anda:

```bash
apt-get update && apt-get install -y wget && wget -qO instal.sh [https://raw.githubusercontent.com/fikystorez/botwa-autoRejectCall/main/instal.sh](https://raw.githubusercontent.com/fikystorez/botwa-autoRejectCall/main/instal.sh) && chmod +x instal.sh && ./instal.sh
```

> **Catatan:** Pastikan Anda mengeksekusi perintah di atas menggunakan *user* `root` atau memiliki akses `sudo`.

---

## ⚙️ Panduan Penggunaan Setelah Instalasi

1. Setelah Anda menjalankan perintah instalasi di atas, *script* akan mengunduh dan menyiapkan semuanya secara otomatis.
2. Saat muncul *prompt*, masukkan nomor WhatsApp yang akan dijadikan bot (Format: `628123456789`).
3. Terminal akan memunculkan **KODE PAIRING**.
4. Buka aplikasi WhatsApp di HP Anda ➔ Pilih **Perangkat Tertaut** ➔ **Tautkan Perangkat** ➔ Pilih opsi **Tautkan dengan nomor telepon saja** (ada di bagian bawah layar).
5. Masukkan **KODE PAIRING** yang muncul di terminal VPS.
6. **Selesai!** Bot akan otomatis berjalan di *background* dengan PM2. Terminal VPS sudah bisa Anda tutup dengan aman.

---

## 🛠️ Perintah Pengelolaan (PM2)

Untuk mengecek atau mengelola bot di kemudian hari, gunakan perintah berikut di terminal VPS Anda:

| Perintah | Fungsi |
| --- | --- |
| `pm2 status` | Melihat status bot (aktif/mati) |
| `pm2 logs bot-wa` | Melihat log aktivitas atau *error* dari bot |
| `pm2 restart bot-wa`| Memulai ulang (restart) bot |
| `pm2 stop bot-wa` | Mematikan bot sementara |

---

<p align="center">
  Dibuat dengan ❤️ oleh <a href="https://github.com/fikystorez">fikystorez</a>
</p>
