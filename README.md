# __Лабораторная работа №6__
## __Цель работы__
Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием. 
## __Порядок выполнения работы__
### 1. Создать аккаунт на сайте GitHub.
### 2. Сделать копию в личное хранилище из https://github.com/Kurtyanik/LR6/ (Fork).
### 3. Установить Git (https://git-scm.com/)
### 4. После установки настроить клиент git, введя имя пользователя (Группа Фамилия И.О.) и email.
### 5. Клонировать свой личный удалённый репозиторий на компьютер.
### 6. Добавить файл через интерфейс GitHub. Подтянуть изменения в локальный репозиторий. 
### 7. Получить историю операций для каждой из веток
### 8. Просмотреть последние изменения.
### 9. Выполнить слияние в ветку master, разрешив конфликт (можно использовать специальные редакторы или графический интерфейс git).
### 10. Удалить побочную ветку после успешного слияния.
### 11. Сделать изменения и зафиксировать их, оставляя комментарии, несколько раз. 
### 12. Сделать откат коммита.
### 13. Создать ветку для отчёта.
### 14. Начать оформлять отчёт в файле README.md (разрешены сторонние редакторы с подсветкой синтаксиса), используя markdown синтаксис (https://guides.github.com/features/mastering-markdown/): 
#### 1. В отчёте должен быть снимки экрана консоли и сторонних программ. Файлы снимков экрана разместить в отдельной папке. 
#### 2. Лог команд (без результатов их выполнения).
### 15. Получить историю операций в форматированном виде (сокращённый хэш + дата + имя автора + комментарий). Добавить её в отчёт и сделать финальную фиксацию изменений. 
### 16. Отправить локальные изменения в сетевое хранилище GitHub (если делаете работу постепенно, то синхронизацию проводить в конце рабочего сеанса)
## __Выполнение работы__
Ввод имени пользователя и email

(/Images/Screenshot_1.png)


Клонирование репозитория на компьютер

(/Images/Screenshot_2.png)


Добавил файл example.txt и подтянул изменения в нем в локальный репозиторий

(/Images/Screenshot_3.png)

Содержимое файла

(/Images/Screenshot_14.png)


Получил историю операций для каждой из веток

(/Images/Screenshot_4.png)

Были созданы две ветки V1 и V2. 

(/Images/Screenshot_6.png)

(/Images/Screenshot_8.png)

В каждой из веток файл example.txt был изменен по разному, это продемонстрировано на скриншотах

Скриншот с изменениями в V1

(/Images/Screenshot_15.png)

Скриншот с изменениями в V2

(/Images/Screenshot_16.png)

Выполнил слияние в ветку мастер вручную

(/Images/Screenshot_9.png)

Содержимое файла example.txt вручную было устаневлено такое как на скриншоте ниже

(/Images/Screenshot_17.png)

Побочные ветки V1 и V2 были удалены

(/Images/Screenshot_11.png)

(/Images/Screenshot_20.png)

В файл example.txt было добавлено 2 изменения и они были зафиксированы комитами

(/Images/Screenshot_21.png)

Первое изменение 

(/Images/Screenshot_19.png)

Второе изменение

(/Images/Screenshot_18.png)

Затем был произведен откат коммита

(/Images/Screenshot_22.png)

Состояние файла после него

(/Images/Screenshot_19.png)

Получил историю операций в форматированном виде 

(/Images/Screenshot_23.png)

## __Лог команд (без результатов их выполнения)__

git reflog

git checkout report

git checkout master

git checkout V1

git checkout V2

git reset --hard d2db345

git commit -m "второе изменение файла"

git commit -m "первое изменение файла"

git commit -m "добавил в папку новый скриншот"

git commit -m "Изменил файл example.txt вручную чтобы избежать конфликт"

git add example.txt

git add README.md

git add Images

git push origin report

git branch -d V2

git branch -d V1

git branch V2

git branch V1

git merge V2

git merge V1

git push origin report

git push origin master







