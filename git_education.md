# Мое руководство по работе с git
## Global settings
- git config --global user.name "*username*" - Имя пользователя для всех git на рабочей станции
- git config --global user.email "*user@email*" - E-mail пользователя
- git config --list - посмотреть файл конфига
## Init repo
- **git init** служит для инициализации репозитория
- **git add <mask_name>** служит для индексации файлов/папок  
- **git status** служит для просмотра статуса индексированных/неиндексированных файлов в репозитории
- **git commit -m "commit_message"** служит для фиксации изменений в репозитории
- **git commit -a -m "commit_message"** если лень делать git add, а зафиксировать изменения надо в *проиндексированных файлах*