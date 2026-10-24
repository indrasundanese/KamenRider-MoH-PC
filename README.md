<div align="center">

# KAMEN RIDER memory of heroez - PC

**Port PC oleh Indra Sundanese**

KAMEN RIDER memory of heroez (PS4, CUSA17374) berjalan di Windows dengan Vulkan.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-0078D6)
![Grafis](https://img.shields.io/badge/grafis-Vulkan%201.3-AC162C)
![Lisensi](https://img.shields.io/badge/lisensi-GPL--2.0--or--later-blue)
![Versi](https://img.shields.io/badge/versi-1.0-green)

</div>

---

> [!IMPORTANT]
> **Tidak ada file game yang disertakan.** Kamu membutuhkan dump game dari konsol milikmu sendiri.

## Tentang Proyek Ini

Runtime dan launcher PC untuk **KAMEN RIDER memory of heroez** (PlayStation 4, CUSA17374).

- Kode x86-64 milik game dijalankan langsung di prosesor PC.
- Library sistem PS4 diimplementasikan ulang di PC.
- Perintah GPU dan shader diterjemahkan ke Vulkan.

Perangkat lunak bebas (free software) di bawah lisensi GNU GPL v2 atau versi yang lebih baru. Kredit lengkap ada di [`NOTICE.md`](NOTICE.md).

## Persyaratan Sistem

| Komponen | Minimum |
|---|---|
| Sistem operasi | Windows 10 atau 11, 64-bit |
| Prosesor | CPU yang mendukung AVX2 |
| Kartu grafis | Mendukung Vulkan 1.3, dengan driver terbaru |

## Cara Bermain

1. Taruh dump game milikmu sendiri (folder yang berisi `eboot.bin`, base game + update sudah digabung) di folder `game\`,
   atau tekan **Browse...** di launcher lalu pilih folder game di lokasi lain.
2. Buka `KMOH Launcher.exe`, atur pengaturan yang kamu mau, lalu tekan **PLAY**.

> [!NOTE]
> Saat pertama kali dijalankan, game akan meng-compile shader dan akan patah-patah (stutter) untuk sementara.
> Shader yang sudah di-compile disimpan di shader cache, jadi permainan berikutnya akan lebih lancar.

## Isi Folder

```
KMOH Launcher.exe   pengaturan dan tombol mulai
bin\                runtime (kmoh-core.exe)
game\               dump game milikmu (lokasi opsional)
user\               save, shader cache (kecuali dipindah), log, kontrol, config.json
```

## Opsi Launcher

| Opsi | Pilihan |
|---|---|
| Mode jendela | Windowed, Borderless fullscreen, Exclusive fullscreen |
| Ukuran jendela | 720p, 900p, 1080p, 1440p, 4K |
| Resolusi render | 720p atau 1080p (maksimum PS4) |
| Upscaling | Mati atau AMD FSR 1, dengan opsi penajaman RCAS |
| Frame rate | 30 FPS (asli) atau 60 FPS (eksperimental) |
| Lainnya | VSync, penghitung FPS, bahasa (Inggris, Jepang, Mandarin Tradisional, Korea), tombol konfirmasi |
| Controls... | Pemetaan keyboard (dua tombol per aksi) dan controller |
| Shader cache | Folder untuk shader yang sudah di-compile (bawaan `user\cache`); tombol **Clear** untuk membangun ulang |

Semua pengaturan disimpan di folder `user\` (portable).

## Kontrol

Controller (XInput, DualShock 4, DualSense) langsung bisa dipakai.
Ubah tombol keyboard dan tombol controller lewat **Controls...** di launcher
(disimpan di `user\input_config\default.ini`).

## Dibangun di Atas

| Karya | Pembuat | Lisensi |
|---|---|---|
| **shadPS4**: seluruh runtime - loader, library sistem PS4, GPU command processor, shader recompiler (GCN ke SPIR-V) dan renderer Vulkan, termasuk FSR 1 / RCAS | Tim dan kontributor shadPS4 | GPL-2.0-or-later |
| SDL3, Vulkan headers dan loader, Vulkan Memory Allocator, glslang, sirit, Dear ImGui, FFmpeg, OpenAL Soft, LibAtrac9, fdk-aac, fmt, spdlog, nlohmann json, toml11, zlib-ng, zstd, xbyak, Zydis, magic_enum, robin-map, half, xxHash, Boost, LibreSSL, dan library lain di folder `externals` shadPS4 | Para pembuatnya masing-masing | Lisensi masing-masing |
| AMD FidelityFX Super Resolution 1 (FSR 1) | AMD | MIT |

Pendekatan ini terinspirasi dari port PC native Bloodborne (bloodborne_pc), God of War III (SpartanPort),
yang juga dibangun di atas shadPS4.

## Versi

```
KAMEN RIDER memory of heroez - PC 1.0 (Vulkan) - Port PC oleh Indra Sundanese
```

## Melaporkan Masalah

Lampirkan file `user\log\shad_log.txt` di laporanmu.

## Lisensi

GNU General Public License, versi 2 atau (sesuai pilihanmu) versi yang lebih baru. Lihat [`LICENSE`](LICENSE).
Siapa pun yang menerima build dari proyek ini berhak mendapatkan source code-nya, termasuk perubahan-perubahannya.

---

<sub>"KAMEN RIDER" dan "memory of heroez" adalah merek dagang milik pemiliknya masing-masing (Ishimori Production, Toei,
Bandai Namco Entertainment). Proyek ini tidak berafiliasi dengan mereka maupun dengan Sony Interactive Entertainment.</sub>
