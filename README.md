# Pratikum8
# Data Diri
Nama : Rafli Dhiya Fadhaly

Nim : 312410251

Kelas : TI 24 a2
# masukan dan keluaran dari Praktikum 8
## Input 
```python
class DaftarMahasiswa:
    def _init_(self):
        self.data_mahasiswa = []

    def tambah(self):
        """Menambah data mahasiswa baru."""
        nama = input("Masukkan nama mahasiswa: ")
        nilai = float(input("Masukkan nilai mahasiswa: "))
        self.data_mahasiswa.append({"nama": nama, "nilai": nilai})
        print("Data mahasiswa berhasil ditambahkan.")

    def tampilkan(self):
        """Menampilkan semua data mahasiswa."""
        if not self.data_mahasiswa:
            print("Data mahasiswa masih kosong.")
        else:
            print("Daftar Nilai Mahasiswa:")
            print("--------------------------")
            for mahasiswa in self.data_mahasiswa:
                print(f"Nama: {mahasiswa['nama']}, Nilai: {mahasiswa['nilai']}")
                print("--------------------------")

    def hapus(self, nama):
        """Menghapus data mahasiswa berdasarkan nama."""
        for i, mahasiswa in enumerate(self.data_mahasiswa):
            if mahasiswa['nama'].lower() == nama.lower():
                del self.data_mahasiswa[i]
                print(f"Data mahasiswa dengan nama {nama} berhasil dihapus.")
                return
        print(f"Data mahasiswa dengan nama {nama} tidak ditemukan.")

    def ubah(self, nama):
        """Mengubah data mahasiswa berdasarkan nama."""
        for mahasiswa in self.data_mahasiswa:
            if mahasiswa['nama'].lower() == nama.lower():
                nilai_baru = float(input("Masukkan nilai baru: "))
                mahasiswa['nilai'] = nilai_baru
                print(f"Data mahasiswa dengan nama {nama} berhasil diubah.")
                return
        print(f"Data mahasiswa dengan nama {nama} tidak ditemukan.")

# Inisialisasi objek DaftarMahasiswa
daftar_mahasiswa = DaftarMahasiswa()

# Menu program
while True:
    print("\nMenu:")
    print("1. Tambah data mahasiswa")
    print("2. Tampilkan data mahasiswa")
    print("3. Hapus data mahasiswa")
    print("4. Ubah data mahasiswa")
    print("5. Keluar")
    pilihan = input("Pilih menu (1/2/3/4/5): ")

    if pilihan == '1':
        daftar_mahasiswa.tambah()
    elif pilihan == '2':
        daftar_mahasiswa.tampilkan()
    elif pilihan == '3':
        nama = input("Masukkan nama mahasiswa yang ingin dihapus: ")
        daftar_mahasiswa.hapus(nama)
    elif pilihan == '4':
        nama = input("Masukkan nama mahasiswa yang ingin diubah: ")
        daftar_mahasiswa.ubah(nama)
    elif pilihan == '5':
        print("Terima kasih! Program selesai.")
        break
    else:
        print("Pilihan tidak valid.") class DaftarMahasiswa:
    def _init_(self):
        self.data_mahasiswa = []

    def tambah(self):
        """Menambah data mahasiswa baru."""
        nama = input("Masukkan nama mahasiswa: ")
        nilai = float(input("Masukkan nilai mahasiswa: "))
        self.data_mahasiswa.append({"nama": nama, "nilai": nilai})
        print("Data mahasiswa berhasil ditambahkan.")

    def tampilkan(self):
        """Menampilkan semua data mahasiswa."""
        if not self.data_mahasiswa:
            print("Data mahasiswa masih kosong.")
        else:
            print("Daftar Nilai Mahasiswa:")
            print("--------------------------")
            for mahasiswa in self.data_mahasiswa:
                print(f"Nama: {mahasiswa['nama']}, Nilai: {mahasiswa['nilai']}")
                print("--------------------------")

    def hapus(self, nama):
        """Menghapus data mahasiswa berdasarkan nama."""
        for i, mahasiswa in enumerate(self.data_mahasiswa):
            if mahasiswa['nama'].lower() == nama.lower():
                del self.data_mahasiswa[i]
                print(f"Data mahasiswa dengan nama {nama} berhasil dihapus.")
                return
        print(f"Data mahasiswa dengan nama {nama} tidak ditemukan.")

    def ubah(self, nama):
        """Mengubah data mahasiswa berdasarkan nama."""
        for mahasiswa in self.data_mahasiswa:
            if mahasiswa['nama'].lower() == nama.lower():
                nilai_baru = float(input("Masukkan nilai baru: "))
                mahasiswa['nilai'] = nilai_baru
                print(f"Data mahasiswa dengan nama {nama} berhasil diubah.")
                return
        print(f"Data mahasiswa dengan nama {nama} tidak ditemukan.")

# Inisialisasi objek DaftarMahasiswa
daftar_mahasiswa = DaftarMahasiswa()

# Menu program
while True:
    print("\nMenu:")
    print("1. Tambah data mahasiswa")
    print("2. Tampilkan data mahasiswa")
    print("3. Hapus data mahasiswa")
    print("4. Ubah data mahasiswa")
    print("5. Keluar")
    pilihan = input("Pilih menu (1/2/3/4/5): ")

    if pilihan == '1':
        daftar_mahasiswa.tambah()
    elif pilihan == '2':
        daftar_mahasiswa.tampilkan()
    elif pilihan == '3':
        nama = input("Masukkan nama mahasiswa yang ingin dihapus: ")
        daftar_mahasiswa.hapus(nama)
    elif pilihan == '4':
        nama = input("Masukkan nama mahasiswa yang ingin diubah: ")
        daftar_mahasiswa.ubah(nama)
    elif pilihan == '5':
        print("Terima kasih! Program selesai.")
        break
    else:
        print("Pilihan tidak valid.")
```

## Output
```python
Menu:
1. Tambah data mahasiswa   
2. Tampilkan data mahasiswa
3. Hapus data mahasiswa    
4. Ubah data mahasiswa     
5. Keluar
Pilih menu (1/2/3/4/5): 1  
Masukkan nama mahasiswa: Rafli Dhiya Fadhaly
Masukkan nilai mahasiswa: 90
Data mahasiswa berhasil ditambahkan.

Menu:
1. Tambah data mahasiswa
2. Tampilkan data mahasiswa
3. Hapus data mahasiswa
4. Ubah data mahasiswa
5. Keluar
Pilih menu (1/2/3/4/5): 2
Daftar Nilai Mahasiswa:
--------------------------
Nama: Rafli Dhiya Fadhaly, Nilai: 90.0
--------------------------

Menu:
1. Tambah data mahasiswa
2. Tampilkan data mahasiswa
3. Hapus data mahasiswa
4. Ubah data mahasiswa
5. Keluar
Pilih menu (1/2/3/4/5): 5
Terima kasih! Program selesai.
```
## Flowchart
![Draw io (2)](https://github.com/user-attachments/assets/186e197a-60e2-4412-8f46-cde81d1c34eb)

![Draw io (3)](https://github.com/user-attachments/assets/22c9be3e-c74d-4c29-b361-58df40bde208)

# Penjelasan
1. Kelas DaftarMahasiswa: Kelas ini menyimpan data siswa dalam bentuk daftar (data_mahasiswa). Setiap siswa disimpan sebagai kamus dengan dua kunci: "nama" dan "nilai".
   
   A. Metode init (self) Ini adalah metode konstruktor, yang dijalankan saat objek dari class DaftarMahasiswa dibuat. Di sini, data_mahasiswa diinisialisasi sebagai daftar kosong untuk menyimpan data mahasiswa.
   
   B. Metode tambah(self) Metode ini digunakan untuk menambahkan data siswa baru ke dalam data_mahasiswa. Ketika dipanggil, program akan meminta pengguna untuk memasukkan nama dan nilai siswa. Setelah itu, data tersebut disimpan dalam bentuk kamus ("nama": nama, "nilai": nilai}) dan ditambahkan ke dalam list data_mahasiswa.

   C. Metode tampilkan(self) Metode ini digunakan untuk menampilkan semua data siswa yang ada dalam data_mahasiswa. Jika daftar kosong, maka program akan menampilkan pesan bahwa data mahasiswa kosong. Jika ada data, program akan menampilkan setiap nama dan nilai siswa satu per satu.

   D. Metode hapus(self, nama) Metode ini digunakan untuk menghapus data siswa berdasarkan nama. Jika nama yang diberikan ditemukan dalam list, maka data siswa tersebut akan dihapus. Jika nama tidak ditemukan, maka program akan memberi tahu pengguna bahwa data siswa tersebut tidak ada.
   
   E. Metode ubah(self, nama) Metode ini digunakan untuk mengubah nilai siswa berdasarkan nama. Program akan mencari siswa yang sesuai dengan nama yang diberikan, kemudian meminta pengguna untuk memasukkan nilai baru untuk siswa tersebut. Setelah nilai baru dimasukkan, nilai siswa akan diperbarui.

2. Bagian Program Utama Pada bagian ini, sebuah objek daftar_mahasiswa dari kelas DaftarMahasiswa diinisialisasi. Program kemudian memasuki loop while True yang menampilkan menu pilihan untuk pengguna. Menu ini memungkinkan pengguna untuk:
Menambah data siswa Menampilkan data siswa Menghapus data siswa Mengubah data siswa Keluar dari program Berdasarkan pilihan yang dimasukkan oleh pengguna, program akan memanggil metode yang sesuai dari objek daftar_mahasiswa. Program terus berjalan dalam loop hingga pengguna memilih untuk keluar (pilihan '5').

3. Detail Menu Program Pilihan 1 (Tambah data siswa): Memanggil metode tambah() untuk menambahkan data siswa baru. Pilihan 2 (Menampilkan data siswa): Memanggil metode tampilkan() untuk menampilkan seluruh data siswa. Pilihan 3 (Hapus data siswa): Meminta pengguna untuk memasukkan nama siswa yang ingin dihapus, lalu memanggil metode hapus(nama). Pilihan 4 (Ubah data siswa): Meminta pengguna untuk memasukkan nama siswa yang ingin diubah, lalu memanggil metode ubah(nama). Pilihan 5 (Keluar): Keluar dari program dan menampilkan pesan terima kasih.
   
4. Validasi Input Program juga mencakup validasi input, seperti: Mengonversi input nilai siswa ke dalam tipe data float untuk memastikan bahwa nilai yang dimasukkan adalah angka. Mengabaikan perbedaan kapitalisasi huruf saat terjadi kebetulan nama siswa (menggunakan .lower()).
   
5. Penggunaan List dan Dictionary List (data_mahasiswa) digunakan untuk menyimpan semua data siswa dalam bentuk kamus. Kamus digunakan untuk menyimpan pasangan nama dan nilai untuk setiap siswa.
