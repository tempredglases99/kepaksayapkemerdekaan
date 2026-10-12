# Prompt Aset Gambar AI — Terbang Elang

Gambar yang Bapak buat dengan AI cukup **disimpan dengan nama file persis seperti di tabel**, di folder yang ditunjukkan. Media otomatis memakainya. Kalau file belum ada, media tetap jalan dengan peraga garis bawaan.

## Aturan umum (berlaku untuk semua gambar)

- **Gaya:** samakan dengan lembar karakter Elang Jawa: *stylized 3D render, soft studio lighting, Pixar-like, clean*.
- **Latar:** polos terang `#E6F3EE` (hijau mint sangat muda), tanpa teks, tanpa bayangan lantai yang tebal.
- **Ukuran:** 1000 × 1250 px (rasio 4:5), format PNG.
- **Tokoh:** satu anak yang sama di semua gambar. Buat dulu **lembar karakter anak** (prompt A), lalu pakai gambar itu sebagai referensi untuk semua prompt B agar wajah, seragam, dan proporsinya konsisten.
- **Sudut pandang demonstrasi: DARI BELAKANG.** Media menulis "kiri gambar = kiri siswa", jadi anak harus membelakangi kamera.

---

## A. Lembar karakter anak (buat sekali, jadi referensi)

> Character reference sheet of a 10-year-old Indonesian elementary school student, short black hair, wearing a red-and-white sports t-shirt, navy blue track pants, white sneakers, friendly and energetic. Show front view, back view, side view, full body, neutral standing pose with arms relaxed. Stylized 3D render, soft studio lighting, Pixar-like, clean, plain light mint background #E6F3EE, no text.

Simpan sebagai: `asset/img/demo/_referensi_anak.png` (tidak dipakai media, hanya arsip).

---

## B. Demonstrasi bertahap → folder `asset/img/demo/`

Awali setiap prompt dengan kalimat ini, lalu tambahkan kalimat khusus dari tabel:

> **Same child as the reference image, seen from directly behind (back view), full body, standing on the spot, feet shoulder-width apart. Stylized 3D render, soft studio lighting, Pixar-like, clean, plain light mint background #E6F3EE, no text.**

| Nama file | Kalimat khusus (tambahkan setelah kalimat awal) |
|---|---|
| `lompat_1.png` | Standing tall, feet shoulder-width apart, arms relaxed at the sides. |
| `lompat_2.png` | Preparing to jump: knees slightly bent, arms swung down and slightly back, feet flat on the floor. |
| `lompat_3.png` | Jumping straight up with both feet off the ground, arms swung up overhead, small gap between shoes and floor, soft shadow on the floor below. |
| `lompat_4.png` | Landing softly on both feet, knees bent to absorb the landing, arms forward for balance. |
| `kepak_1.png` | Both arms stretched straight out to the sides at shoulder height like eagle wings. |
| `kepak_2.png` | Both arms swung slightly upward above shoulder height at the same time, like a wing upstroke, slight motion blur on hands. |
| `kepak_3.png` | Both arms swung slightly downward below shoulder height at the same time, like a wing downstroke, slight motion blur on hands. |
| `liuk_1.png` | Both arms stretched out to the sides, body upright. |
| `liuk_2.png` | Bending the upper body sideways to HER/HIS LEFT from the waist, left shoulder lower than right, arms still stretched out, feet stay planted. |
| `liuk_3.png` | Returning to upright position, arms stretched out to the sides. |
| `liuk_4.png` | Bending the upper body sideways to HER/HIS RIGHT from the waist, right shoulder lower than left, arms still stretched out, feet stay planted. |
| `raih_1.png` | Standing tall, arms relaxed at the sides. |
| `raih_2.png` | Raising both arms straight up overhead, palms facing each other, arms beside the ears. |
| `raih_3.png` | Holding both arms straight up overhead, reaching as high as possible, standing on the whole foot, calm. |
| `tekuk_1.png` | Standing tall, arms stretched out to the sides. |
| `tekuk_2.png` | Half squat: both knees bent, back straight and upright, heels on the floor, arms stretched out to the sides for balance. |
| `tekuk_3.png` | Rising back up to standing, knees almost straight, arms stretched out to the sides. |

> Catatan: karena tampak belakang, "kiri anak" = kiri gambar. Periksa `liuk_2` (miring ke **kiri gambar**) dan `liuk_4` (miring ke **kanan gambar**) sebelum disimpan.

---

## C. Ilustrasi materi → folder `asset/img/materi/` (opsional)

Ukuran 1600 × 900 px (16:9), PNG.

| Nama file | Prompt |
|---|---|
| `lokomotor.png` | Same child as the reference image running and jumping across a schoolyard field, showing movement from one place to another, dotted motion path on the ground, stylized 3D render, Pixar-like, bright daylight, no text. |
| `nonlokomotor.png` | Same child as the reference image standing in one spot inside a painted circle on the schoolyard, bending the body sideways with arms stretched out, feet not moving, small curved motion arrows around the arms and waist, stylized 3D render, Pixar-like, bright daylight, no text. |

---

## Gambar yang sudah ada (jangan ditimpa)

- `latar_pulau.jpg`: latar pulau 16:9, hasil render Blender.
- `elang/*.png`: 17 pose dan ekspresi Elang Jawa dari lembar karakter Bapak.
