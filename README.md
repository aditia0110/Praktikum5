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
