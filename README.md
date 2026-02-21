# URO Pretest Institut Teknologi Bandung - Sekuro 18
**Divisi:** Programming  
**Nama:** [Nama Lengkap Kamu]  
**NIM:** [NIM Kamu]  

Repositori ini berisi penyelesaian tugas seleksi (Pretest) untuk Divisi Programming Unit Robotika (URO) ITB. Seluruh pengerjaan dilakukan sesuai dengan petunjuk teknis yang diberikan, mencakup pengelolaan environment Linux, Git, dan pemrograman C++.

---

## 📁 Struktur Direktori

Repositori ini terdiri dari 4 folder utama:

1.  **Soal_1_[Nama]_[NIM]_Cakru18**: Administrasi sistem Linux (WSL/Dual Boot), CLI, dan manajemen file.
2.  **Soal_2_[Nama]_[NIM]_Cakru18**: Version Control System menggunakan Git (Branching & Merging).
3.  **Soal_3_[Nama]_[NIM]_Cakru18**: Simulasi Robot Pemadam Api menggunakan paradigma Object-Oriented Programming (OOP) C++.
4.  **Soal_4_[Nama]_[NIM]_Cakru18**: [Isi jika ada soal ke-4, atau hapus jika hanya sampai 3].

---

## 🛠️ Detail Pengerjaan

### Soal 1: Environment & CLI
Bagian ini membuktikan pemahaman mengenai arsitektur sistem operasi dan kemahiran menggunakan terminal Linux.
* **File Utama:** `Jawaban_1_a.pdf` (Analisis arsitektur OS).
* **Highlight:** Ekstraksi data sensor dari baris 1250-1260 menggunakan `head` dan `tail` piping.
* **Tools:** WSL 2 / Ubuntu, VS Code, Bash.

### Soal 2: Git & Version Control
Simulasi manajemen proyek menggunakan Git untuk menangani *conflict* antar branch.
* **Tautan Repositori Tugas 2:** [Masukkan Link Repo Sekuro18_Git_Nama Kamu Disini]
* **Log:** Histori penggabungan branch `v1` dan `v2` dapat dilihat pada file `riwayat_git.txt`.

### Soal 3: OOP C++ (Robot Pemadam Api)
Implementasi logika sensor-aktuator menggunakan Class dalam C++.
* **Logika Sensor:**
    * `> 20 cm`: Maju Mencari Api.
    * `5 - 20 cm`: Peringatan jarak dekat.
    * `<= 5 cm`: Aktivasi penyemprot.
* **Cara Menjalankan:**
    ```bash
    g++ robot_pemadam.cpp -o robot_pemadam
    ./robot_pemadam
    ```

---

## ⚠️ Engineering Integrity
> "Understanding the ’Why’ is your job. Finding the ’How’ is AI’s job."

Seluruh tugas ini dikerjakan dengan riset mandiri. Operasi file pada Soal 1 dilakukan murni melalui Terminal (CLI) tanpa manipulasi GUI untuk menjaga integritas teknis.

---
© 2024 [Nama Kamu] - Calon Kru URO 18
