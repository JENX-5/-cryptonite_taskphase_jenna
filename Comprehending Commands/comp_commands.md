# Comprehending Commands

## Challenge 1: cat
```bash
hacker@commands~cat-not-the-pet-but-the-command:~$ cat flag
pwn.college{0A_7Aid3AvGsMqe4fbzsx2Vt0_j.dFzN1QDL0gTN0czW}
```
- Since the 'flag' file is in the current home directory. Use cat command to read it

## Challenge 2: Catting Absolute Paths
``` bash
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{IW8G7nmgjoLdaqd-W_6C5d-vsNP.dlTM5QDL0gTN0czW}
```
- Here we just read the contents by giving the absolute path of the file i.e. /flag

## Challenge 3: More catting Practice
``` bash
Connected!
You cannot use the 'cd' command in this level, and must retrieve the flag by
absolute path. Plus, I hid the flag in a different directory! You can find it
in the file /usr/lib/pkgconfig/flag. Go cat it out **without** cding into that
directory!
hacker@commands~more-catting-practice:~$ cat /usr/lib/pkgconfig/flag
pwn.college{8_bwSJvoISl5BAaukCyBjRja6e3.dBjM5QDL0gTN0czW}
```
- Same logic as above, just the directory changed.

## Challenge 4: grepping for a needle in a haystack
```bash
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{MBZAaEusZT4VJ--lhV3E3MHcBmi.ddTM4QDL0gTN0czW}
```
## Challenge 5: Listing Files
```bash
hacker@commands~listing-files:~$ ls /challenge
27802-renamed-run-6901  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/27802-renamed-run-6901
Yahaha, you found me! Here is your flag:
pwn.college{IMPE55WpRRmSF0xk4nGcaLZzZmh.dhjM4QDL0gTN0czW}
```

## Challenge 6: Touching Files
```bash
hacker@commands~touching-files:/$ cd tmp
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.MiOQGWw5Zc
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{Y0YIgEuMWuBi-szzJwoUQS13wMX.dBzM4QDL0gTN0czW}
```
## Challenge 7: Removing Files
```bash
hacker@commands~removing-files:~$ ls
Desktop  delete_me  j
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ ls
Desktop  j
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{8hAijCG33_lFf41Z9hlaPkMm4pZ.dZTOwUDL0gTN0czW}
```
## Challenge 8: Hidden Files
```bash
hacker@commands~hidden-files:~$ ls -a /
.                      bin        etc    lib64   nix   run   tmp
..                     boot       home   libx32  opt   sbin  usr
.dockerenv             challenge  lib    media   proc  srv   var
.flag-146782335826902  dev        lib32  mnt     root  sys
hacker@commands~hidden-files:~$ /.flag-146782335826902
ssh-entrypoint: /.flag-146782335826902: Permission denied
hacker@commands~hidden-files:~$ cat /.flag-146782335826902
pwn.college{ktDm3goSkCtPdeRh0i5Nfn9y-xE.dBTN4QDL0gTN0czW}
```

