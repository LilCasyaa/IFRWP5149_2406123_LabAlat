Mahasiswa dan dosen sama-sama merupakan Civitas Akademika yang
dapat melihat kalender akademik. Dosen menginput nilai mata kuliah yang
diampunya setelah masa perkuliahan berakhir. Mahasiswa melihat Kartu
Hasil Studi (KHS) untuk semester yang nilainya sudah dipublikasikan. Admin
Akademik mengelola data mahasiswa: menambah data mahasiswa baru,
mengubah data mahasiswa, dan menghapus data mahasiswa. Dua use case
utama, Input Nilai Mata Kuliah dan Lihat KHS, ditunjukkan realisasinya oleh
collaboration yang bersesuaian.

# Batas dan asumsi
• Kode kebutuhan dimulai dari SIA-R07 agar SIA-R01 dan SIA-R02
(Pertemuan 2) serta SIA-R03 sampai SIA-R06 (Pertemuan 3) tetap
mempunyai identitas berbeda.
• Pengguna telah terautentikasi dan memiliki hak akses sesuai peran.
• Kalender akademik pada tugas ini adalah agenda resmi institusi (awal
semester, batas KRS, masa ujian, dan sejenisnya); jangan
menyamakannya dengan jadwal kuliah pada Pertemuan 2.
• Nilai hanya dapat diinput oleh dosen pengampu mata kuliah tersebut. Nilai
yang diinput belum terpublikasi sebelum dinyatakan resmi oleh ketentuan
tugas ini: KHS hanya menampilkan nilai yang sudah dipublikasikan.
• Hapus Data Mahasiswa hanya untuk mahasiswa yang tidak memiliki data
akademik aktif. Ketentuan ini fiktif untuk latihan.
• Pengajuan KRS tetap digambar sebagai bagian diagram kumulatif dari
Pertemuan 3. Pembayaran dan perancangan basis data berada di luar
tugas ini.

### Identifikasi aktor dan use case

| Aktor | Kedudukan | Tujuan terhadap Sistem |
|---|---|---|
| Civitas Akademika | Aktor umum | Melihat kalender akademik untuk mengetahui informasi dan agenda akademik yang berlaku. |
| Mahasiswa | Aktor khusus dari Civitas Akademika | Melihat jadwal kuliah, mengajukan KRS, mengunduh bukti pengajuan KRS, melihat kalender akademik, dan melihat KHS untuk semester yang nilainya telah dipublikasikan. |
| Dosen | Aktor khusus dari Civitas Akademika | Melihat kalender akademik dan menginput nilai mata kuliah yang diampunya setelah masa perkuliahan berakhir. |
| Admin Akademik | Aktor pengelola administrasi akademik | Mengelola jadwal kuliah serta mengelola data mahasiswa melalui proses penambahan, perubahan, dan penghapusan data. |
| Dosen Wali | Aktor pada proses KRS | Memproses keputusan KRS mahasiswa sesuai dengan ketentuan akademik yang berlaku. |

# Tabel Katalog Use Case

| ID | Nama use case | Aktor/keterangan | Status |
|---|---|---|---|
| SIA-UC01 | Lihat Jadwal Kuliah | Mahasiswa | Tetap, P2 |
| SIA-UC02 | Kelola Jadwal Kuliah | Admin Akademik | Tetap, P2 |
| SIA-UC03 | Ajukan KRS | Mahasiswa | Tetap, P3 |
| SIA-UC04 | Validasi KRS | Bagian dari proses pengajuan KRS | Tetap, P3 |
| SIA-UC05 | Unduh Bukti Pengajuan KRS | Mahasiswa | Tetap, P3 |
| SIA-UC06 | Proses Keputusan KRS | Dosen Wali | Tetap, P3 |
| SIA-UC07 | Lihat Kalender Akademik | Civitas Akademika | Baru, P4 |
| SIA-UC08 | Input Nilai Mata Kuliah | Dosen | Baru, P4 |
| SIA-UC09 | Lihat KHS | Mahasiswa | Baru, P4 |
| SIA-UC10 | Kelola Data Mahasiswa | Admin Akademik; use case umum | Baru, P4 |
| SIA-UC11 | Tambah Data Mahasiswa | Admin Akademik; use case khusus | Baru, P4 |
| SIA-UC12 | Ubah Data Mahasiswa | Admin Akademik; use case khusus | Baru, P4 |
| SIA-UC13 | Hapus Data Mahasiswa | Admin Akademik; use case khusus | Baru, P4 |

# Tabel generalization use case
| Use Case Khusus | Use Case Umum | Perilaku yang Membedakan |
|---|---|---|
| SIA-UC11: Tambah Data Mahasiswa | SIA-UC10: Kelola Data Mahasiswa | Menambahkan data mahasiswa baru. |
| SIA-UC12: Ubah Data Mahasiswa | SIA-UC10: Kelola Data Mahasiswa | Mengubah data mahasiswa yang sudah tersimpan. |
| SIA-UC13: Hapus Data Mahasiswa | SIA-UC10: Kelola Data Mahasiswa | Menghapus data mahasiswa yang tidak memiliki data akademik aktif. |

# Tabel collaboration dan realization
| ID Collaboration | Nama Collaboration | Use Case yang Direalisasikan |
|---|---|---|
| SIA-CO01 | Input Nilai Mata Kuliah | SIA-UC08: Input Nilai Mata Kuliah |
| SIA-CO02 | Lihat KHS | SIA-UC09: Lihat KHS |