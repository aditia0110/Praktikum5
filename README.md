# Praktikum5
# Latihan membuat list, menambahkan, mengedit, mengambil elemen pads list di python.

## Repository ini dibuat untuk memenuhi Tugas Mata Kuliah Bahasa Pemrograman

1. Pertama-tama buatlah folder pada `Praktikum5` dan didalamnya diisi file `list.py` & `Praktikum5.py` seperti gambar berikut :

<img width="170" alt="image" src="https://user-images.githubusercontent.com/115475348/202884479-b74f0c67-6a31-4f6c-8a8d-3708facf7e9e.png">


2. Langkah selanjutnya buka file `List.py` lalu input seperti berikut ini :

            # membuat 5 list dengan type data yang berbeda

            listData = ["Teknik Informatika", "UPB", 650000, True, "Fakultas Teknik"]

            ###########################
            # mengakses element list #
            #########################

            # menampilkan element ke-3 pada sebuah list
            print(listData[2])

            # menampilkan elemen ke-2 sampai ke-4
            print(listData[1:4])

            # menampilkan elemen terakhir
            print(listData[4])
            # atau bisa juga seperti ini
            print(listData[-1])

            ##########################
            # Mengubah element list #
            ########################

            # Merubah elemen ke-4 dengan nilai lain
            listData[3] = False
            print(listData)

            # Merubah elemen ke-4 sampai dengan terakhir degan nilai lain
            listData[3:5] = [True, "TI22B1"]
            print(listData)

            ##########################
            # Menambah element list #
            ########################

            # membuat listA dan diisi oleh element yang ada di listData
            listA = listData

            # membuat list B dengan element masih kosong
            listB = []

            # mengambil 2 nilai dari listA lalu simpan ke listB
            listB = listA[0:2]
            print(listB)

            # Menambahkan list B dengan nilai string
            listB.append("Fakultas Teknik")
            print(listB)

            # Menambahkan list B dengan 3 nilai
            listB.extend(["Teknik Sipil", "Teknik Lingkungan", "Teknik Industri"])
            print(listB)

            # Menggabungkan list B dengan listA
            listGabungan = listA + listB
            print(listGabungan)
            
 <img width="289" alt="image" src="https://user-images.githubusercontent.com/115475348/202884927-38ede1b9-24d3-4088-a48a-660946952cdf.png">


3. Langkah selanjutnya jalankan file, dan hasilnya seperti berikut ini :

<img width="770" alt="hasil list" src="https://user-images.githubusercontent.com/115475348/202885019-1bbb3d00-035b-40ac-9034-030091b9ccd7.png">

## Membuat program input data mahasiswa beserta nilai dan disimpan didalam List. 

Berikut ini adalah Flowchart program yang akan kita buat :

![image](https://user-images.githubusercontent.com/115475348/202885090-3b532af7-402c-4a16-b71b-ffb018f0e9e6.png)

1. Buka file `Praktikum5.py` dan input seperti berikut ini :

            # import package tabulate
            from tabulate import tabulate

            # membuat list kosong untuk menampung data
            dataMahasiswa = []
            no = 0
            # melakukan perulangan input sesuai keinginan sampai pertanyaan tambah data dimunculkan kembali
            while(True):
            # membuat variable untuk menampung inputan
            no += 1
            nama = input("Masukan Nama : ")
            nim = input("Masukan NIM : ")
            kelas = input("Masukan Kelas : ")
            matkul = input("Masukan Mata Kuliah : ")

            # mengkonversi string ke integer
            tugas = int(input("Masukan Nilai Tugas : "))
            uts = int(input("Masukan Nilai UTS : "))
            uas = int(input("Masukan Nilai UAS : "))

            # menjumlahkan nilai dari tugas,uts dan uas
            nilai_akhir = (tugas * 30 / 100) + (uts * 35 / 100) + (uas * 35 / 100)

            # lakukan pengecekan jika nilai_akhir lebih besar dari 50 maka Lulus selain itu tidak lulus dan mengulang mata kuliah
            if (nilai_akhir > 50):
                  keterangan = "Lulus"
            else:
                  keterangan = "Tidak Lulus, Mengulang Mata kuliah"
            # menambahkan data input ke list dataMahasiswa
            dataMahasiswa.append(
                  [no, nama, nim, kelas, matkul, tugas, uts, uas, nilai_akhir, keterangan])

            # input tambah data jika tekan y maka input kembali, selain itu berhenti dan tampilkan data
            tambah_data_lagi = input("Tambah Data lagi ? (y/t) : ")
            if(tambah_data_lagi == "t"):
                  break

            # tampilkan dataMahasiswa menggunakan tabulate package agar tampilan berbentuk table
            print(tabulate(dataMahasiswa, headers=[
                  "No", "Nama", "Nim", "Kelas", "Mata Kuliah", "Tugas", "UTS", "UAS", "Nilai Akhir", "Keterangan"], tablefmt="fancy_grid"))

<img width="632" alt="image" src="https://user-images.githubusercontent.com/115475348/202885291-6853f50a-c482-434d-acb6-2f39e4634528.png">

2. Langkah selanjutnya jalankan file, dan hasilnya seperti berikut ini :

<img width="767" alt="hasil akhir praktikum 5" src="https://user-images.githubusercontent.com/115475348/202885346-aaa6c115-b996-4237-8259-70d6429c04bf.png">

Demikianlah sedikit penjelasan dari saya, kurang lebihnya mohon maaf

Terimakasih








