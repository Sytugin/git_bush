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
##Поиск и редактирование файлов, работа с процессами, проверка доступности сервера, передача данных на сервер в bash:
```
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ mkdir test3                    # Создать папку test 3

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ cd test3

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 1 > 4.txt       # Добавить в папку test 3 три файла 4, 5 и 6, в каждом из которых должно быть по 4 строки row1, row2, row3, row4
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 2 >> 4.txt
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 3 >> 4.txt
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 4 >> 4.txt
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 1 >> 5.txt
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 2 >> 5.txt
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 3 >> 5.txt
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 4 >> 5.txt
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 1 >> 6.txt
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 2 >> 6.txt
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 3 >> 6.txt
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo row 4 >> 6.txt

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ grep -ir "row2" 5.txt                         # Найти строку row2 в файле 5
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ grep -ir "row" test3                                # Найти строку row в папке test3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ grep -c "^row*" 6.txt 4                       # Посчитать сколько строк с содержимым row в файле 6
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ find test3 -name "5*" test3/5.txt                   # Найти файл 5 внутри папки test3
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ find test3 -name "5*" -exec rm {} +                 # Используя команду find, удалить файл 5

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo test > 4.txt                             # Используя команду echo, добавить слово test в файл 4 
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo fail > 4.txt                             # Заменить слово test в файле 4 на fail
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training/test3 $ echo test >> 4.txt                            # Добавить в файл 4 слово test так, чтобы сохранилось содержимое

Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ tasklist                                            # Просмотреть все процессы для юзеров не только в консоли, которые происходят в системе
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ kill 666                                            # Убить процесс 666 в консоли
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ ping rusau.net                                      # Узнать доступность ресурса rusau.net, используя ping
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ ping -n 5 rusau.net                                 # Отправить 5 пакетов на сайт rusau.net
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $
curl https://petstore.swagger.io/v2/pet/findByStatus?status=sold                                             # Используя GET и команду curl, получить информацию о зарегистрированных питомцах с любым статусом на https://petstore.swagger.io/
                                                                                                             # Используя POST и команду curl, создать нового пользователя 
Oleg@DESKTOP-HF693OU MINGW64 ~/Documents/Bash_training $ $ curl -X POST -H "Content-Type=application/json" -d '{"id=555", "username=one", "firstName=two", "lastName=free", "email=four", "password=five", "phone=5", "userStatus=1"}' https://petstore.swagger.io/user
```
