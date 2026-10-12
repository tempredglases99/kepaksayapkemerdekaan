# Folder pipeline: mesin yang menjalankan Terbang Elang tanpa internet

Semua yang biasanya diunduh dari internet saat bermain sudah disimpan di sini. Dibungkus sebagai file `.js` supaya Chrome mau membacanya saat `index.html` dibuka langsung (klik dua kali), tanpa server.

| File | Isi | Dipakai kapan |
|---|---|---|
| `engine.js` | Three.js 0.160 (grafis 3D) + GLTFLoader + MediaPipe Tasks Vision 0.10.14 | Selalu |
| `fonts.css` | Huruf Baloo 2 dan Lexend | Selalu |
| `vision_wasm_internal.js` | Pemuat mesin MediaPipe | Saat "Mulai dengan Kamera" |
| `vision_wasm_data.js` | Mesin WebAssembly MediaPipe (dalam bentuk teks) | Saat "Mulai dengan Kamera" |
| `pose_model_data.js` | Model pose tubuh *pose_landmarker_lite* (dalam bentuk teks) | Saat "Mulai dengan Kamera" |
| `pose_landmarker_lite.task` | Model pose asli dari Google (cadangan, tidak dibaca langsung) | Arsip |

Alur pipeline saat kamera dinyalakan:

1. Kamera laptop (`getUserMedia`)
2. MediaPipe Pose: 33 titik tubuh per bingkai
3. Klasifikasi gerak (di `index.html`): kepak, meliuk, meraih, menekuk
4. Mesin game 3D: elang bergerak
5. Rekap data gerak di layar hasil

**Jangan memindahkan atau mengganti nama file di folder ini.** Jika media dipindahkan ke laptop lain, salin seluruh folder `MPI_KEPAK SAYAP_NONLOKOMOTOR` (berisi `index.html` dan folder `asset`).
