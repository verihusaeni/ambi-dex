# 🛩️ AMBIDEX

**Pelatih Sinkronisasi Mouse & Keyboard berbasis Game — dalam satu file HTML**

*Satu Misi · Dua Tangan · Mouse + Keyboard*

![Version](https://img.shields.io/badge/version-1.3_FINAL-57f6c8?style=for-the-badge&labelColor=04090b)
![Dependencies](https://img.shields.io/badge/dependencies-0-ffb04d?style=for-the-badge&labelColor=04090b)
![Vanilla JS](https://img.shields.io/badge/vanilla-JS_100%25-57f6c8?style=for-the-badge&labelColor=04090b)
![License](https://img.shields.io/badge/license-All_Rights_Reserved-ff4d5e?style=for-the-badge&labelColor=04090b)

[▶️ **MAIN SEKARANG**](#-cara-memulai) · [🎮 Kontrol](#-kontrol) · [⚔️ Kesulitan](#-tingkat-kesulitan) · [🛠️ Teknologi](#️-teknologi)

</div>

---

## 📖 Tentang Aplikasi

**AMBIDEX** adalah aplikasi web untuk melatih kemampuan mengoperasikan **mouse dan keyboard secara simultan** — dua tangan bekerja pada dua alat kontrol berbeda dalam satu waktu.

Dalam game ini, Anda memiloti sebuah pesawat tempur (mouse) sementara tangan kiri bertugas mengetik kode musuh (keyboard). Keduanya terjadi **bersamaan**, memaksa otak Anda untuk membagi perhatian — persis seperti skill yang dibutuhkan dalam FPS, MOBA, atau pekerjaan multitasking di komputer.

> 💡 **Kenapa "AMBIDEX"?** Dari kata *ambidexterity* — kemampuan menggunakan dua tangan dengan sama terampil.

---

## ✨ Fitur

| Fitur | Deskripsi |
|---|---|
| 🖱️ **Latihan Mouse Komprehensif** | Gerak presisi, klik kiri (tembak), klik kanan (EMP), scroll (ganti senjata) |
| ⌨️ **Latihan Keyboard Terintegrasi** | Mengetik kode musuh & event **KEYSTORM** (mengetik secepat mungkin) |
| 🎯 **4 Tingkat Kesulitan** | Dari ramah anak-anak (6+) hingga brutal untuk dewasa |
| 🏆 **Sistem Gamifikasi** | Skor, combo multiplier ×8, gelombang musuh, power-up, rekor pribadi |
| 🎵 **Audio Prosedural Total** | Musik synthwave & seluruh SFX disintesis via Web Audio API — **nol file audio** |
| 📊 **Statistik Lengkap** | Akurasi tembak, kecepatan ketik (WPM), combo maksimum, gelombang tertinggi |
| 💾 **Tanpa Database** | Rekor & pengaturan tersimpan di `localStorage` — 100% privasi, 100% offline |
| 📱 **Responsif Penuh** | Menyesuaikan semua resolusi — dari jendela sempit hingga 4K, garansi musuh tidak pernah keluar layar |
| 🚫 **Tanpa Instalasi** | Satu file HTML. Buka di browser. Selesai. |

---

## 🎮 Kontrol

| Input | Aksi |
|---|---|
| **Gerak Mouse** | Pesawat mengikuti kursor — presisi adalah nyawa Anda |
| **Klik Kiri** | Tembak — *tahan* untuk tembakan otomatis |
| **Klik Kanan** | Gelombang **EMP** — pecah perisai & lumpuhkan musuh sekitar (ada cooldown) |
| **Scroll** | Ganti senjata: **LASER** → **SPREAD** (3 arah) → **ION** (pandu, damage 3) |
| **Keyboard (A–Z)** | Ketik kode musuh kristal untuk menghancurkannya |
| **ESC** | Jeda / lanjut |

### Mekanik Penting

- 🔮 **Musuh Breaker (kristal amber)** — tidak bisa ditembak. Ketik kata pada panel *UPLINK KODE* sampai selesai sebelum ia lolos. Bonus: EMP langsung terisi penuh.
- 🛡️ **Musuh berperisai (hexagon)** — hanya runtuh oleh EMP.
- ⚡ **KEYSTORM** — setiap ±40 detik, muncul huruf raksasa. Ketik secepat mungkin! Setiap 15 huruf benar = +1 hull.
- 🚨 **Garis Pertahanan** — musuh yang lolos ke bawah layar memotong 1 hull (dengan grace window 1 detik agar lolos serentak tidak menumpuk penalti).
- 📦 **Power-up** — 🔧 perbaiki hull · ⚡ overdrive (tembakan 1.8× lebih cepat) · 🔵 perisai 3 lapis.

---

## ⚔️ Tingkat Kesulitan

| Level | Target | Karakteristik |
|---|---|---|
| 🟢 **KADET** | Anak-anak · 6+ | Musuh lambat, kata 3–4 huruf, musuh tidak menembak, salah ketik diabaikan |
| 🔵 **PILOT** | Santai · Remaja | Ritme sedang, kata 3–5 huruf, ramah untuk pemula |
| 🟠 **VETERAN** | Dewasa · Standar | Musuh menembak, kata 4–7 huruf, salah ketik mengulang dari awal |
| 🔴 **ACE ELIT** | Dewasa · Brutal | Serangan rapat, kata 5–9 huruf, refleks & typing diuji tuntas |

---

## 🚀 Cara Memulai

### Prasyarat

Cukup sebuah browser modern (Chrome, Edge, Firefox, Safari — versi terakhir). **Tidak perlu server, tidak perlu instalasi.**

### Menjalankan

**Opsi 1 — Langsung:**

```bash
# unduh / clone repo, lalu buka filenya
git clone https://github.com/USERNAME/ambi-dex.git
cd ambidex
# buka index.html dengan double-click
```

**Opsi 2 — Lokal via server (opsional):**

```bash
# Python
python -m http.server 8080
# lalu buka http://localhost:8080/index.html

# atau Node.js
npx serve .
```

**Opsi 3 — Deploy online (gratis):**

- **GitHub Pages**: Settings → Pages → pilih branch `main` → selesai
- **Netlify / Vercel**: drag & drop folder berisi `index.html`

> ⚠️ **Catatan:** Aplikasi ini dirancang untuk **mouse + keyboard fisik**. Perangkat touch-only (HP/tablet) akan mendapat peringatan otomatis.

---

## 🛠️ Teknologi

| Teknologi | Peran |
|---|---|
| **HTML5 Canvas 2D** | Seluruh rendering game (60 FPS, devicePixelRatio-aware) |
| **Web Audio API** | Musik synthwave prosedural (sequencer 16th-note) + 15+ SFX tersintesis |
| **Vanilla JavaScript** | State machine, game loop `requestAnimationFrame`, fisika & kolisi |
| **CSS3** | HUD futuristik, media query responsif berlapis, efek scanline |
| **localStorage** | Penyimpanan rekor & pengaturan (dengan fallback aman try/catch) |
| **Google Fonts** | Orbitron · Rajdhani · Share Tech Mono (via CDN) |

### Arsitektur (ringkas)

```
ambidex.html
├── <style>          → UI futuristik + media query responsif
├── <div> HUD/Menu   → Title, Briefing, Settings, Pause, Game Over, Keystorm
└── <script>
    ├── AU / SFX / MUSIC → mesin audio prosedural
    ├── G / player / enemies → state game & entitas
    ├── update(dt)   → simulasi fisika, spawn, kolisi
    ├── enforceBounds() → jaminan musuh tak pernah di luar layar
    ├── drawWorld()  → seluruh render canvas
    └── loop()       → game loop utama (delta-time capped)
```

### Keputusan Teknis: Kenapa Tanpa Database?

Data yang dibutuhkan (rekor skor, volume, pilihan kesulitan) bersifat **lokal per pemain** — `localStorage` sudah lebih dari cukup, sehingga aplikasi tetap portabel, offline, dan tanpa setup. Jika kelak dibutuhkan leaderboard online, rekomendasi naik tingkat: **Supabase/Firebase** (tanpa backend sendiri). Backend + SQL baru perlu jika ada sistem akun multi-user.

---

## 🗺️ Roadmap

- [x] Sistem breach yang jujur & terlihat (garis pertahanan + grace window)
- [x] Presisi viewport — musuh dijamin tidak pernah di luar layar
- [x] Responsif semua ukuran & orientasi layar
- [ ] Mode latihan terisolasi (khusus mouse / khusus keyboard)
- [ ] Leaderboard online (Supabase)
- [ ] Mode 2 pemain bersaing (split keyboard)
- [ ] Ekspor statistik latihan (CSV/JSON)
- [ ] Dukungan layout keyboard non-QWERTY (Dvorak, dll)

---

## 🤝 Kontribusi

Pull request terbuka! Untuk perubahan besar, mohon buka *issue* terlebih dahulu untuk mendiskusikan apa yang ingin Anda ubah.

1. Fork repo ini
2. Buat branch fitur (`git checkout -b fitur/KerenBanget`)
3. Commit (`git commit -m 'Menambah fitur KerenBanget'`)
4. Push (`git push origin fitur/KerenBanget`)
5. Buka *Pull Request*

---

## 📜 Lisensi

Hak cipta dilindungi undang-undang. *(All rights reserved.)*

---

<div align="center">

**Made With** ❤️ **by** [**Veri Husaeni**](https://wa.me/6285311753792)

*All rights reserved.*

</div>
