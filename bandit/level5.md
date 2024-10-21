# LEVEL 5

# Description
The password for the next level is stored in a file somewhere under the inhere directory 
and has all of the following properties:
human-readable
1033 bytes in size
not executable


# SOLUTION
- Using find with its options. Refer man find for details.
```bash
bandit5@bandit:~/inhere$ find -type f -size 1033c ! -executable
./maybehere07/.file2
bandit5@bandit:~/inhere$ cat ./maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```
