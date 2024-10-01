```bash
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{kt4DU_GgFP3qRTWFzpItFbdI_a0.dhzN5QDL0gTN0czW}
```

```bash
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{YC_GSfQ8D42xAvCMEUR7r7kUz4M.dVDN1QDL0gTN0czW}
```
```bash
hacker@paths~position-thy-self:/$ cd /sys
hacker@paths~position-thy-self:/sys$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Iukf5oLRcCR6ZqVuQqQdb4O1Uw9.dZDN1QDL0gTN0czW}
```

```
hacker@paths~position-elsewhere:~$ cd /home
hacker@paths~position-elsewhere:/home$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{gGytZOrhIUarGpO4aoCyPVz7FfH.ddDN1QDL0gTN0czW}
```

```
hacker@paths~position-yet-elsewhere:/usr/aarch64-linux-gnu$ cd /usr/aarch64-linux-gnu/include/gnu
hacker@paths~position-yet-elsewhere:/usr/aarch64-linux-gnu/include/gnu$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{MEKHaumZcGACHjQI3ufy4Icdya-.dhDN1QDL0gTN0czW}
```
```
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{kXEDmQPPFOv6SlSUHNm5RzSp_hy.dlDN1QDL0gTN0czW}
```

```
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{cVjQko4_9C6aLZrDY0iUhtnDjal.dBTN1QDL0gTN0czW}

```
```
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{4int0EqSbzY_PB0J8exTM-PkW1V.dFTN1QDL0gTN0czW}
```
```
hacker@paths~home-sweet-home:~$ /challenge/run ~/j
Writing the file to /home/hacker/j!
... and reading it back to you:
pwn.college{0q_mOvEBlG7xezKFEN675TcAcg0.dNzM4QDL0gTN0czW}
```
