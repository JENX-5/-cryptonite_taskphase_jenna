# Matching Paths with []

```bash
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[abhs]
You got it! Here is your flag!
pwn.college{UvGFLZUlH321VWApH-Cr6QM1XmF.dRjM4QDL0gTN0czW}
```
- As instructed, we need to run /challenge/run with a single argument that bracket-globs into the absolute paths to the \
  file_b, file_a, file_s, and file_h files.
- Then to give the arguments as absolute path of the files using [], we put those characters which need to be matched \
  with the given files.
- Here the files that need to be matched are file_a,file_b, file_s, file_h. So use file_[absh]
