# Redirecting Script Output
- Like the previous challenge, store the commands in a file(here x.sh)
- Then run the file but use | to pip the output as input to /challenge.solve

```bash
hacker@chaining~redirecting-script-output:~$ echo "/challenge/pwn
> /challenge/college" > x.sh
hacker@chaining~redirecting-script-output:~$ cat x.sh
/challenge/pwn
/challenge/college
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{YKK96FpT1jLa0IyhNaehGGyH2qw.dhTM5QDL0gTN0czW}
```
