## Работа с Git

Проверка наличия установленного Git
В терминале выполняем команду 'git --version', она выводит версию Git.


## Настройка Git

Ввод имени пользователя и почты:

git config --global user.name "username"
git config --global user.email "useremail"
Чтобы посмотреть изменения: 'git config --list'

## Инициализация Git

Чтобы инициализировать git: 'git init'


## Git status

Выводит статус текущей ветки: 'git status'


## Добавление файла к отслеживанию

Команда git add используется для добавления файлов в индекс Git. Добавьте файл в индекс с помощью команды 'git add <filename>' или добавьте все файлы с помощью 'git add .'


## Фиксация изменений

После добавления файлов в индекс вы можете сделать коммит, который зафиксирует ваши изменения. Используйте 'git commit -m "Commit message"', чтобы сделать коммит с сообщением.


## Информация об истории коммита

Чтобы просмотреть историю ваших коммитов, используйте команду 'git log'. Это покажет вам автора коммита, дату и сообщение коммита.


## Сравнение с последним коммитом

Команда 'git diff' позволяет вам увидеть различия между вашими рабочими файлами и файлами в индексе. Это позволяет вам видеть, какие изменения вы сделали, но еще не закоммитили.


## Перемещение между сохранениями

Команда git checkout используется для переключения между разными ветками и коммитами в вашем репозитории. Например, 'git checkout <branch-name>' переключит вас на указанную ветку.


## Добавление картинок 

![]() Чтобы добавить картинку, нужно скачать нашу картинку в нашу папку. Далее прописать в VSCode '![наш комментарий](имя картинки)'  Вуаля, вот она!


## .gitignore

Файл .gitignore используется для указания Git на файлы или директории, которые следует игнорировать и не отслеживать. Чтобы создать файл .gitignore, просто создайте новый текстовый файл с именем .gitignore в корневом каталоге вашего репозитория. Затем добавьте имена файлов, которые вы хотите игнорировать. Например, чтобы игнорировать png картинки '*.png', все файлы .log, добавьте '*.log' в ваш файл .gitignore


## Создание ветки

Чтобы создать новую ветку, воспользуемся командой 'git branch <имя ветки>'.


## Слияние веток

Слияние веток выполняется с помощью команды git merge. Для слияния вашей текущей ветки с другой веткой используйте 'git merge <other-branch-name>'


## Решение конфликтов

При слиянии веток могут возникнуть конфликты, если одни и те же части файла были изменены в обеих ветках. Git помечает конфликтные области в файле, и вам нужно ручное решить эти конфликты. Конфликтные области будут помечены <<<<<<<, ======= и >>>>>>>. Все, что находится между <<<<<<< и ======= - это ваш код, а все, что находится между ======= и >>>>>>> - это код из другой ветки.


## Удаление ветки

Чтобы удалить ветку, используйте команду 'git branch -d <branch-name>'. Это удалит ветку, если она была слита. Если вы хотите удалить ветку, даже если она не была слита, используйте 'git branch -D <branch-name>'.