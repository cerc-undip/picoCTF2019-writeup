# Bases
**Category:** general <br>
**Point:** 100

> What does this bDNhcm5fdGgzX3IwcDM1 mean? I think it has something to do with bases.

---

Clue pada judul adalah **bases**, maka ada kaitannya dengan Base64, Base32, Base16, dkk. Kita perlu tahu dulu bentuk umum dari hasil encoding ini, bisa baca-baca [disini](https://tools.ietf.org/html/rfc4648).

String `bDNhcm5fdGgzX3IwcDM1` merupakan bentuk encoding dari **Base64**. Untuk melakukan decoding, kita bisa menggunakan tools online [cryptii](https://cryptii.com) atau menggunakan tools di terminal.

```sh
➜  bases ✗ echo bDNhcm5fdGgzX3IwcDM1 | base64 -D
l3arn_th3_r0p35
```

flag : `picoCTF{l3arn_th3_r0p35}`