
## Подготовка
1. Установите VS Code https://code.visualstudio.com
2. Установите Git https://git-scm.com/downloads (Инструкция тут, хотя в целом там должно быть интуитивно https://git-scm.com/book/ru/v2/Введение-Установка-Git)
3. Проверьте, что git работает \
   3.1. Откройте Terminal в MacOS или Git Bash в Windows (в дальнейшем, если не узказано иное, команды выполняются в Terminal в MacOS и в Git Bash в Windows) \
   3.2. Выполните команду git --version \
   3.3. Если вы увидели вывод git version ..., значит все в порядке, git установлен.
4. Сгенерируйте SSH ключ по инструкции https://git-scm.com/book/ru/v2/Git-на-сервере-Генерация-открытого-SSH-ключа
5. Добавьте публичный ключ SSH в профиль github https://github.com/settings/keys (New SSH key)
6. Создайте папку, в которой вы будете работать, например Projects \
   $ cd ~ \
   $ mkdir Projects \
   $ cd Projects
7. Склонируйте репозиторий. Выполните команду в консоли: \
   $ git clone git@github.com:KateVasovski/soft-crafts-jule-2026.git
8. Откройте проект в VS Code. Если VS Code спросит "Do you trust the authors ... ?", выберете "Yes, ..." \
   $ code .
9. В VS Code откройте терминал Terminal -> New  Terminal
10. В меню VS Code включите опцию File -> AutoSave
11. Нужно выполнить команды в терминале, подставив своё имя и е-мейл: \
    $ git config --global user.name "John Doe" \
    $ git config --global user.email johndoe@example.com \
    $ git config --global pull.rebase true