# Process Exit Codes
- To get the exit code in which program terminated with, we first obviously need to run it.
- Then get the code using $?, here we used echo to output the exit code value.
- Then use the given exit code as an argument for /challenge/submit-code.
  
```bash
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
221
hacker@processes~process-exit-codes:~$ /challenge/submit-code 221
CORRECT! Here is your flag:
pwn.college{ku3-WYJcGajFD46uCTwO21oQfVy.dljN4UDL0gTN0czW}
```
