# Praktik Dasar OpenCV Part 2: Image Crop, Resize & Blending

Repository ini berisi hasil praktik mandiri Kelompok 1 untuk mata kuliah **Praktik Machine Learning / Pengolahan Citra Digital**. Proyek ini mencakup teknik manipulasi citra tingkat lanjut menggunakan library OpenCV, termasuk penggunaan Mouse Event untuk interaksi langsung dengan gambar.

## Anggota Kelompok 1
**Informatika – Universitas Teknologi Sumbawa**
* **Sherly Novia Indriani** - 231001057
* **Dinda Oktavia Pratiwi** - 231001026
* **Ahsanul Ikram** - 231001077
* **Wanda Setya Budi** - 231001008

**Dosen Pengampu:** Herfandi, Ph.D.

---

## Alat dan Library
Untuk menjalankan proyek ini, kami menggunakan:
* **Bahasa:** Python 3.x
* **Library Utama:**
    * OpenCV (opencv-python)
    * NumPy
* **Editor:** Visual Studio Code / Jupyter Notebook

---

## Langkah-Langkah Praktik
Dokumentasi ini menjelaskan proses yang dilakukan di dalam file kodingan:

### 1. Image Cropping (Pemotongan Citra)
Melakukan pemotongan area tertentu pada gambar menggunakan teknik *Numpy Slicing*. Praktik ini mencakup:
* Crop koordinat tetap.
* Crop dengan margin (piksel & persentase).
* **Interactive Cropping:** Menggunakan Mouse Event (`cv2.setMouseCallback`) untuk memilih area potong secara dinamis.
* **Task:** Implementasi fitur simpan gambar otomatis ke folder lokal saat klik kanan mouse ditekan.

### 2. Image Resizing (Pengubahan Ukuran)
Mengubah dimensi gambar melalui beberapa pendekatan:
* Ukuran tetap (fixed size) dan rasio skala.
* Eksperimen berbagai metode **Interpolasi** seperti `INTER_NEAREST`, `INTER_AREA`, dan `INTER_CUBIC` untuk menjaga kualitas gambar saat diperbesar atau diperkecil.
* **Interactive Resize:** Mengubah ukuran gambar secara real-time mengikuti gerakan mouse.

### 3. Image Blending & Overlay
Teknik mencampur dua gambar dengan formula matematis menggunakan `cv2.addWeighted()`:
* Blending dua gambar dengan ukuran sama maupun berbeda.
* Membuat bingkai (*Frame*) agar gambar proporsional (Fit Window).
* **Transparent Overlay:** Memberikan lapisan warna transparan pada area tertentu.

### 4. Homework: Blue Overlay Interaktif
Implementasi tugas akhir berupa pembuatan filter biru transparan yang dapat digambar langsung menggunakan mouse pada gambar target secara real-time.

---

## Video Presentasi
Penjelasan detail mengenai proses koding, analisis kode, dan hasil praktik dapat dilihat pada video YouTube kami berikut:
👉 [https://youtu.be/tILiQoA3hy8?si=V0gVP8lm4qdJ-bfc]

---

## Cara Menjalankan
1. Clone repository ini:
    ```bash
    git clone https://github.com/Sherlynoviaa/Praktik-OpenCV-Part2-Kelompok1.git
    ```
2. Pastikan library sudah terinstal:
    ```bash
    pip install opencv-python numpy
    ```
3. Buka file `opencv_part2.ipynb` di VS Code atau Jupyter Notebook.
4. Pastikan file gambar (`lena.jpg`, `apple.jpg`, dll) berada di folder yang sama dengan file kodingan.
