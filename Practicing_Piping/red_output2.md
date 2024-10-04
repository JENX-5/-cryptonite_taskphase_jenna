# Challenge 2: Redirecting more output
- To get the output we need to execute it.
- But we need to redirect the output to another file, so we use >.
- Therefore the output of /challenge/run will be saved in myflag.
- Then using cat, read the contents of myflag.
```bash
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.

hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{AtP_jaCb5UtwlqtjjBMYLENfalF.dVjN1QDL0gTN0czW}
```
