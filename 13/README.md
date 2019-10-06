# 13
**Category:** crypto <br>
**Point:** 100

> Cryptography can be easy, do you know what ROT13 is? `cvpbPGS{abg_gbb_onq_bs_n_ceboyrz}`

---

Pada judul challenge sudah diberikan clue yang cukup jelas untuk bisa menyelesaikan challenge ini, yaitu menggunakan algoritma enkripsi **ROT13** atau **Caesar** dengan putaran sebanyak 13.

Saya biasa menggunakan tools online [cryptii](https://cryptii.com/) karena terdapat banyak library kriptografi yang bisa di-_custom_ disana.

Jika menggunakan terminal bisa diselesaikan dengan command berikut.

```bash
echo 'cvpbPGS{abg_gbb_onq_bs_n_ceboyrz}' | tr 'A-Za-z' 'N-ZA-Mn-za-m
```

flag : `picoCTF{not_too_bad_of_a_problem}`