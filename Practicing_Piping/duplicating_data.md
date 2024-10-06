# Duplicating Piped data With Tee

- To find the secret code we need to find the right input for the /challenge/college
- Using tee pwn it stores the ouput in pwn file.
- Reading the contents using cat, we figure the secret code.
- Now using /challenge/pwn with the secret code and pip it to /challenge/college for the flag.
  
```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee pwn |/challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.

hacker@piping~duplicating-piped-data-with-tee:~$ cat pwn
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "IV3omMGq"

hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret "IV3omMGq" | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{IV3omMGqCS7nTmC3-lXZp0Bsskg.dFjM5QDL0gTN0czW}
```

