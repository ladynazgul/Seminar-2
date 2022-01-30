# Инструкция для работы с Git

## Что такое Git?

Git - это одна из реализаций систем контроля версий, имеющая как локальные, так и удаленные репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Подготовка репозитория

Для создания репозитория необходимо выполнить команду *git init*  в папке с репозиторием, и у вас создастся репозиторий (появится скрытая папка .git).

## Создание коммитов

### Git add

Для добавления изменений в коммит используется команда *git add*. Чтобы использовать команду *git add*, напишите *git add <имя файла>*.

### Создание коммитов

Для того, чтобы создать коммит (сохранение), необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m <сообщение к коммиту>*. Всe файлы для коммита должны быть ***ДОБАВЛЕНЫ***, и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями

Для перемещения между коммитами и ветками используется команда *git checkout <код коммита или имя ветки>*. Код коммита получаем с помощью команды *git log*.

## Журнал изменений

Для просмотра всех существующих коммитов используется команда *git log*. Если к ней добавить аргумент *--graph*, то можно получить журнал коммитов в более наглядном представлении.

## Ветки в Git

Ветки используются как черновик, а также для организации работы команды. Для просмотра имеющихся веток используется команда *git branch*. Чтобы создать новую ветку, надо выполнить эту же команду с добавлением имени новой ветки: *git branch <название новой ветки>*.

## Слияние веток

Команда *git merge <имя ветки>* выполняет слияние веток. Вызывать из той ветки, с КОТОРОЙ нужно слить изменения, а не из той КОТОРУЮ сливаете. При этом могут возникунуть конфликты, их можно решить из основной ветки.

## Удаление веток