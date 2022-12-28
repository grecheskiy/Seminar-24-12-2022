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
Для того, чтобы посмотреть, на какой ветки находимся, необходимо ввести команду в терминале *git branch*.
Для того, чтобы создать новую ветку используется команда *git branch <name file>*. 

### Создание веток в Git
Для создания новой ветки используется команда *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать *git branch <название ветки>*
### Просмотр списка веток
Для просмотра списка веток используется комнада *git branch*. Для этого в терминале с папкой-репозиторием необходимо написать команду *git branch*. Зелёным цветом с символом **звёздочка** будет выделена текущая ветка

### Переключение между вектами
Для перехода на другую ветку используется команда *git checkout*. Для этого в терминале с папкой-репозиторием пишем команду *git checkout <название ветки*. Для перехода на ветку ветка должна быть ***создана***!!!

## Слияние веток и разрешение конфликтов
Для того, чтобы произвести слияние ветки с текущей, необходимо в терминале набрать команду *git merge <name file>*. После, если производились изменения в текущем файле, происходит конфликт. Необходимо выбрать какие версии файла оставить, после произвести сохранение файла.

## Удаление веток
<<<<<<< HEAD
После слияния, если ветка которую слили больше не нужна, можно удалить.
Для удаления ненужной ветки, необходимо ввести в терминале команду *git branch -d <name file>*
=======

## Копировать внешний репозиторий
Копировать внешний репозиторий на свой ПК можно командой *git clone*.
Команда git clone составная: она не только загружает все изменения, но и пытается слить 
все ветки на локальном компьютере и в удаленном репозитории.

## Отправить свою версию репозитория во внешний репозиторий
Отправить свою версию репозитория во внешний репозиторий поможет команда *git push*. При первом её использовании 
нужна авторизация.

## скачать все из текущего репозитория
Команда *git pull* позволяет скачать все из текущего репозитория и автоматически сделать merge с нашей версией.

## Как настроить совместную работу
1. Создать аккаунт на GitHub.com
2. Создать локальный репозиторий
3. “Подружить” ваш локальный и удалённый репозитории. 
   GitHub при создании нового репозитория подскажет, как это можно сделать
4. Отправить (push) ваш локальный репозиторий в удалённый (на GitHub), при этом, возможно, вам нужно 
   будет авторизоваться на удалённом репозитории.
5. Провести изменения “с другого компьютера”.
6. Выкачать (pull) актуальное состояние из удалённого репозитория.

### pull request
➜ команда для предложения изменений
➜ запрос на вливание изменений в репозиторий
В больших компаниях один ответственный за проект создает аккаунт. Другие пользователи дают
команду pull request. Предлагать изменения на GitHub нужно в отдельной ветке. Сначала
пользователь копирует репозиторий на свой компьютер, делает fork репозитория, затем
клонирует версию на своём ПК, создаёт ветку с предлагаемыми изменениями, отправляет
изменения командой push в свой аккаунт на GitHub и даёт команду pull request. 

## Как сделать pull request
1. Делаем   (ответвление) репозитория fork
2. Делаем git clone   версии репозитория СВОЕЙ
3. Создаем новую ветку и в НЕЕ вносим свои изменения
4. Фиксируем изменения (делаем коммиты)
5. Отправляем свою версию в свой GitHub
6. На сайте GitHub нажимаем кнопку pull request
>>>>>>> GitRemoteRepositories
