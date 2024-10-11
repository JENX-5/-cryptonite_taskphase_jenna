# Executable Files
- From ls -l we notice that file is owned by the user(i.e. hacker).
- So we change the permission so that the file can be executed by the user.
- Use chmod u+x and the permissions will change. Now the user can execute the program.
```bash
hacker@permissions~executable-files:~$ ls -l /challenge/run
-r--r--r-- 1 hacker hacker 32 Jul  4 06:37 /challenge/run
hacker@permissions~executable-files:~$ chmod u+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{ITV5Di4_5qjEqOBzeNi7V6c58vE.dJTM2QDL0gTN0czW}
```
