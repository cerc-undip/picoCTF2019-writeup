# First Grep
**Category:** general <br>
**Point:** 100

> Can you find the flag in file? This would be really tedious to look through manually, something tells me there is a better way. You can also find the file in /problems/first-grep_1_6788154ca7ee937f569985ff397203b6 on the shell server.

---

Diberikan sebuah file dengan format `ASCII text, with very long lines` yang mana di dalam file ini berisikan teks yang sangat panjang dan acak. Judul telah memberikan clue bahwa kita perlu melakukan `grep` terhadap file ini.

Dengan grep memudahkan kita untuk mencari kata-kata yang ingin dicari, sama seperti fitur search pada dokumen namun dilakukan pada terminal.

```sh
➜  first-grep ✗ cat file | grep -i pico
picoCTF{grep_is_good_to_find_things_4b2451ea}
```

exploit : [exploit.sh](./exploit.sh)

flag : `picoCTF{grep_is_good_to_find_things_4b2451ea}`