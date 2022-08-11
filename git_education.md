# <p align = center> __Мое руководство по работе с git__ </p>
  
![git workflow](images/Git-flow.jpg)  
<p align = center>работа с гит</p> 

## __Осовные команды гита__
___
### __Global settings__
___
- **git version** - Посмотреть версию Git
- **git config --global user.name "*username*"** - Имя пользователя для всех git на рабочей станции
- **git config --global user.email "*user@email*"** - E-mail пользователя
- **git config --list** - посмотреть файл конфига
### __Init repo__
___
- **git init** служит для инициализации репозитория
- **git add <mask_name>** служит для индексации файлов/папок  
- **git status** служит для просмотра статуса индексированных/неиндексированных файлов в репозитории
- **git commit -m "commit_message"** служит для фиксации изменений в репозитории
- **git commit -a -m "commit_message"** если лень делать git add, а зафиксировать изменения надо в *проиндексированных файлах*
- **git commit -a** коммит проиндексированных файлов  

последовательность добавления коммита:
<pre>
1. <kbd>Shift</kbd> + <kbd>I</kbd> Commit_message
2. <kbd>Esc</kbd>
3. <kbd>Shift</kbd> + <kbd>;</kbd>
4. <kbd>w</kbd><kbd>q</kbd> ===> <kbd>Enter</kbd>
</pre>
- **git checkout <*commit_name*>** перейти к конкретному коммиту
- **git checkout master** - вернуться в ветку *master* на актуальную версию коммита
- **git diff** сравнить изменения
## __Просмотр веток коммитов и изменений__
___
- **git log** служит для просмотра подробного журнала изменений. <kbd>Q</kbd> - выход из журнала
- **git log --pretty=oneline** посмотреть изменения в удобном формате в одну строчку один коммит
- **git log --pretty-short** краткий формат фиксаций
- **git log --graph** - просмотр лога в виде дерева
- **git log <_file_>** - показать фиксации файла
- **git log <_dir_>/** - показать фиксации директории
### __Работа с ветками Git__
___
- **git branch** - вывести все ветки в репозитории, указывает на текущую
- **git merge<_branchName_>** - влить <_branchName_> в текущую
- **git merge --abort** - отменить слияние веток
- **git branch <_branchName_>** - создать ветку *branchName*
- **git rebase <_branch_>** - перенести в ветку
- **git rebase <_main_>** - перенести в главную ветку
- **git rebase --abort** - отменить перенос
___
## Pull-Request workflow
1. Fork репозиторий с удаленного чужого - это создаст клон удаленного репозитория на странице GitHub
2. **Git Clone <_URL_>** - скопировать с сайта репозиторий в локальный
3. **Git branch <_branch-name_>** - создать ветку в репозитории. __Работать с форкнутыми репозиториями только в побочных ветках!!!__
4. **git checkout <_branch-name_>** - перейти в ветку. Работать в ней!
5. **git commit -m "_Commit-info_"** - зафиксировать изменения
6. **git push** - отправить репозиторий на удаленный сервер
7. **pull request** - появится пул-реквест. Запросить, если есть необходимость
