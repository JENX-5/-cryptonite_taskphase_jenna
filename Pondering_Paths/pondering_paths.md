# PONDERING PATHS
<p>&nbsp;</p>

## Challenge 1: The Root
```bash
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{kt4DU_GgFP3qRTWFzpItFbdI_a0.dhzN5QDL0gTN0czW}
```
- Absolute path uses the root directory as the starting directory 
- Begins with / and then name of directory

## Challenge 2: Program and Absolute Paths
```bash
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{YC_GSfQ8D42xAvCMEUR7r7kUz4M.dVDN1QDL0gTN0czW}
```
- Since the run file is stored in directory challenge: ./challenge/run will run the file

## Challenge 3: Position Thy Self
```bash
hacker@paths~position-thy-self:/$ cd /sys
hacker@paths~position-thy-self:/sys$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Iukf5oLRcCR6ZqVuQqQdb4O1Uw9.dZDN1QDL0gTN0czW}
```
- Change the directory to the directory in which challenge is stored(i.e sys).
- Then run the program like before

## Challenge 4: Position Elsewhere
```bash
hacker@paths~position-elsewhere:~$ cd /home
hacker@paths~position-elsewhere:/home$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{gGytZOrhIUarGpO4aoCyPVz7FfH.ddDN1QDL0gTN0czW}
```
- Same Logic used before

## Challenge 5: Position yet elsewhere
```bash
hacker@paths~position-yet-elsewhere:/usr/aarch64-linux-gnu$ cd /usr/aarch64-linux-gnu/include/gnu
hacker@paths~position-yet-elsewhere:/usr/aarch64-linux-gnu/include/gnu$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{MEKHaumZcGACHjQI3ufy4Icdya-.dhDN1QDL0gTN0czW}
```
- First use absolute path to change the directory then get the flag

## Challenge 6: Implicitive Relative Paths, from /
```bash
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{kXEDmQPPFOv6SlSUHNm5RzSp_hy.dlDN1QDL0gTN0czW}
```
- Use cd /  to get in the main directory, then get the flag like usual.

## Challenge 7: Explicit Relative Paths, from /
```bash
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{cVjQko4_9C6aLZrDY0iUhtnDjal.dBTN1QDL0gTN0czW}
```
- ./ and ../ are relative paths with respect to the current working directory.
- Since 'challenge/run' is in currect directory we use ./

## Challenge 8: Implicit Relative Path
```bash
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{4int0EqSbzY_PB0J8exTM-PkW1V.dFTN1QDL0gTN0czW}
```
- Change the directory to 'challenge' and then run the program.
- Since we are using relative path and run is in the current directory ./run works.

## Challenge 9: Home Sweet Home
```bash
hacker@paths~home-sweet-home:~$ /challenge/run ~/j
Writing the file to /home/hacker/j!
... and reading it back to you:
pwn.college{0q_mOvEBlG7xezKFEN675TcAcg0.dNzM4QDL0gTN0czW}
```
- In this challenge /challenge/run would take the argument you give and write the flag into it.
- Since the argument had to be absolute path and less than three characters. ~ is used since it basically expands to /home/hacker.
- The last argument can be any letter and the flag will be written in it.

## References
-[PWN COLLEGE](https://pwn.college/linux-luminarium/paths/)
