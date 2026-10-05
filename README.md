# DigiPlan (Digital Planner)

**Kelompok 2 – EdTech** · Product Requirements Document (PRD)

## 1. Latar Belakang
Mahasiswa dan siswa sering lupa tenggat tugas, menunda pekerjaan, lalu kelelahan (burnout). Portal akademik konvensional mengharuskan login berulang hanya untuk melihat jadwal atau tugas. Dibutuhkan aplikasi seluler yang mengambil data akademik secara otomatis dan mengingatkan penggunanya.

## 2. Tujuan
- Menarik jadwal dan tugas dari LMS otomatis, tanpa input manual.
- Menyusun jadwal harian otomatis (Smart Scheduling) berdasarkan bobot dan sisa waktu tugas.
- Memberi notifikasi bertingkat dan rekomendasi jam belajar saat tugas menumpuk.
- Menampilkan dashboard adaptif sesuai jenjang (IPK untuk mahasiswa, rata-rata nilai untuk siswa).

## 3. Deskripsi Produk
DigiPlan adalah aplikasi seluler sebagai asisten akademik. Fitur utama: sinkronisasi LMS, Smart Scheduling, notifikasi proaktif, dashboard adaptif, pelacakan tugas kelompok, dan gamifikasi pencapaian.

## 4. Kebutuhan Pengguna
- Sebagai mahasiswa/siswa, saya ingin tugas dari LMS masuk otomatis agar tidak perlu menyalin manual.
- Sebagai pengguna, saya ingin melihat tugas paling mendesak di dashboard agar tidak melewatkan tenggat.
- Sebagai pengguna, saya ingin diingatkan sebelum tugas menumpuk agar tidak burnout.
- Sebagai anggota kelompok, saya ingin melihat progres tugas kelompok agar pembagian kerja jelas.
- Sebagai pengguna, saya ingin menambah jadwal non-akademik secara manual.

## 5. Ruang Lingkup
**Termasuk:** autentikasi (Sign In/Sign Up/Reset Password), onboarding jenjang dan mata pelajaran, dashboard, sinkronisasi LMS, jadwal dan tugas, tugas kelompok, notifikasi, pencapaian, pengaturan.

**Tidak termasuk:** fitur nilai/rapor lengkap, chat antar pengguna, dan versi iOS/Android native terpisah (tahap awal hanya prototipe UI).

## 6. Persyaratan Fungsional
| Kode | Persyaratan | Entitas ERD |
|---|---|---|
| FR-01 | Pengguna dapat mendaftar, login, dan reset password dengan kode verifikasi | Pengguna |
| FR-02 | Pengguna memilih jenjang (SD/SMP/SMA/Universitas) dan mata pelajaran | Pengguna, Mata Pelajaran |
| FR-03 | Sistem menyinkronkan jadwal dan tugas dari LMS, menampilkan waktu sinkron terakhir | LMS, Jadwal, Tugas |
| FR-04 | Pengguna dapat menambah jadwal manual | Jadwal |
| FR-05 | Sistem mengurutkan tugas berdasarkan prioritas dan deadline, dengan penanda warna | Tugas, Kategori Tugas |
| FR-06 | Sistem menyusun timeline harian otomatis (Smart Scheduling) | Jadwal, Tugas |
| FR-07 | Tugas dapat dikerjakan individu atau kelompok, dengan peran dan persentase progres | Tugas (relasi Mengerjakan) |
| FR-08 | Sistem mengirim notifikasi pengingat, peringatan dini, dan rekomendasi jam belajar | Notifikasi |
| FR-09 | Pengguna mendapat lencana (badge) saat menyelesaikan tugas | Pencapaian |
| FR-10 | Pengguna mengatur profil, preferensi notifikasi, mode senyap, dan kredensial LMS | Pengguna, LMS |

## 7. Persyaratan Non-Fungsional
- **Keamanan:** password disimpan ter-hash, kredensial LMS dienkripsi.
- **Performa:** dashboard tampil kurang dari 3 detik (usulan).
- **Kegunaan:** Clean UI biru-putih, font Inter, mudah dijangkau ibu jari.
- **Keandalan:** notifikasi tetap terkirim walau aplikasi tidak dibuka.
- **Skalabilitas:** mendukung banyak pengguna dan banyak LMS.

## 8. Jadwal dan Timeline
| Tahap | Waktu |
|---|---|
| Mentoring (6 sesi) | 13–23 April 2026 |
| Presentasi dan pameran poster | 25 April 2026 |

## 9. Risiko dan Asumsi
**Risiko:** LMS institusi tidak menyediakan akses data otomatis (API); data LMS tidak seragam antar kampus/sekolah; pengguna merasa notifikasi terlalu banyak.

**Asumsi:** pengguna punya akun LMS aktif dan koneksi internet; pengguna mengisi jenjang pendidikan saat registrasi.

## 10. Anggota Kelompok
| No | Nama | NPM |
|---|---|---|
| 1 | Irvan Indra Mustofa | 4525210107 |
| 2 | Muhamad Rasha Zein | 4525210042 |
| 3 | Muhammad Farrel Rizky | 4525210117 |
| 4 | Muzaki Arifin | 4525210051 |
| 5 | Nur Wahyu Muhtiin Haniv | 4525210078 |
| 6 | Rangga Prataya Setiono Putro | 4525210131 |

## 11. LINK ERD BY GDRIVE 
[ERD Digiplan](https://drive.google.com/file/d/1eh9J8d0jQ2jOiSbpdC-Ewr1v2XvvXRc4/view?usp=sharing)
