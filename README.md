# HW_Terminal

**Посмотреть где я;**
```Bash
pwd
```
**Создать папку;**
```Bash
mkdir HW_P1
```
**Зайти в папку;**
```Bash
cd HW_P1
```
**Создать 3 папки;**
```Bash
mkdir dir_1 dir_2 dir_3
```
**Зайти в любоую папку;**
```Bash
cd dir_3
```
**Создать 5 файлов (3 txt, 2 json);**
```Bash
touch thefirst.txt thesecond.txt thethird.txt first.json second.json
```
**Создать 3 папки;**
```Bash
mkdir thefirst thesecon thethird
```
**Вывести список содержимого папки;**
```Bash
ls -la
```
**Открыть любой txt файл;**
```Bash
vim thefirst.txt
```
**Написать туда что-нибудь, любой текст;**
```Bash
i --> "enter the text"
```
**Сохранить и выйти;**
```Bash
ESC --> ":wq"
```
**Выйти из папки на уровень выше;**
```Bash
cd ../
```
**Переместить любые 2 файла, которые вы создали, в любую другую папку;**
```Bash
mv first.json second.json ../dir_2
```
**Скопировать любые 2 файла, которые вы создали, в любую другую папку;**
```Bash
cp first.json second.json ../dir_1
```
**Найти файл по имени;**
```Bash
find . -name “thefirst.txt”
```
**Просмотреть содержимое в реальном времени;**
```Bash
tail thefirst.txt
```
**Вывести несколько первых строк из текстового файла;**
```Bash
head -3 thefirst.txt
```
**Вывести несколько последних строк из текстового файла;**
```Bash
tail -3 thefirst.txt
```
**Просмотреть содержимое длинного файла;**
```Bash
less thefirst.txt
```
**Вывести дату и время;**
```Bash
date
```

**Задание #***

**Отправить http запрос на сервер:**
***http://162.55.220.72:5005/terminal-hw-request***
```Bash
curl http://162.55.220.72:5005/terminal-hw-request
curl -I http://162.55.220.72:5005/terminal-hw-request
```
**Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13**
```Bash
#!/bin/bash
cd ../../
cd HW_P1
cd dir_2
mkdir dir_1 dir_2 dir_3
cd dir_1
pwd
touch first.txt second.txt third.txt thefirst.json thesecond.json
mkdir first second third
ls -la
mv first.txt second.txt ./dir_2
mv first.txt second.txt ../dir_2
mv first.txt second.txt dir_2

in the terminal enter this command:

./myscript
```