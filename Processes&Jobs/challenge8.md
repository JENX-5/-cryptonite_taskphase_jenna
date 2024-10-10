# Starting Background Processes
- Instead of suspending a program to run it in the background, we can do it by appending & at the end of the command.
- This will start the program run in the background itself.

```bash
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &
[1] 99



Yay, you started me in the background! Because of that, this text will probably
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{8eKKiuhXYFpPIs7Wds84fWxCQcm.dlDN4QDL0gTN0czW}
[1]+  Done                    /challenge/run
```
