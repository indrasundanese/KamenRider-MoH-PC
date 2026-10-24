# KAMEN RIDER memory of heroez - PC

Port PC oleh **Indra Sundanese**.

Runtime dan launcher PC untuk **KAMEN RIDER memory of heroez** (PlayStation 4, CUSA17374).
Kode x86-64 milik game dijalankan langsung di prosesor PC; library sistem PS4 diimplementasikan
di PC; perintah GPU dan shader diterjemahkan ke Vulkan.

Tidak ada file game yang disertakan. Kamu membutuhkan dump game dari konsol milikmu sendiri.

## Proyek ini dibangun di atas

| Karya | Pembuat | Lisensi |
|---|---|---|
| **shadPS4**: seluruh runtime - loader, library sistem PS4, GPU command processor, shader recompiler (GCN ke SPIR-V) dan renderer Vulkan, termasuk FSR 1 / RCAS | Tim dan kontributor shadPS4 | GPL-2.0-or-later |
| SDL3, Vulkan headers dan loader, Vulkan Memory Allocator, glslang, sirit, Dear ImGui, FFmpeg, OpenAL Soft, LibAtrac9, fdk-aac, fmt, spdlog, nlohmann json, toml11, zlib-ng, zstd, xbyak, Zydis, magic_enum, robin-map, half, xxHash, Boost, LibreSSL, dan library lain di folder `externals` shadPS4 | Para pembuatnya masing-masing | Lisensi masing-masing |
| AMD FidelityFX Super Resolution 1 (FSR 1) | AMD | MIT |

Pendekatan ini terinspirasi dari port PC native Bloodborne (bloodborne_pc), God of War III (SpartanPort), yang juga dibangun di atas shadPS4.

## Lisensi

GNU General Public License, versi 2 atau (sesuai pilihanmu) versi yang lebih baru. Lihat `LICENSE`.
Siapa pun yang menerima build dari proyek ini berhak mendapatkan source code-nya, termasuk perubahan-perubahannya.

"KAMEN RIDER" dan "memory of heroez" adalah merek dagang milik pemiliknya masing-masing (Ishimori Production, Toei,
Bandai Namco Entertainment). Proyek ini tidak berafiliasi dengan mereka maupun dengan Sony Interactive Entertainment.
