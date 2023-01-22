# Инструкция по работе с Git

## Что такое Git?

***Git*** - это одна из реализаций распределенной системы контроля версий, поддерживащей как локальные, так и удаленные репозитории. Самая популярная реализация Git - это [GitHub](https://github.com/).

## Подготовка репозитория

Для создания репозитория используется команда **git init**. Для этого необходимо открыть в терминале папку с будущим репозиторием и там написать **git init*.

## Создание коммитов

### Добавление файла к коммиту

Для добавления файла к коммиту используется команда **git add**. Для этого в терминале с папкой-репозиторием нужно написать **git add <название файла>**.

### Выполнение коммитов

Для того, чтобы выполнить коммит используется команда **git commit**. Для этого в терминале с папкой-репозиторием нужно написать **git commit -m "<сообщение к коммиту>"**. Сообщение к коммиту писать нужно ***ОБЯЗАТЕЛЬНО***.

## Журнал изменений

Для просмотра истории используется команда **git log**. Для этого в терминале с папкой-репозиторием нужно написать **git log**. В открывшемся журнале можно найти:
* Хеш (номер) коммита,
* Дату и время коммита,
* Автора коммита,
* Сообщение коммита.

## Перемещение между коммитами

Для перемещения между коммитами используется команда *git checkout*. Для этого в терминале с папкой-репозиторием нужно написать **git checkout <хеш коммита>**. Хеш коммита можно найти в истории коммитов, о которой рассказано в предыдущем пункте.

## Ветки в Git
### Просмотр списка веток
Чтобы увидеть полный список существующих веток, достаточно написать в терминале команду **git branch**. Ветка, в которой вы находитесь сейчас, будет отмечена звездочкой и выделена зеленым цветом.

### Перемещение между ветками

Чтобы перемещаться между ветками, используется команда **git checkout**. Для этого в терминале с папкой-репозиторием нужно написать **git checkout <название ветки>**.

### Создание новых веток
Чтобы добавить ветку в Git, используется команда **git branch**. Для этого в терминале с папкой-репозиторием необходимо набрать **git branch <название ветки>**.

## Слияние веток и разрешение конфликтов
### Слияние веток
Чтобы слить две ветки, необходимо проверить, что вы находитесь в нужной ветке (с помощью команды **git branch**), а затем использовать команду **git merge**. Для этого в терминале написать **git merge <название сливаемой ветки>**.

### Разрешение конфликтов
При возникновении конфликта просто отредактируйте конфликтующий файл, выполните сохранение и создайте новый коммит с помощью команд **git add* и **git commit**.

## Удаление веток
Чтобы удалить ненужные ветки используйте команду **git branch -d**. В терминале с папкой-репозиторием напишите **git branch -d <название удаляемой ветки>**.
