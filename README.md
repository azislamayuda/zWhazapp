# Whazapp

Whazapp adalah aplikasi desktop untuk WhatsApp Web di Linux dan Windows. Satu jendela, sampai tiga akun WhatsApp, dan notifikasi desktop.

Repo ini hanya berisi file rilis. Unduh versi terbaru dari halaman [Releases](https://github.com/azislamayuda/zWhazapp/releases/latest).

## Unduh

| Sistem | File |
|---|---|
| Linux (x86_64) | `Whazapp_0.1.5_amd64.AppImage` |
| Windows 10/11 (x64) | `Whazapp_0.1.5_x64-setup.exe` |
| Checksum | `SHA256SUMS` |

**Linux:** jadikan AppImage bisa dijalankan, lalu buka.

```sh
chmod +x Whazapp_0.1.5_amd64.AppImage
./Whazapp_0.1.5_amd64.AppImage
```

**Windows:** jalankan `Whazapp_0.1.5_x64-setup.exe` dan ikuti installer. Installer belum ditandatangani, jadi Windows SmartScreen bisa menampilkan peringatan. Pilih "More info", lalu "Run anyway".

Setelah aplikasi terbuka, pindai kode QR dengan WhatsApp di ponsel, sama seperti WhatsApp Web.

## Verifikasi file

Simpan `SHA256SUMS` di folder yang sama dengan file yang diunduh, lalu jalankan:

```sh
sha256sum -c SHA256SUMS
```

Setiap file yang cocok ditandai `OK`. Kalau Anda hanya mengunduh satu installer, tambahkan `--ignore-missing`. Jangan pakai file yang hasilnya `FAILED`; unduh ulang.

## Yang baru di 0.1.5

- Tombol blur melayang di halaman chat untuk menyamarkan isi pesan, daftar chat, gambar dan media, atau layar penuh. Pilihan disimpan per akun (Linux).
- Cek update memverifikasi installer dengan `SHA256SUMS` lalu menyimpannya ke folder Unduhan. Aplikasi juga mengecek sendiri paling sering sekali per 24 jam.
- Tombol aktif di toolbar lebih jelas dan tidak lagi bergaris tepi. Di Windows, tombol update pindah ke footer.
- Perbaikan stabilitas.

Daftar lengkap ada di catatan setiap rilis.

## Catatan

Whazapp adalah aplikasi komunitas dan tidak berafiliasi dengan WhatsApp atau Meta. WhatsApp adalah merek dagang milik pemiliknya.

## Lisensi

[MIT](LICENSE)
