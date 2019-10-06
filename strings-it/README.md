# strings it
**Category:** general <br>
**Point:** 100

> Can you find the flag in file without running it? You can also find the file in /problems/strings-it_1_7a67382a38fc00751a6b9b29b0872813 on the shell server.

---

Diberikan sebuah file bernama `strings` dengan format

```
ELF 64-bit LSB shared object x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/l, for GNU/Linux 3.2.0, BuildID[sha1]=48e55d3ef2891ca5b5a242ee99ad297a281e70d5, not stripped
```

Judul dan deskripsi menunjukkan clue yang cukup jelas, kita tidak perlu menjalankan program tersebut namun cukup melihat isi string-nya saja.

Gunakan tools bawaan terminal yaitu `strings` dan `grep` untuk mencari string yang diinginkan

```zsh
➜ strings-it ✗ strings ./strings | grep -i pico
picoCTF{5tRIng5_1T_c7fff9e5}
```

### exploit
* shell : [exploit.sh](./exploit.sh)

flag : `picoCTF{5tRIng5_1T_c7fff9e5}`