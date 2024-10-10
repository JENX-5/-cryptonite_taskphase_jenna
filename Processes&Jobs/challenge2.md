# Killing Processes
- We are using some previous concepts of piping |. Using the output as input to a command.
- To find /challenge/dont_run we use the grep function that will search through the output of ps -e.
- For some reason 'ps -e' didn't work or give the needed output(Kinda Confused why it didn't) so used 'ps -ef'.
- Then kill the process using kill pid(Process ID) and run /challenge/run


```bash
hacker@processes~killing-processes:~$ ps -e | grep /challenge/dont_run
hacker@processes~killing-processes:~$ ps -ef | grep /challenge/dont_run
hacker        73      71  0 17:29 ?        00:00:00 /challenge/dont_run
hacker       116      92  0 17:31 pts/1    00:00:00 grep --color=auto /challenge/dont_run
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{QaDExZQFQSnBmGN3JqBZVGMWT9e.dJDN4QDL0gTN0czW}
```
