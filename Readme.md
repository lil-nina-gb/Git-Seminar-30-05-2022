# Инстуркция по работе с git и удаленными репозиториями

## Что такое git?
Git - это система управления версиями. У Git две основных задачи : первая - хранить информацию о всех изменениях в вашем коде, начиная с самой первой строчки, а вторая - обеспечение удобства командной работы над кодом.
*Git* одна из реализаций распределенных систем контроля версий. Самой популярной реализацией *Git* является [Github](https://github.com)


## Подготовка репозитория   
Для того, чтобы создать репозиторий используется команда *git init*. Для этого необходимо написать в терминале в папке будущего репозитория команду *git init*

### Добавление файла к коммиту 

Для добавления файла к коммиту используется команда *git add*. Пишется она следующим образом *git add <имя файла>* в терминале в папке с созданным репозиторием.

### Создание коммита

Для создания нового "сохраниения" используется команда *git commit*. Импользуется она следующим образом: в терминале с папкой-репозиторием пишется *git commit -m <сообщение к коммиту>*. Сообщение к коммиту писать **ОБЯЗАТЕЛЬНО**!

## Перемещение между сохранениями 
Для перемещения между сохранениями используется команда *git checkout*. Для того, чтобы перемиститься на указанный коммит в терминале в папке с репозиторием пишем *git checkout <номер коммита>*. **Номер коммита** берется из журнала ихменений,, о котором сказано выше. После перемещения на указанный коммит мы попадаем в состояние **detached head*. Чтобы вернуться к обычной работе, необходимо написать *git checkout master*

## Журнал изменений 

Для просмотра журнала изменений используется команда *git log*. Для этого в терминале в папке с репозиторием достаточно написать *git log*.

## Ветки git
Ветки в *git* нужны, чтобы работать с "чистовиком" и "черновиками". Для того, чтобы создать новую ветку используется команда *git branch*. В терминале в папке с репозиторием, напишите *git branch <название ветки>*.

## Слияние веток и разрешение конфликтов 
Для слияния веток используется команда *git merge*. Для ее использования необходимо перейти в ту ветку куда Вы хотите сделать слияние. После чего в терминале в папке с репозиторием написать *git merge <название сливаемой ветки>*. Чаще всего слияние происходит автоматически, но возможны **конфликты**. В таком случае, необходимо вручную получить желаемую версию файла и сделать коммит.

## Удаление веток 
Для удаление ветки используется команда *git branch -d*. Для этого необходимо в папке с репозиторием в терминале написать *git branch -d <название ветки>*. Удаляемая ветка **обязательно** должна быть **слита**.

## Получение удаленного репозитория






