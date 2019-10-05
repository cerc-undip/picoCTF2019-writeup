# Lets Warm Up
**Category:** crypto <br>
**Point:** 50

> The numbers... what do they mean?

---

![](./the_numbers.png)

Disini kita diberikan sebuah file gambar yang terdapat deretan angka beserta tanda `{` dan `}` yang menandakan bahwa angka-angka ini akan membentuk flag.

Jika dilihat dari format flag `picoCTF{......}` dapat diketahui bahwa setiap angka merepresentasikan urutan huruf dalam alfabet. Untuk menyelesaikannya saya menggunakan Python

```python
data = [16, 9, 3, 15, 3, 20, 6, 20, 8, 5, 14, 21, 13, 2, 5, 18, 19, 13, 1, 19, 15, 14]

for c in data:
  print(chr(c + 64) , end='')
```

flag : `PICOCTF{THENUMBERSMASON}`