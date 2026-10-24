KAMEN RIDER memory of heroez - PC
=================================
Port PC oleh Indra Sundanese.
KAMEN RIDER memory of heroez (PS4, CUSA17374) berjalan di Windows dengan Vulkan.
Perangkat lunak bebas, GNU GPL v2 atau lebih baru. Kredit: NOTICE.md. Tidak ada file game yang disertakan.

Cara bermain
  1. Taruh dump game milikmu sendiri (folder yang berisi eboot.bin, base game + update sudah digabung) di "game\",
     atau tekan "Browse..." di launcher lalu pilih folder game di lokasi lain.
  2. Buka "KMOH Launcher.exe", atur pengaturanmu, lalu tekan PLAY.
  Saat pertama kali dijalankan, game meng-compile shader dan akan patah-patah untuk sementara; shader disimpan di shader cache.

Persyaratan
  Windows 10 atau 11, 64-bit. CPU yang mendukung AVX2. Kartu grafis dengan Vulkan 1.3 dan driver terbaru.

Isi folder
  KMOH Launcher.exe   pengaturan dan tombol mulai
  bin\                runtime (kmoh-core.exe)
  game\               dump game milikmu (lokasi opsional)
  user\               save, shader cache (kecuali dipindah), log, kontrol, config.json

Opsi launcher
  Mode jendela        Windowed, Borderless fullscreen, Exclusive fullscreen
  Ukuran jendela      720p, 900p, 1080p, 1440p, 4K
  Resolusi render     720p atau 1080p (maksimum PS4)
  Upscaling           Mati atau AMD FSR 1, dengan opsi penajaman RCAS
  Frame rate          30 FPS (asli) atau 60 FPS (eksperimental)
  VSync, penghitung FPS, bahasa (Inggris, Jepang, Mandarin Tradisional, Korea), tombol konfirmasi
  Controls...         pemetaan keyboard (dua tombol per aksi) dan controller
  Shader cache        folder untuk shader yang sudah di-compile (bawaan user\cache); Clear untuk membangun ulang

Kontrol
  Controller (XInput, DualShock 4, DualSense) langsung bisa dipakai. Ubah tombol keyboard dan tombol controller
  lewat "Controls..." di launcher (disimpan di user\input_config\default.ini).

Masalah
  Lampirkan user\log\shad_log.txt di laporanmu.
