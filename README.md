URO PRETEST INSTITUT TEKNOLOGI BANDUNG
PROGRAMMING SEKURO 18
Selamat Datang CaKRU-18 !!
URO Test Divisi Programming merupakan bagian dari proses seleksi URO pada divisi programming dimana CaKru-18 diwajibkan untuk memenuhi beberapa ketentuan berikut:
PETUNJUK PENGERJAAN
Peserta wajib mengerjakan semua soal, tidak menjawab sekurang-kurangnya 1 soal maka diberikan nilai 0.
Peserta mengerjakan URO Test dengan serius dimana penilaian ini akan mempengaruhi kelulusan hingga tahap penentuan tim.
Peserta mengerjakan URO Test pada waktu yang telah ditentukan, yaitu sejak Oprec dibuka hingga Oprec ditutup + 2 hari. Peserta yang mengumpulkan melewati tenggat waktu maka dianggap tidak mengumpulkan.
Peserta disarankan untuk memaksimalkan kemampuan riset dan mencari tahu sumber informasi terkait permasalahan yang ditemui pada URO Test di kanal youtube ataupun sumber lainnya.
Peserta dilarang keras untuk menggunakan AI untuk menjawab soal-soal yang melibatkan kemampuan riset dan teknis.
Semua Pengumpulan dilakukan dengan sebuah link Github dimana mencakup 4 folder utama pada sebuah repository Private:
Soal_1_(Nama)_(NIM)_Cakru18
Soal_2_(Nama)_(NIM)_Cakru18
Soal_3_(Nama)_(NIM)_Cakru18
Soal_4_(Nama)_(NIM)_Cakru18
Peserta mengumpulkan link github URO Test tersebut pada form yang disediakan.
Pastikan semua file/link yang dikumpul, aksesnya dapat dibuka dengan baik.
 
 
 
 
WARNING: ENGINEERING INTEGRITY CHECK
"Understanding the ’Why’ is your job. Finding the ’How’ is AI’s job. If you can’t tell the
difference, you’re the one being programmed, not the robot. Submissions with zero logic will
be treated as spam."

SOAL 1
Bagian ini menguji pemahaman CaKru mengenai environment Linux, penguasaan Command Line Interface (CLI), dan arsitektur WSL/Dual Boot. DILARANG memanipulasi data. Semua operasi pemindahan atau ekstraksi file wajib dilakukan melalui terminal menggunakan perintah dasar Linux, piping, dan redirection.
Install WSL: https://youtu.be/zZf4YH4WiZo?si=bBJDMFtotHubHK_P
Dual Boot on Windows (Opsional): https://youtu.be/mXyN1aJYefc?si=eFLpz3TgMl32kFuK
a.   	Arsitektur Sistem Operasi
Sebagai engineer robotika, CaKru diwajibkan memahami environment tempat sistem  beroperasi. Buatlah sebuah dokumen PDF (Jawaban_1_a.pdf) yang berisi penjelasan dengan Bahasa sendiri
1.        Jelaskan perbedaan fundamental arsitektur antara sistem operasi Windows, Linux yang dijalankan menggunakan metode WSL 2, dan Dual Boot.
2.        Mengapa OS Linux murni (Dual Boot) lebih disarankan dibandingkan WSL 2 pada kondisi pengembangan robotika tertentu? (Berikan penjelasan dan contoh kasus nyata di mana WSL 2 dapat mengalami kendala atau bottleneck saat pengerjaan proyek robot).
3.        Sebutkan minimal 2 (dua) karakteristik visual atau perintah bawaan yang paling membedakan terminal Windows (PowerShell/CMD) dengan terminal Linux (Bash/Zsh) saat digunakan.
 
b.   	Verifikasi Environment
Bagi pengguna Macbook, kerjakan poin 2 dan 3 secara mandiri di terminal bawaan macOS).
1.        Buka Windows Terminal. Lakukan Split Pane (bagi layar menjadi dua panel). Gunakan panel kiri untuk PowerShell/Command Prompt (Windows) dan panel kanan untuk Ubuntu (WSL).
2.        Jalankan perintah berikut secara bersamaan untuk menunjukkan perbedaan kernel dan identitas OS:
·        Kiri (Windows): wsl --list –verbose
·        Kanan (Linux/macOS): uname -sr && whoami
3.        Ambil screenshot layar penuh (Full Screen) yang menampilkan kedua panel tersebut bersandingan. Simpan gambar dengan nama bukti_split_os.png.
 
c.   	Manajemen Package & Manipulasi Data via CLI
1.        Pada terminal Linux, lakukan update repository lalu install package build-essential.
2.        Verifikasi instalasi build tools C++ dengan menjalankan perintah chaining berikut (jangan dipisah):
which g++ > compiler_trace.log && g++ --version | head -n 1 >> compiler_trace.log
3.        Buat sebuah direktori baru bernama recovery_ops di dalam direktori home (~), lalu masuk ke direktori tersebut.
4.        Simulasikan pengambilan data log sensor dari server pusat. Unduh file data mentah menggunakan perintah wget atau curl dari tautan berikut: [LINK TXT]
5.        CaKru diwajibkan melakukan ekstraksi data spesifik yang berada di urutan baris ke-1250 sampai ke-1260 dari file system_raw.txt. Gunakan kombinasi perintah piping (head dan tail) di terminal untuk mengekstrak kesebelas baris tersebut, lalu simpan output-nya ke dalam file baru bernama recovered_sector.txt. Hapus file system_raw.txt secara permanen.
6.        Buka direktori recovery_ops menggunakan VSCode yang dieksekusi langsung dari terminal WSL (gunakan perintah code .). Pastikan indikator "WSL: Ubuntu..." ada di pojok kiri bawah layar VSCode.
7.        Buka file recovered_sector.txt di VSCode tersebut dan ambil screenshot layar penuh. Simpan sebagai bukti_vscode.png.
8.        Kembali ke terminal, jalankan perintah history | tail -n 30 > history_audit.txt untuk merekam jejak 30 pengerjaan terakhir CaKru.
 
POIN BONUS KE NILAI KESELURUHAN URO TEST (OPSIONAL):
Khusus bagi Anda yang menggunakan Linux murni secara Dual Boot (bukan WSL/Virtual Machine), buktikan environment Anda untuk mendapat nilai tambahan:
1.        Buka terminal Linux, lalu jalankan perintah berikut untuk merekam status sistem operasi: systemd-detect-virt > bukti_native.txt && uname -r >> bukti_native.txt
2.        Jalankan perintah neofetch di terminal (install terlebih dahulu jika belum ada).
3.        Ambil FOTO fisik (gunakan kamera HP, dilarang menggunakan screenshot) yang memperlihatkan layar laptop secara utuh beserta output neofetch di terminal.
4.        Simpan foto tersebut dengan nama bukti_fisik_native.jpg.
5.        Kumpulkan file bukti_native.txt dan bukti_fisik_native.jpg ke dalam folder repository Anda.
 
Format Pengumpulan :
Folder Soal_1_(Nama)_(NIM)_Cakru18 pada Github yang berisikan:
·        Jawaban_1_a.pdf
·        bukti_split_os.png (Wajib bagi pengguna WSL)
·        bukti_vscode.png
·        compiler_trace.log
·        recovered_sector.txt (Hanya berisi 11 baris data ekstraksi)
·        history_audit.txt
·        bukti_native.txt & bukti_fisik_native.jpg (Khusus pengerjaan poin bonus Dual Boot)



SOAL 2
Bagian ini menguji pemahaman dasar Anda dalam memulai, mengonfigurasi, dan mengelola version control menggunakan Git. Kerjakan instruksi di bawah ini menggunakan Git Bash (Windows) atau Terminal (Linux/macOS).
1.        Buat repository kosong di GitHub dengan nama Sekuro18_Git_[NamaPanggilan].
2.        Buka terminal lokal Anda. Lakukan konfigurasi user Git (gunakan perintah git config untuk nama dan email).
3.        Buat folder baru di laptop Anda, masuk ke folder tersebut, dan lakukan inisiasi Git (git init).
4.        Buat satu file bernama main.cpp yang berisi fungsi C++ kosong (hanya include iostream dan main()).
5.        Cek status folder Git Anda (git status). Simpan buktinya dengan perintah: git status > bukti_status.txt
6.        Tambahkan file tersebut ke staging area (git add .), lalu lakukan penyimpanan (commit) pertama dengan pesan: "inisiasi github".
7.        Buat dan berpindahlah ke branch baru bernama v1. Tambahkan sebaris komentar “// ini versi 1” pada file main.cpp, lalu commit.

8.        Kembali ke branch main. Dari situ, buat dan berpindahlah ke branch lain bernama v2. Tambahkan komentar “// ini versi 2” di baris yang sama, lalu commit.

9.        Lakukan penggabungan (merge) antara branch v1 ke dalam branch v2 secara lokal. (Selesaikan Merge Conflict secara manual jika terjadi bentrokan baris, pertahankan kedua komentar, lalu commit).
10.   Cetak riwayat cabang Git Anda dengan perintah: git log --graph --oneline --all > riwayat_git.txt
11.   Hubungkan repositori lokal Anda ke GitHub dan push semua branch tersebut.
Format Pengumpulan:
Folder Soal_2_(Nama)_(NIM)_Cakru18 pada Github yang berisikan:
·        File bukti_status.txt
·        File riwayat_git.txt
·        Tautan repositori GitHub Anda (pastikan visibilitasnya publik saat dinilai).
 








SOAL 3

	Buatlah program robot dengan konsep pemrograman fungsi dan/atau object oriented programming. Program dibuat dengan sistem 1 input dan 1 output seperti 1 input sensor ultrasonic dan 1 output motor. Program robot ini menggunakan bahasa C++ dan menggunakan compiler C++. Disarankan untuk mempelajari sistem input dan output yang ingin dibuat. 
Tujuan: Menguji pemahaman logika sensor-aktuator menggunakan paradigma OOP.
Skenario: Anda diminta membuat program simulasi untuk Robot Pemadam Api. Robot akan terus membaca input dari sensor jarak (Ultrasonic). Jika ada rintangan di depannya, robot harus mengambil tindakan tertentu.
Instruksi Koding: Buatlah sebuah program C++ dengan ketentuan sebagai berikut:
Class RobotPemadam:
Private Members: 
int jarak (untuk menyimpan data sensor).
string status (untuk menyimpan status pergerakan).
Public Methods:
Fungsi inputSensor: Mengisi variabel jarak.
Fungsi prosesLogika():
Jika jarak > 20. status = "Maju Mencari Api".
Jika jarak <= 20 dan jarak > 5. status = "UDAH DEKET NIH BRAY".
Jika jarak <= 5. status = "Posisi Tepat! gas semprot kali ya!".
Fungsi cetakStatus(): Menampilkan output ke layar dengan format: 
[Sensor: XX cm] -> Action: [Status]

Fungsi main():
Gunakan perulangan agar program berjalan terus-menerus.
Minta pengguna memasukkan angka (simulasi input sensor).
Program berhenti jika pengguna memasukkan angka -99

Eksekusi dan Kompilasi
Kompilasi program Anda menggunakan compiler g++ di terminal (yang sudah Anda siapkan di Soal 1). Jalankan programnya, lalu tes dengan memasukkan beberapa angka secara berurutan (misal: 30, 15, 3, lalu -99). Ambil screenshot terminal yang menampilkan history input/output tersebut.






Format Pengumpulan:
Folder Soal_3_(Nama)_(NIM)_Cakru18 pada Github yang berisikan:
File source code murni robot_pemadam.cpp.
File bukti_running.png (screenshot terminal saat program dijalankan dan dites).

