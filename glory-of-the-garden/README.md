# Glory of the Garden
**Category:** general <br>
**Point:** 50

> This garden contains more than it seems. You can also find the file in /problems/glory-of-the-garden_4_cf9f4aaf458caf5268f8cf0a6465eb98 on the shell server.

---

![](./garden.jpg)

Pada challenge ini kita diberikan sebuah file gambar `garden.jpg`. Ketika dibuka tidak ada keanehan apa-apa. Kuncinya adalah dengan menggunakan _command_ `strings` dan `grep`

```zsh
➜  glory-of-the-garden ✗ strings garden.jpg | grep -i pico
Here is a flag "picoCTF{more_than_m33ts_the_3y3f089EdF0}"
```


flag : `picoCTF{more_than_m33ts_the_3y3f089EdF0}`