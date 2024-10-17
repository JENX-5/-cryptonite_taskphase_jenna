# Your First Shell Script
- First create a file using touch which stores the commands.
- Then write the commands into the file. You can use apps like Notepad etc.
- I decided to write commands in the file in the terminal itself. So echo your commands and redirect it to the file.
- Then run the file use bash file.sh.

```bash
hacker@chaining~your-first-shell-script:~$ touch x.sh
hacker@chaining~your-first-shell-script:~$ echo "/challenge/pwn ; /challenge/college" > x.sh
hacker@chaining~your-first-shell-script:~$ bash x.sh
Great job, you've written your first shell script! Here is the flag:
pwn.college{Q89JT6wgbhWk60QVd4-zwTx9NdJ.dFzN4QDL0gTN0czW}
```
