# unzip
**Category:** forensic <br>
**Point:** 50

> Can you unzip this file and get the flag?

---

Di challenge ini kita diberikan sebuah file berekstensi `.zip`. Untuk menyelesaikannya kita cukup  melakukan ekstraksi file ini, bisa  dilakukan dengan menggunakan terminal maupun aplikasi extractor lainnya.

```
➜  unzip ✗ unzip flag.zip 
Archive:  flag.zip
  inflating: flag.png                
➜  unzip ✗ ls
flag.png flag.zip
➜  unzip ✗ open ./flag.png 
➜  unzip ✗
```

![](./flag.png)

flag : `picoCTF{unz1pp1ng_1s_3a5y}`