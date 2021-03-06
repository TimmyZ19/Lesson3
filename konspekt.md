# Конспект по работе с Git
<img align="right" src="https://cdn-icons.flaticon.com/png/512/4494/premium/4494748.png?token=exp=1657717570~hmac=ad225bdcda0f547bfe83ca0ac59b84a5" width="100"> 


## Первоначальная настройка Git
### Утилита git confiig :
 - Посмотреть все установленные настройки и узнать где именно они заданы, используйте команду :
      
      ***git config --list --show-origin***
- Первое, что следует сделать после установки Git — указать имя и адрес электронной почты :
     
     ***git config --global user.name ~~"name user"~~***

    ***git config --global user.email ~~name@example.com~~***


 - Проверить используемую конфигурацию, можете использовать команду
    
    ***git config --list***


### Инициализация репозитория :
- Команда создаёт __в текущем каталоге__ новый подкаталог с именем .git, содержащий все необходимые файлы репозитория — структуру Git репозитория:

    ***git init***

## Основные команды Git
 - git add - добавляет содержимое рабочей директории в индекс для последующего коммита.
    > ***git add .*** - добавляет содержимое всей выбранной директориий для последующего коммита

    > ***git add namefile*** - добавляет указанный файл для последующего коммита

- git status - показывает состояния файлов в рабочей директории и индексе: какие файлы изменены, но не добавлены в индекс; какие ожидают коммита в индексе. Вдобавок к этому выводятся подсказки о том, как изменить состояние файлов

- git deff - используется для вычисления разницы между любыми двумя Git деревьями. Это может быть разница между вашей рабочей директорией и индексом
    > ***git diff --staged*** - разница между индексом и последним коммитом

    > ***git diff master branchB*** - между любыми двумя коммитами

- git commit - берёт все данные, добавленные в индекс с помощью **git add**, и сохраняет их слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок


## Команды для ветвления и слияния
- git checkout - используется для переключения веток и выгрузки их содержимого в рабочую директорию
- git merge - используется для слияния одной или нескольких веток в текущую. Затем она устанавливает указатель текущей ветки на результирующий коммит.
- git log - спользуется для просмотра истории коммитов, начиная с самого свежего и уходя к истокам проекта
    > ***git log -p*** - показывает дельту по строкам привнесенную каждым коммитом

    > ***git log -p --word-diff*** - для отображения дельты по словам
                                     

# Работа с ветвлением и слиянием

## Ветка 4
Конфликт

## Ветка 3 с инфомацией из ветки 1
## Ветка 1
Заполнение из ветки 1







## ветка 2
![](https://i.gifer.com/7h7L.gif)

# Работа с удаленным репозиторием

## Подключение к удаленному репозиторию
>git remote add origin "ссылка на репозиторий"

## Отправить изменения в удаленный репозитарий
>git push origin master

## Запросить изменения с удаленного репозитария
>git pull origin master

## Клонировать удаленный репозитарий
>git clone "ссыдка на репозиторий"
___
![](https://i.gifer.com/1abF.gif)
