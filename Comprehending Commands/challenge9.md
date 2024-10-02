# Challenge 9: An Epic File System Quest
```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
TIP  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin  challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat TIP
Tubular find!
The next clue is in: /usr/share/racket/pkgs/distributed-places-doc/scribblings/distributed-places

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ ls -a /usr/share/racket/pkgs/distributed-places-doc/scribblings/distributed-places
.  ..  .BRIEF  compiled  distributed-places.scrbl  info.rkt  rmpi.scrbl
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/share/racket/pkgs/distributed-places-doc/scribblings/distributed-places/.BRIEF
Great sleuthing!
The next clue is in: /usr/lib/R/library/splines/R

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/R/library/splines/R
hacker@commands~an-epic-filesystem-quest:/usr/lib/R/library/splines/R$ ls -a
.  ..  .INFO  splines  splines.rdb  splines.rdx
hacker@commands~an-epic-filesystem-quest:/usr/lib/R/library/splines/R$ cat .INFO
Tubular find!
The next clue is in: /opt/rappel/.git/objects/f7

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/R/library/splines/R$ ls -a /opt/rappel/.git/objects/f7
.  ..  9809bcb70ce88c1f9f355970e01c23f6116353  NOTE-TRAPPED
hacker@commands~an-epic-filesystem-quest:/usr/lib/R/library/splines/R$ cat /opt/rappel/.git/objects/f7/NOTE-TRAPPED
Great sleuthing!
The next clue is in: /usr/local/share/doc/networkx-3.1/examples/3d_drawing/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/lib/R/library/splines/R$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls -a  /usr/local/share/doc/networkx-3.1/examples/3d_drawing/__pycache__
.  ..  BLUEPRINT  mayavi2_spring.cpython-38.pyc  plot_basic.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/$ cat  /usr/local/share/doc/networkx-3.1/examples/3d_drawing/__pycache__/BLUEP
RINT
Lucky listing!
The next clue is in: /opt/radare2/shlr/capstone/msvc/test_arm

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/$ ls /opt/radare2/shlr/capstone/msvc/test_arm
NUGGET-TRAPPED  test_arm.vcxproj
hacker@commands~an-epic-filesystem-quest:/$ cat /opt/radare2/shlr/capstone/msvc/test_arm/NUGGET-TRAPPED
Lucky listing!
The next clue is in: /usr/lib/R/library/translations/fr/LC_MESSAGES
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/lib/R/library/translations/fr/LC_MESSAGES
hacker@commands~an-epic-filesystem-quest:/usr/lib/R/library/translations/fr/LC_MESSAGES$ ls -a
.        R-base.mo       R-graphics.mo  R-parallel.mo  R-stats4.mo  R-utils.mo  grDevices.mo  methods.mo   stats.mo
..       R-compiler.mo   R-grid.mo      R-splines.mo   R-tcltk.mo   R.mo        graphics.mo   parallel.mo  tcltk.mo
INSIGHT  R-grDevices.mo  R-methods.mo   R-stats.mo     R-tools.mo   RGui.mo     grid.mo       splines.mo   tools.mo
hacker@commands~an-epic-filesystem-quest:/usr/lib/R/library/translations/fr/LC_MESSAGES$ cat INSIGHT
Great sleuthing!
The next clue is in: /usr/share/nvim/runtime/autoload/dist

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/R/library/translations/fr/LC_MESSAGES$ cd  /usr/share/nvim/runtime/autoload/dist
hacker@commands~an-epic-filesystem-quest:/usr/share/nvim/runtime/autoload/dist$ ls
POINTER  ft.vim
hacker@commands~an-epic-filesystem-quest:/usr/share/nvim/runtime/autoload/dist$ cat POINTER
Yahaha, you found me!
The next clue is in: /usr/share/rubygems-integration/all/specifications

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/nvim/runtime/autoload/dist$ cd /usr/share/rubygems-integration/all/specifications
hacker@commands~an-epic-filesystem-quest:/usr/share/rubygems-integration/all/specifications$ ls
README                   net-telnet-0.1.1.gemspec    rake-13.0.1.gemspec      xmlrpc-0.3.0.gemspec
minitest-5.13.0.gemspec  power_assert-1.1.7.gemspec  test-unit-3.3.5.gemspec

hacker@commands~an-epic-filesystem-quest:/usr/share/rubygems-integration/all/specifications$ cat README
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{AnVgcIctpbmmXONKvqi-pMKr-3h.dljM4QDL0gTN0czW}
```
- First use 'ls' to get the list of all the files in the directory.
- Then use cat to read the contents either by first changing the directory using cd or directly giving cat absolute path.
- If the file begins with '.' the use 'ls -a \[directory\]' to find the file.

### References
- None
