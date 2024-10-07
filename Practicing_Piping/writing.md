# Writing to Multiple Programs
## Challenge 10:-
- OK SO, we need to redirect the output of /challenge/hack to two different commands.
- First get the output from /challenge/hack and use it as input using |
- Then use >(command1) >(command2) to redirect the output to those two.
```bash
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
12838303471726632395
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{InmKrNrF20VKtUCGF1sOABU3KRU.dBDO0UDL0gTN0czW}
```
## References
[STACK EXCHANGE](https://unix.stackexchange.com/questions/28503/how-can-i-send-stdout-to-multiple-commands)
