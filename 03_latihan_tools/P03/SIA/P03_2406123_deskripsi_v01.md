# Ajukan KRS
| Elemen | SIA-R03 - Ajukan KRS |
| :--- | :--- |
| Tujuan                | Menghasilkan pengajuan KRS yang dipilih                                   |
| Aktor utama           | Mahasiswa                                                                 |
| Sumber kebutuhan      | SIA-R03 dan SIA-R04                                                       |
| Pemicu                | Mahasiswa memilih fungsi pengajuan KRS                                    |
| Prasyarat             | Mahasiswa telah terautentikasi; data mata kuliah tersedia                 |
| Pascakondisi berhasil | Pengajuan tersimpan dan jadwal tersedia; menunggu persetujuaan dosen wali |
| Pascakondisi gagal    | Data gagal tersimpan                                                      |
| Include               | SIA-R04 - Validasi KRS                                                    |
| Extension point       | Konfirmasi penyimpanan /bukti pengajuan tersedia                          |  
| Extend                | SIA-UC05- jika [mahasiswa memilih menyimpan bukti ]                       |

# Validasi KRS
| Elemen | SIA-R04 — Validasi KRS |
| :--- | :--- |
| Tujuan                | Memastikan pengajuan KRS memenuhi ketentuan                 |
| Aktor utama           | Sistem                                                      |
| Sumber kebutuhan      | SIA-R03 dan SIA-R04                                         |
| Pemicu                | Mahasiswa mengajukan KRS                                    |
| Prasyarat             | Mahasiswa telah memilih mata kuliah                         |
| Pascakondisi berhasil | KRS dinyatakan valid dan dapat disimpan                     |
| Pascakondisi gagal    | Pengajuan KRS ditolak karena tidak lengkap,                 |
|                       | prasyarat tidak terpenuhi, atau jadwal bentrok              |
| Include               | -                                                           |
| Extension point       | Hasil validasi KRS                                          |
| Extend                | -                                                           |

# Unduh bukti pengajuan KRS
| Elemen | SIA-UC06 — Proses Keputusan KRS |
| :--- | :--- |
| Tujuan                | Menentukan persetujuan atau penolakan pengajuan KRS         |
| Aktor utama           | Dosen Wali                                                  |
| Sumber kebutuhan      | SIA-R03                                                     |
| Pemicu                | Dosen wali membuka pengajuan KRS yang menunggu persetujuan  |
| Prasyarat             | Pengajuan KRS telah tersimpan dan menunggu persetujuan      |
| Pascakondisi berhasil | Status KRS berubah menjadi disetujui atau ditolak,          |
|                       | disertai catatan keputusan                                  |
| Pascakondisi gagal    | Keputusan gagal disimpan dan status KRS tidak berubah       |
| Include               | -                                                           |
| Extension point       | Penentuan keputusan KRS                                     |
| Extend                | -                                                           |

# Proses keputusan KRS.
| Elemen | SIA-UC06 — Proses Keputusan KRS |
| :--- | :--- |
| Tujuan                | Menentukan persetujuan atau penolakan pengajuan KRS         |
| Aktor utama           | Dosen Wali                                                  |
| Sumber kebutuhan      | SIA-R03                                                     |
| Pemicu                | Dosen wali membuka pengajuan KRS yang menunggu persetujuan  |
| Prasyarat             | Pengajuan KRS telah tersimpan dan menunggu persetujuan      |
| Pascakondisi berhasil | Status KRS berubah menjadi disetujui atau ditolak,          |
|                       | disertai catatan keputusan                                  |
| Pascakondisi gagal    | Keputusan gagal disimpan dan status KRS tidak berubah       |
| Include               | -                                                           |
| Extension point       | Penentuan keputusan KRS                                     |
| Extend                | -                                                           |
