# 🖥️📚 TUGAS PBO – Pertemuan Kesembilan  

**Implementasi iReport Jasper pada Aplikasi CRUD Member Gym (Java Swing + JDBC + PostgreSQL)**  

---

## 📄 Studi Kasus  
Tugas ini dibuat untuk **memenuhi mata kuliah Pemrograman Berorientasi Objek (PBO)** dengan studi kasus pengembangan sistem **CRUD Data Member Gym** yang sebelumnya sudah dibuat pada pertemuan ke-6.  Pada versi kali ini, sistem dikembangkan dengan **integrasi laporan otomatis menggunakan iReport Jasper** yang terhubung langsung ke **database PostgreSQL**.  Hasil akhirnya berupa laporan data member yang dapat ditampilkan dan dicetak langsung dari aplikasi Java melalui **JasperViewer**.  

Data yang ditampilkan meliputi:  
- 🆔 ID Member  
- 👤 Nama  
- 🏋️‍♂️ Tipe Paket  
- 🧑‍🏫 Coach  


---

## 🧩 Peran iReport Jasper  
iReport Jasper berfungsi untuk **mendesain dan men-generate laporan otomatis** berdasarkan data di database.  

Fungsinya yakni:  
- 🗂️ **Desain Laporan (.jrxml / .jasper)**  
  Menentukan layout laporan (logo, header, tabel, footer).  
- 🔗 **Koneksi ke Database PostgreSQL**  
  Mengambil data langsung menggunakan query SQL (`SELECT * FROM member_gym`).  
- 🧾 **JasperViewer Integration**  
  Menampilkan hasil laporan langsung dari aplikasi dengan tampilan siap cetak.  


---

## ⚙️ Langkah-Langkah Implementasi  
1. **Instalasi iReport Designer**  
   - Unduh dari situs resmi Jaspersoft. Linknya (https://sourceforge.net/projects/erpbarcode/files/latest/download)
     <img width="741" height="547" alt="image" src="https://github.com/user-attachments/assets/39ff0795-632f-4f14-9992-ed079e11d4a7" />
     
   - Tambahkan plugin *JasperReport* dan *JDesktop Layout* ke NetBeans.
     <img width="741" height="547" alt="image" src="https://github.com/user-attachments/assets/f6a6e9ad-4b9f-473f-873a-30b527c6b6ac" />


2. **Konfigurasi Database Connection di iReport**  
   - Gunakan koneksi **PostgreSQL JDBC**.
     <img width="741" height="547" alt="image" src="https://github.com/user-attachments/assets/ea902638-2d03-45a4-8634-a0ddb38d26c4" />
     
   - Test Connection → pastikan status “Connection succeeded”.
     <img width="741" height="547" alt="image" src="https://github.com/user-attachments/assets/b4e020e2-9c63-46ef-b585-07798ac6718f" />


3. **Desain Template Laporan**  
   - Tambahkan elemen logo gym, judul, dan tabel kolom (`ID Member`, `Nama`, `Paket`, `Coach`).
     <img width="741" height="547" alt="image" src="https://github.com/user-attachments/assets/563156f0-9fa7-4673-bce2-fdeab014ca6e" />
     

4. **Integrasi Tombol Cetak di Aplikasi**  
   - Tambahkan tombol **“Cetak”** pada `MemberFrame.java`.
     <img width="741" height="547" alt="image" src="https://github.com/user-attachments/assets/cdc4b379-8fb5-48c9-9085-cd91bd6b4f66" />
     
     <img width="741" height="547" alt="image" src="https://github.com/user-attachments/assets/02f31405-fa01-403f-a8b6-b0724320e14a" />
    

5. **Uji Coba Program**  
   - Klik tombol Cetak → Laporan muncul otomatis dengan data terbaru dari database.
     <img width="741" height="547" alt="image" src="https://github.com/user-attachments/assets/ddbc2bc7-b437-4f82-8006-58537c2ea96c" />
     
   - Laporan siap disimpan atau dicetak langsung.
     <img width="844" height="1019" alt="image" src="https://github.com/user-attachments/assets/6c5d5a8c-997f-4e60-bd6b-d1f271b69604" />


---

## 🖼️ Tampilan Aplikasi  

- Tampilan Form Utama dengan data member gym.  
  <img width="741" height="547" alt="image" src="https://github.com/user-attachments/assets/f049db2b-4c3f-4fd3-9294-06c0a844f5e3" />
  
- Desain Laporan di iReport.  
  <img width="747" height="547" alt="image" src="https://github.com/user-attachments/assets/a9d65a52-a22a-4835-8178-2da00c8c315d" />
  
- Hasil Cetak Laporan via JasperViewer.  
  <img width="622" height="880" alt="image" src="https://github.com/user-attachments/assets/2e3a0fe8-3cde-4642-9b02-ea556b98a48c" />



---

## 👨‍💻 Author  
**Ryo Satriagung Hidayat**  
NIM: 09010624015  
Program Studi: Sistem Informasi  
Universitas Islam Negeri Sunan Ampel Surabaya – 2025  

---
