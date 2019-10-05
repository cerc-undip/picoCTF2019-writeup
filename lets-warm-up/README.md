# Lets Warm Up
**Category:** general <br>
**Point:** 50

> If I told you a word started with 0x70 in hexadecimal, what would it start with in ASCII?

---

Challenge ini masih mudah, kita hanya perlu mengkonversi dari bilangan heksadesimal ke karakter ASCII. Berikut ini saya gunakan script menggunakan Python

```python
c = chr(int('0x70', 16))
print(c)
```

flag : `picoCTF{p}`