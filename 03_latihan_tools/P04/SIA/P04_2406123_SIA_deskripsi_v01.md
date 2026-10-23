## Tabel Use Case SIA-UC07
| Elemen | SIA-UC07 — Lihat Kalender Akademik |
|---|---|
| Sumber Kebutuhan | SIA-R07 |
| Tujuan | Menampilkan kalender akademik resmi institusi. |
| Aktor Utama | Civitas Akademika (Mahasiswa dan Dosen). |
| Pemicu | Civitas akademika memilih fungsi lihat kalender akademik. |
| Prasyarat | Pengguna telah terautentikasi; data kalender akademik tersedia. |
| Pascakondisi Berhasil | Kalender akademik resmi institusi ditampilkan. |
| Pascakondisi Gagal | Kalender akademik tidak ditampilkan; tidak ada data yang berubah. |
| Include | - |
| Extension Point | - |
| Extend | - |
| Collaboration | - |
| Generalization | - |

## Tabel Use Case SIA-UC08
| Elemen | Keterangan |
|---|---|
| ID dan Nama | SIA-UC08: Input Nilai Mata Kuliah |
| Sumber Kebutuhan | SIA-R08 dan SIA-R12 |
| Tujuan | Menyimpan nilai mata kuliah yang diampu dosen untuk diproses sesuai ketentuan publikasi nilai. |
| Aktor Utama | Dosen |
| Aktor Pendukung | Tidak ditetapkan dalam skenario. |
| Pemicu | Dosen membuka fungsi Input Nilai Mata Kuliah setelah masa perkuliahan berakhir. |
| Prasyarat | Dosen telah login dan merupakan pengampu mata kuliah yang dipilih. |
| Generalization | Tidak ada. |
| Collaboration | SIA-CO01: Input Nilai Mata Kuliah. |
| Pascakondisi Berhasil | Nilai yang valid tersimpan untuk mata kuliah yang diampu dosen. Nilai belum dianggap dipublikasikan hanya karena sudah diinput. |
| Pascakondisi Gagal | Nilai tidak disimpan atau tidak berubah apabila input ditolak. |

## Tabel Use Case SIA-UC09
| Elemen | Keterangan |
|---|---|
| ID dan Nama | SIA-UC09: Lihat KHS |
| Sumber Kebutuhan | SIA-R09 dan SIA-R12 |
| Tujuan | Mahasiswa melihat Kartu Hasil Studi untuk semester yang dipilih. |
| Aktor Utama | Mahasiswa |
| Pemicu | Mahasiswa memilih fungsi Lihat KHS dan memilih semester. |
| Prasyarat | Mahasiswa telah login. |
| Alur Utama | Sistem menampilkan KHS semester yang dipilih dengan hanya menampilkan nilai yang sudah dipublikasikan. |
| Alur Alternatif | Jika nilai belum dipublikasikan, nilai tersebut tidak ditampilkan sebagai nilai resmi pada KHS. |
| Pascakondisi Berhasil | KHS ditampilkan berdasarkan nilai yang sudah dipublikasikan. |
| Pascakondisi Gagal | KHS tidak ditampilkan apabila data tidak dapat diakses; tidak ada data nilai yang diubah. |
| Collaboration | SIA-CO02: Lihat KHS. |

## Tabel Use Case SIA-UC10
| Elemen | SIA-UC10 — Kelola Data Mahasiswa |
|---|---|
| Sumber Kebutuhan | SIA-R10 dan SIA-R11 |
| Tujuan | Mengelola data mahasiswa melalui tambah, ubah, dan hapus. |
| Aktor Utama | Admin Akademik |
| Pemicu | Admin Akademik memilih fungsi Kelola Data Mahasiswa. |
| Prasyarat | Admin Akademik telah terautentikasi dan memiliki hak akses. |
| Pascakondisi Berhasil | Data mahasiswa berhasil ditambah, diubah, atau dihapus sesuai bentuk yang dipilih. |
| Pascakondisi Gagal | Data mahasiswa tidak berubah. |
| Include | - |
| Extension Point | - |
| Extend | - |
| Collaboration | - |
| Generalization | Induk dari SIA-UC11, SIA-UC12, dan SIA-UC13. |

## Tabel Use Case SIA-UC11
| Elemen | SIA-UC11 — Tambah Data Mahasiswa |
|---|---|
| Sumber Kebutuhan | SIA-R11 |
| Tujuan | Menambahkan data mahasiswa baru ke sistem. |
| Aktor Utama | Admin Akademik |
| Pemicu | Admin Akademik memilih bentuk tambah data mahasiswa. |
| Prasyarat | Admin Akademik telah terautentikasi; data mahasiswa baru lengkap. |
| Pascakondisi Berhasil | Data mahasiswa baru tersimpan. |
| Pascakondisi Gagal | Data mahasiswa baru tidak tersimpan. |
| Include | - |
| Extension Point | - |
| Extend | - |
| Collaboration | - |
| Generalization | SIA-UC10 — Kelola Data Mahasiswa. |

## Tabel Use Case SIA-UC12
| Elemen | SIA-UC12 — Ubah Data Mahasiswa |
|---|---|
| Sumber Kebutuhan | SIA-R11 |
| Tujuan | Memperbarui data mahasiswa yang sudah ada. |
| Aktor Utama | Admin Akademik |
| Pemicu | Admin Akademik memilih bentuk ubah data mahasiswa. |
| Prasyarat | Admin Akademik telah terautentikasi; data mahasiswa yang diubah tersedia. |
| Pascakondisi Berhasil | Perubahan data mahasiswa tersimpan. |
| Pascakondisi Gagal | Data mahasiswa tidak berubah. |
| Include | - |
| Extension Point | - |
| Extend | - |
| Collaboration | - |
| Generalization | SIA-UC10 — Kelola Data Mahasiswa. |

## Tabel Use Case SIA-UC13
| Elemen | SIA-UC13 — Hapus Data Mahasiswa |
|---|---|
| Sumber Kebutuhan | SIA-R11 |
| Tujuan | Menghapus data mahasiswa yang tidak lagi diperlukan. |
| Aktor Utama | Admin Akademik |
| Pemicu | Admin Akademik memilih bentuk hapus data mahasiswa. |
| Prasyarat | Admin Akademik telah terautentikasi; mahasiswa tidak memiliki data akademik aktif (ketentuan fiktif latihan). |
| Pascakondisi Berhasil | Data mahasiswa terhapus. |
| Pascakondisi Gagal | Data mahasiswa tidak terhapus. |
| Include | - |
| Extension Point | - |
| Extend | - |
| Collaboration | - |
| Generalization | SIA-UC10 — Kelola Data Mahasiswa. |