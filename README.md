# 🌍 Peta Posisi Matahari & Bulan Real-time

Aplikasi web interaktif satu halaman (single-file HTML) yang menampilkan **posisi Matahari dan Bulan secara real-time** di atas peta **OpenStreetMap**, lengkap dengan:

- ☀️ **Subsolar Point** — titik di Bumi yang saat ini tepat berada di bawah Matahari (siang hari)
- 🌙 **Sublunar Point** — titik di Bumi yang saat ini tepat berada di bawah Bulan
- 🌓 **Area malam (night side)** yang diarsir gelap dan **garis terminator** yang memisahkan siang dan malam
- 🏳️ **Nama negara** dan bendera di titik tersebut
- 🕒 **Zona waktu** dan **waktu lokal** di titik tersebut

---

## ✨ Fitur

| Fitur | Keterangan |
|---|---|
| **Peta interaktif** | OpenStreetMap via Leaflet — bisa di-zoom, digeser, dan di-klik |
| **Subsolar & Sublunar Point** | Dihitung secara akurat memakai library [Astronomy Engine](https://github.com/cosinekitty/astronomy) |
| **Area malam** | Poligon semi-transparan menutupi belahan Bumi yang sedang gelap |
| **Garis terminator** | Garis kuning yang menandai batas siang/malam |
| **Nama negara** | Otomatis lewat reverse geocoding (BigDataCloud API, gratis tanpa API key) |
| **Bendera negara** | Emoji bendera dikonversi dari kode ISO negara |
| **Zona waktu** | IANA timezone (mis. `Asia/Jakarta`) beserta singkatan (`WIB`) via Open-Meteo API |
| **Waktu lokal** | Jam di lokasi tersebut, dihitung dengan `Intl.DateTimeFormat` |
| **Auto-refresh** | Posisi diperbarui setiap **30 detik**; info negara & zona waktu di-cache 10 menit |
| **Fallback** | Jika suatu titik berada di laut, ditampilkan `🌊 Laut / Samudra` |
| **Timeout API** | Setiap `fetch` punya timeout 10 detik supaya UI tidak macet |
| **Diagnostik** | Panel kecil menampilkan status library & metode perhitungan yang berhasil |

---

## 📁 Struktur Repositori
