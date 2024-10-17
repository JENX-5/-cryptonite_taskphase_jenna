# Executable Shell Scripts
- Store the commands in a file called script.sh .
- Then change its permissions so that the file can be executed.
- Finally, run the file.
```bash
hacker@chaining~executable-shell-scripts:~$ echo "/challenge/solve" > script.sh
hacker@chaining~executable-shell-scripts:~$ ls -l script.sh
-rw-r--r-- 1 hacker hacker 17 Oct 17 05:43 script.sh
hacker@chaining~executable-shell-scripts:~$ chmod ugo+x ~/script.sh
hacker@chaining~executable-shell-scripts:~$ ./script.sh
Congratulations on your shell script execution! Your flag:
pwn.college{sN_kGXJnSt2Qpxvdr6_uGFfJsY0.dRzNyUDL0gTN0czW}
```
