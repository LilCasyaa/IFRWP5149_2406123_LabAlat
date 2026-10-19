Mahasiswa mengajukan KRS dengan memilih mata kuliah Setiap pengajuan menjalankan validasi KRS yang memeriksa kelengkapan, prasyarat mata kuliah, dan benturan jadwal. Jika validasi berhasil, sistem menyimpan pengajuan berstatus menunggu persetujuan dosen wali. Pada konfirmasi penyimpanan, mahasiswa dapat memilih mengunduh bukti pengajuan. Dosen wali menyetujui atau menolak KRS dan memberikan catatan keputusan.

# Tabel Daftar Kebutuhan Sistem
| ID | Kebutuhan Tugas |
| :---: | :--- |
|SIA-R01 | Mahasiswa dapat melihat jadwal kuliah                                    |
|SIA-R02 | Admin akademik dapat mengelola jadwal kuliah                             | 
|SIA-R03 | Mahasiswa dapat mengajukan KRS                                           |
|SIA-R04 | Sistem memvalidasi KRS sebagai bagian pengajuan                          |
|SIA-R05 | Mahasiswa dapat mengunduh bukti jika memilihnya pada konfirmasi pengajuan|
|SIA-R06 | Dosen wali dapat memproses persetujuan atau penolakan KRS                |


Batas dan asumsi:
• Pengguna telah terautentikasi.
• Data mata kuliah, prasyarat, dan jadwal tersedia.
• Validasi gagal menyebabkan pengajuan belum berhasil tersimpan.
• Unduh bukti tidak menjadi syarat keberhasilan pengajuan.
• KRS tersimpan belum berarti disetujui.
• Pembayaran, pengisian nilai, dan implementasi basis data berada di luar tugas.

# Tabel Identifikasi Aktor
| Aktor | Tujuan Terhadap Sistem 
| :---: | :---- |
| Mahasiswa  | Mengajukan KRS dengan memilih mata kuliah;                                  |
|            | Memilih apakah akan mengunduh bukti pengajuan KRS setelah berhasil disimpan |
| Dosen Wali | Memeriksa pengajuan KRS mahasiswa;                                          |
|            | Menyetujui atau menolak KRS dan memberikan catatan keputusan                |


# Tabel Daftar Use Case
|    ID    | Nama use case	Peran dalam model                        |
| :---: | :---- |
| SIA-UC01 | Ajukan KRS	Fungsi utama mahasiswa                       | 
| SIA-UC02 | Validasi KRS	Perilaku yang disertakan UC01            | 
| SIA-UC03 | Unduh bukti pengajuan KRS	Tambahan bersyarat pada UC01 |
| SIA-UC04 | Proses keputusan KRS	Fungsi utama dosen wali          |
|----------+---------------------------------------------------------|

# Relasi Include
SIA-UC03 «include» SIA-UC04 
Extension point: Bukti pengajuan tersedia.
Kondisi: [mahasiswa memilih mengunduh bukti].
Alasan: validasi kelengkapan, prasyarat, dan benturan jadwal selalu menjadi bagian dari setiap pengajuan KRS.

# Relasi Extend
SIA-UC05 «extend» SIA-UC03 
Extension point: Bukti pengajuan tersedia 
Kondisi: [mahasiswa memilih unduh] 
Alasan: pengajuan tetap berhasil tanpa pengunduhan bukti.
