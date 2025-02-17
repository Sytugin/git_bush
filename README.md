# Работа с git и bash

## Работа с файлами и папками в bash (базовые команды)
```
  Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ pwd                        # Определяем имя папки, в которой вы находитесь
/c/Users/Олег/Documents/Bash_training

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mkdir test1                  # Создать внутри этой папки каталог с именем test1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ cd test1                     # Перейти в папку test1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ touch 1 2 3            # Создать файл 1,2 и 3 внутри каталога test1  
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ ls 1  2  3             # Проверить содержимое каталога test1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ cd ..                  # Перейти в директорию на уровень выше

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mkdir test2                  # Создать папку test2 внутри домашней директории
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ ls test2                     # Проверить содержимое каталога test2
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ rmdir test2                  # Удалить папку test2
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ rm test1/2             # Удалить файл 2 из папки test1
             
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ cd ..                  # Создать папку в домашней директории test3 и добавить в нее два файла
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mkdir test3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ cd test3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ touch file_1 file_2

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ cd ..                  
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ rm -rf test3                 # Удалить папку test3

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mkdir test4                  # Создать папку test4 в домашней директории

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mv test1/1 test4             # Переместить файлы 1 и 3 из папки test1 в папку test4 
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mv test1/3 test4
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ ls test1
               
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test1 $ cd ..                  # Добавить в файл 1 три строки со словами line
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ cd test4
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line > 1

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ cat 1 line
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line >> 1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line >> 1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ cat 1                  # Посмотреть содержимое файла 1


Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line > 3          # Добавить в файл 3 три строки со словами line
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line >> 3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ echo line >> 3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ cat 3                  # Посмотреть содержимое файла 3


Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ cat 1 3                # Просмотрите содержимое двух файлов (1 и 3) сразу

                                                                                      # Используя один из редакторов, заменить все строки в файле 1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ cat 1                  # Посмотреть содержимое файла 1
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test4 $ less 1                 # Открыть файл программой для просмотра текстовых файлов 

```
