# Lab 2

## Operator pada Python
Operator adalah simbol khusus pada Python yang merupakan perhitungan aritmatika atau logika.
Nilai yang dioperasikan operator disebut operand.

## Òperator Aritmatika Seperti:
•	Operator Simbol 1 Penjumlahan + 2 Pengurangan - 3 Perkalian * 4 Pembagian / 5 Sisa bagi % 6 Pemangkatan **

## Tampilan Syntax Yang Salah:
•	a=input("masukkan nilai a:")
•	b=input("masukkan nilai b:")
•	print("variable a=" ,a)
•	print("variable b=" ,b)
•	print("hasil penggabungan {1}&{0}=%d" .format(a,b) %(a+b))
•	a=int(a)
•	b=int(b)
•	print("hasil penjumlahan {1}+{0}=%d" .format(a,b) %(a+b))
•	print("hasil pembagian {1}/{0}=%f" .format(a,b) %(a/b))

## Tampilan Syntax Yang Benar:
•	a=input("masukkan nilai a:")
•	b=input("masukkan nilai b:")
•	print("variable a=" ,a)
•	print("variable b=" ,b)
•	print("hasil penggabungan {0}&{1}=%s" .format(a,b) %(a+b))
•	a=int(a)
•	b=int(b)
•	print("hasil penjumlahan {0}+{1}=%d" .format(a,b) %(a+b))
•	print("hasil pembagian {0}/{1}=%d" .format(a,b) %(a/b))

## Kenapa Bisa Salah?
1.	"d" adalah fungsi untuk bilangan bulat desimal sedangkan "s" adalah fungsi untuk Konversi string, seperti ini: str () sebelum memformat.
2.	{1}&{0}=%s Seharusnya adalah {0}&{1}=%s. Karna jika {1}&{0}=%s hasilnya akan terbalik jadi variable b lebih dulu lalu variable a. Berbeda dengan {0}&{1}=%s variable a lebih dulu, baru variable b. {0} adalah variable a, {1} adalah variable b.

## Langkah-langkah Mengoprasikanya
1.	a=input("Masukkan nilai a: ")
2.	b=input("Masukkan nilai b: ") urutan yang pertama dan kedua ini untuk: meminta kita memasukkan nilai kepada variable a dan b.
3.	print("Variable a= ", a)
4.	print("Variable b= ", b) Lalu kita akan menuliskan ulang nilai yang telah kita masukkan tadi di langkah pertama.
5.	print("Hasil penggabungan {1}&{0}=%d".format(a,b) %(a+b)) Syntax ini akan menggabungkan variable a dan b, tetapi pada tahap ini akan terjadi error karena tipe data pada variable adalah string sedangkan yang diminta adalah nomor atau integer, maka kita harus mengubah '%d' menjadi '%s' agar sistem membacanya sebagai string bukan integer. Lalu karena {1} adalah variable b dan {0} adalah variable a (b, a), maka diubah menjadi {0}&{1} agar tidak terbalik dan sesuai dengan format yang akan digabungkan.
6.	a=int(a)
7.	b=int(b) Lalu di urutan 6 dan 7 akan mengkonversikan tipe data variable a dan b, dari yang tadinya str menjadi int.
8.	print("Hasil penjumlahan {1}+{0}=%d".format(a,b) %(a+b)) pada langkah ini, akan menjumlahkan nilai variable a dan b, dan sebaiknya {1}+{0} diubah menjadi {0}+{1}
9.	print("Hasil pembagian {1}/{0}=%d".format(a,b) %(a/b)) Dan yang terakhir, melakukan pembagian nilai variable a dengan b, ubah {1}/{0} menjadi {0}/{1} agar nilai yang dibagi sesuai dengan hasilnya. Gunakan '%d' atau '%s' apabila hasilnya adalah angka desimal.
