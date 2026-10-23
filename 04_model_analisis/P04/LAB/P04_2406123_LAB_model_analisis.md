# Tabel Hubungan Use Case

| Sumber | Hubungan | Tujuan |
|---|---|---|
| Peminjam | Association | LAB-UC01: Lihat Ketersediaan Peralatan |
| Peminjam | Association | LAB-UC03: Ajukan Peminjaman |
| Mahasiswa | Association (khusus, tetap dari Pertemuan 3) | LAB-UC05: Cetak Bukti Pengajuan |
| Mahasiswa | Generalization → Peminjam | Mewarisi fungsi dari aktor Peminjam |
| Dosen | Generalization → Peminjam | Mewarisi fungsi dari aktor Peminjam |
| Petugas Laboratorium | Association | LAB-UC02: Kelola Data Peralatan |
| Petugas Laboratorium | Association | LAB-UC06: Proses Keputusan Peminjaman |
| Petugas Laboratorium | Association | LAB-UC11: Catat Pengembalian Peralatan |
| Kepala Laboratorium | Association | LAB-UC07: Lihat Laporan Peminjaman |
| LAB-UC03: Ajukan Peminjaman | `«include»` (tetap dari Pertemuan 3) | LAB-UC04: Periksa Ketersediaan |
| LAB-UC05: Cetak Bukti Pengajuan | `«extend»` (tetap dari Pertemuan 3) | LAB-UC03: Ajukan Peminjaman |
| LAB-UC08: Tambah Data Peralatan | Generalization → LAB-UC02: Kelola Data Peralatan | Fungsi khusus untuk menambah data peralatan |
| LAB-UC09: Ubah Data Peralatan | Generalization → LAB-UC02: Kelola Data Peralatan | Fungsi khusus untuk mengubah data peralatan |
| LAB-UC10: Hapus Data Peralatan | Generalization → LAB-UC02: Kelola Data Peralatan | Fungsi khusus untuk menghapus data peralatan |
| LAB-UC11: Catat Pengembalian Peralatan | `«include»` | LAB-UC12: Periksa Kondisi Peralatan |
| LAB-CO01 (Collaboration) | Realization → LAB-UC03: Ajukan Peminjaman | Merealisasikan proses pengajuan peminjaman |
| LAB-CO02 (Collaboration) | Realization → LAB-UC11: Catat Pengembalian Peralatan | Merealisasikan proses pencatatan pengembalian peralatan |