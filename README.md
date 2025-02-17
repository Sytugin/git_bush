# Работа с git и bash

## Работа с файлами и папками в bash (базовые команды)
```
  Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ pwd
/c/Users/Олег/Documents/Bash_training

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mkdir test1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ cd test1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ touch 1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ touch 2

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ touch 3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ ls 1  2  3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ cd ..
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mkdir test2

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ ls test1/  test2/
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ rmdir test2
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ ls test1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ cd test1

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ rm 2
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ ls 1  3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ cd ..
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mkdir test3

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ cd test3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ touch file_1 file_2
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ cd ..
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ rm -rf test3

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mkdir test4
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mv test1/1 test4
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mv test1/3 test4
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ ls test1

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ ls test4 1  3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ cd ..
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ cd test4
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line > 1

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ cat 1 line
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line >> 1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line >> 1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ cat 1
line
line
line

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line > 3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line >> 3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line >> 3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ cat 3
line
line
line

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ cat 1 3
line
line
line
line
line
line
```
