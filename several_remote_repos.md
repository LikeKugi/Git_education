# Подключение к нескольким удалённым репозиториям

- Создаём связь с исходным репозиторием:

```
 git remote add source path
```

- Просматриваем связи и убеждаемся, что все установились:

```
 git remote -v
```

- Вносим изменения в локальный код и отправляем в оба репозитория:

```
git push -u origin master
git push -u source master
```

- Просматриваем изменения в удалённых репозиториях
- Вносим в удалённых репозиториях изменения в разные файлы
- Затягиваем изменения:

```
 git fetch --all
```

- Просматриваем их:

```
git log origin/master ^master
git log source/master ^master
```

- Вливаем их:

```
git merge origin/master
git merge source/master
```
