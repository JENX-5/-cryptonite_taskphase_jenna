# Resuming Processes
- As the challenge stated, run the programs run, suspend it and run from where you suspended it.
- To suspend the program use Ctrl-Z.
- Then, use fg <program_name> to resume the process.

```bash
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg /challenge/run
/challenge/run
I'm back! Here's your flag:
pwn.college{oJY3x8L3SQFngFKDSI7CO2Z2vWs.dZDN4QDL0gTN0czW}
Don't forget to press Enter to quit me!

Goodbye!
```
