# Инструкция по работе с Git и удалёнными репозиториями

## Что такое git?
**Git** - это наиболее популярная реализация распределённой системы контроля версий. Самая популярная реализация **Git** - это [GitHub](https://github.com/)

## Подготовка репозитория
Для сооздания репозитория используется команда *git init*. Для этого необходимо в терминале перейти в пустую папку, где в будущем будет репозиторий. Затем в терминале с папкой написать команду *git init*.

## Создание коммитов

### Добавление файла к коммиту
Для добавления файла к будущему коммиту используется команда *git add*. Для этого в терминале с папкой-репозиторием необходимо написать *git add <название файла>*.

### Создание коммита
Для создания коммита используется команда *git commit*. Для этого в терминале с папкой репозиторием необходимо написать *git commit -m <сообщение к коммиту>*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО!!!***.

## Журнал изменений
Для просмотра журнала изменений используется команда *git log*. Для этого в терминале с папкой-репозиторием необходимо написать *git log*.

## Перемещение между коммитами
Для перемещения на предущие коммиты используется команда *git checkout*. Для этого необходимо в журнале изменений, как показано в предыдущей части, найти необходимый коммит и его номер. После чего в терминале с папкой-репозиторием написать команду *git checkout <номер коммита>*. После примененения этой команды Вы попадёте в состояние **Detached head**, в котором никакие изменения фиксироваться не будут. Для возврата в обычное состояние необходимо написать команду *git checkout master*.

## Ветки в Git
### Создание веток в Git
Для создания новой ветки используется команда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch <название ветки>*
### Просмотр списка веток
Для просмотра списка веток используется комнада *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать команду *git branch*. Зелёным цветом с символом **звёздочка** будет выделена текущая ветка

### Переключение между вектами
Для перехода на другую ветку используется команда *git checkout*. Для этого в терминале с папкой-репозиторием пишем команду *git checkout <название ветки*. Для перехода на ветку ветка должна быть ***создана***!!!

## Слияние веток и разрешение конфликтов

Для слияние веток используется команда *git merge __/branch's name/__*
Если при слиянии веток происходит конфликт, тоесть в ветке которую мы хотим залить и в ветке в которую мы хотим залить есть различия , то программа выдает нам окно выбора с тем , что было, что будет и что могло было быть... И нам необходимо выбрать, вносить изменения или нет, или собрать все что было вместе. 

## Удаление веток

## Работа с репозиториями в гит хаб.

Для работы с репозиториями на гитхабе, необходимо :
1. зарегестрироваться на гитхабе
2. на главной странице во вкладке *repositories* нажать *new*
3. ввести название репозитория в *repository name*
4. сделать его публичным  выбрав *public*
5. нажать зеленую кнопку *create ropository*
6. Вести последовательно данные команды в терминале в Visual Code
    * **git remote add origin https://github.com/BigGrib/new.git**
    * **git branch -M main**
    * **git push -u origin main**
7. После того как все загрузится продлжить работать.

### Работа с удаленными репозиториями

+ git clone - скопировать репозиторий
+ git push - залить репозиторий
+ git pull - скачать репозиторий
+ (в самом реппозитории на гитхаб) fork - скопировать весь репозитори к себе на аккаунт
+ (в самом реппозитории на гитхаб) pull request - показать собственнику изменения
