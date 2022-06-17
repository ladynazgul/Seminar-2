# Инструкция для работы с Git и удаленными репозиториями

## Что такое Git?

Git - это одна из реализаций систем контроля версий, имеющая как локальные, так и удаленные репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду *git init*  в папке с репозиторием, и у вас создастся репозиторий (появится скрытая папка .git).

## Создание коммитов

### Git add

Для добавления изменений в коммит используется команда *git add*. Чтобы использовать команду *git add*, напишите *git add <имя файла>*.

### Просмотр состояния репозитория

Для того, чтобы посмотреть состояние репозитория, используется команда *git status*. Для этого необходимо в папке с репозиторием написать команду git status и вы увидите, были ли изменения в файлах или их не было.

### Создание коммитов

Для того, чтобы создать коммит (сохранение), необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m <сообщение к коммиту>*. Всe файлы для коммита должны быть ***ДОБАВЛЕНЫ***, и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями

Для того, чтобы перемещаться между коммитами и ветками, используется команда *git checkout <код коммита или имя ветки>*. Используется она в папке с репозиторием. Код коммита получаем с помощью команды *git log*.

## Журнал изменений

Для того, чтобы посмотреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием. Если к ней добавить аргумент *--graph*, то можно получить журнал коммитов в более наглядном представлении.

## Ветки в Git

Ветки используются как черновик, а также для организации работы команды. Для просмотра имеющихся веток используется команда *git branch*. Для того, чтобы создать ветку, надо выполнить в папке с репозиторием эту же команду с добавлением имени новой ветки: *git branch <название новой ветки>*.

## Слияние веток

Команда *git merge <имя ветки>* выполняет слияние веток. Вызывать из той ветки, с КОТОРОЙ нужно слить изменения, а не из той КОТОРУЮ сливаете. При этом могут возникунуть конфликты, их можно решить из основной ветки.

## Удаление веток

Чтобы удалить ветку, просто добавляем к команде *git branch* аргумент -d, затем указываем имя удаляемой ветки, напрмер, так *git branch -d deleteInfo*
