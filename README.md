# Minpro-2-DDP-Muhammad-Fachri-Razabi_069

Nama: Muhammad Fachri Razabi

Nim: 2609116069

Kelas: B

INPUT

<img width="467" height="458" alt="Screenshot 2026-10-06 171531" src="https://github.com/user-attachments/assets/45ec87a1-a782-4476-8578-883072061bbf" />

<img width="535" height="471" alt="Screenshot 2026-10-06 171628" src="https://github.com/user-attachments/assets/396cc2c3-7660-469e-ba28-601a178584c8" />

<img width="432" height="456" alt="Screenshot 2026-10-06 171712" src="https://github.com/user-attachments/assets/b0d858a8-4fe7-4e5c-85ca-aa7da4663506" />

<img width="524" height="437" alt="Screenshot 2026-10-06 171831" src="https://github.com/user-attachments/assets/a3c15099-eaaf-44a4-8fca-ecef322d04b0" />

<img width="420" height="262" alt="Screenshot 2026-10-06 171900" src="https://github.com/user-attachments/assets/afe90ae3-b6e0-40ab-8b10-23bed298a868" />

Program ini adalah sistem pencatatan muatan CPO berbasis menu, dengan login dan pembagian hak akses.

Kode

Library: json menyimpan data ke file agar tidak hilang saat program ditutup, os mengecek keberadaan file, dan datetime mencatat waktu input.

Dictionary: akun menyimpan username, password, dan role. data_muatan menyimpan data kapal (nama, tujuan, jumlah, waktu) dengan ID sebagai key. menu_role menentukan menu tiap role.

Role: admin punya CRUD lengkap (tambah, tampil, ubah, hapus) dan cari. User hanya bisa menampilkan dan mencari data.
Function: login(), tambah_data(), tampilkan_data(), ubah_data(), hapus_data(), cari_data(), menu(), dan main().

Validasi: memakai if/elif/else untuk input kosong, jumlah bukan angka, ID tidak ditemukan, dan pilihan menu salah.

OUTPUT

<img width="241" height="387" alt="Screenshot 2026-10-06 170501" src="https://github.com/user-attachments/assets/089c851b-ade6-4538-9766-58a56997ccaa" />

Gambar 1: Login dan tambah data pertama. Program menampilkan menu utama. Pengguna memilih Login dan masuk sebagai admin, lalu muncul menu admin dengan 6 pilihan. Data kapal pertama (MT Borneo Jaya, Rotterdam, 5000 ton) berhasil ditambahkan.

<img width="257" height="389" alt="Screenshot 2026-10-06 170548" src="https://github.com/user-attachments/assets/da5a1031-041c-4056-9c89-725df40ec116" />

Gambar 2: Tambah data, validasi, tampil, dan ubah. Data kedua ditambahkan. Percobaan menambah data dengan tujuan kosong ditolak dengan pesan "Gagal!", sehingga validasi terbukti bekerja. Menu Tampilkan Data menampilkan 2 data dengan total 8200 ton. Setelah itu data ID 2 diubah (tujuan menjadi Surabaya, jumlah menjadi 3500 ton), sementara nama kapal dikosongkan sehingga tidak berubah.

<img width="263" height="392" alt="Screenshot 2026-10-06 170633" src="https://github.com/user-attachments/assets/83e932d1-7cbc-4f3c-8c69-f820da9780a1" />

Gambar 3: Hapus data. Admin memilih data ID 1 dan program meminta konfirmasi. Setelah dijawab "y", data MT Borneo Jaya terhapus. Tampilan data berikutnya hanya menyisakan 1 data dengan total 3500 ton.

<img width="277" height="71" alt="Screenshot 2026-10-06 170653" src="https://github.com/user-attachments/assets/cb5a4086-6f13-462b-a3cd-6c11f3cdc944" />

Gambar 4: Logout dan keluar. Admin logout dan kembali ke menu utama, lalu memilih Keluar. Program menampilkan ucapan terima kasih dan berhenti.

FLOWCHART

<img width="264" height="364" alt="Screenshot 2026-10-06 183548" src="https://github.com/user-attachments/assets/c8e0e0c8-6598-4818-92f5-f5c494bf7f18" />

Alur program dimulai dari menu utama, lalu pengguna login (maksimal 3 kali) dan masuk ke menu sesuai role, yaitu admin dengan CRUD lengkap atau user yang hanya bisa melihat dan mencari data, sampai logout dan kembali ke menu utama.
