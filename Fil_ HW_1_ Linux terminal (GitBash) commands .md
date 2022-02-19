Первое ДЗ 
Linux terminal (GitBash) commands 

1) Посмотреть где я ===== $ pwd 
2) Создать папку =====    $ mkdir git
3) Зайти в папку =====    $ cd git
4) Создать 3 папки =====  $ mkdir folder_1 folder_2 folder_3
5) Зайти в любую папку ====  $ cd folder_1
6) Создать 5 файлов (3 txt, 2 json)=====  $ touch git file_1.txt file_2.txt file_3.txt j_file_1.json j_file_2.json
7) Создать 3 папки =====    $ mkdir  folder1 folder2 folder3
8) Вывести список содержимого папки ==== $ ls        (список без даты изменения)
										                     $ ls -l     (список с датой, но без скрытых файлов)
										                     $ ls -la    (список с датой и скрытыми папками/файлами)
9) Открыть любой txt файл =====    $ vim file1.txt
10) Написать туда что-нибудь, любой текст. === i (write a text)
11) Сохранить и выйти. =====    to quit press Esc, :, wq ("write" "quit")
12) Выйти из папки на уровень выше ===== $ cd ..
—
13) переместить любые 2 файла, которые вы создали, в любую другую папку. ===== $ mv file1.txt file2.txt /c/users/user/git
14) скопировать любые 2 файла, которые вы создали, в любую другую папку. ===== $ cp file1.txt file2.txt /d/QA_Training/GIT/
15) Найти файл по имени ======= $ find . file1.txt	
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает. ==== $ grep "word" file1.txt
17) вывести несколько первых строк из текстового файла ==== $ head -n2 file1.txt
18) вывести несколько последних строк из текстового файла ====== $ tail -n2 file1.txt
19) просмотреть содержимое длинного файла (команда less) изучите как она работает. ==== $ less --help
																						                                            $ less file_long.txt
20) вывести дату и время ======= $ date
=========

Задание *
### 1)  Отправить http запрос на сервер ###
	http://162.55.220.72:5005/terminal-hw-request  
	$ curl http://162.55.220.72:5005/terminal-hw-request   ->   "Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"Send the next URL in terminal: 
	http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}
		
	$ curl  'http://162.55.220.72:5005/get_method?name=Igor&age=115'      ->      ["Igor","115"]

### 2)  Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13 ###
>$ nano script.sh
>>#!bin/bash  
>>cd git  
>>mkdir folder_1 folder_2 folder_3  
>>cd /d/QA_training/git  
>>touch git file_1.txt file_2.txt file_3.txt j_file_1.json j_file_2.json  
>>mkdir folder1 folder2 folder3  
>>ls -la  
>>mv /d/Qa_training/Git file_1.txt file_2.txt /d/Qa_training/Git  
