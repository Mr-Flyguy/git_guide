# Гайд по пользованию git для новичка
---
## Скачивание git bash  
* Качаем [здесь](https://git-scm.com/download/win)
---
## Основные команды  
* **ls** — Отображение списка файлов и папок в текущей директории.  
* **cd [директория]** — Переход в указанную директорию.  
* **cd ..** — Перейти на уровень выше (в родительскую директорию).  
* **pwd** — Отображение текущего пути (в какой директории вы находитесь).  
* **cat [файл]** — Вывод содержимого файла в консоль.  
* **touch [файл]** — Создание нового пустого файла.  
* **mkdir [директория]** — Создание новой директории (папки).  
* **rmdir [директория]** — Удаление пустой директории.  
* **rm [файл]** — Удаление файла.  
* **rm -r [директория]** — Удаление директории с содержимым.  
* **cp [файл] [новое_место]** — Копирование файла в указанное место.  
* **mv [файл/директория] [новое_место]** — Перемещение файла или папки в другое место (или переименование).
---
## Создание репозитория
* **git init** — создание локального репозитория.
* **git remote add origin <URL-репозитория>** — привязка к удалённому репозиторию.
* **git add .** — добавление всех файлов в индекс.
* **git commit -m "Сообщение коммита"** — создание коммита с сообщением.
* **git push -u origin master** — отправка изменений на удалённый репозиторий (-u используется только в первый раз).
---
## Хеш  
* Git преобразует информацию о коммитах с помощью алгоритма SHA-1 и для каждого из них рассчитывает уникальный идентификатор — хеш.
* Хеш — основной идентификатор коммита и позволяет узнать его автора, дату и содержимое закоммиченных файлов.
* Все хеши, а также таблицу соответствий хеш → информация о коммите Git хранит в папке .git.
--- 
## Логи  
* Вызываются командой **git log**
* Содержат **хеш, имя автора, дату и сообщения коммитов**
* Можно вызвать не только полный лог, но и сокращённый — это делается командой git log --oneline.
* В сокращённом логе выводятся сокращённые хеши — их можно использовать точно так же, как и полные.
---
## HEAD-файл
* Можно вызвать не только полный лог, но и сокращённый — это делается командой git log --oneline.
* В сокращённом логе выводятся сокращённые хеши — их можно использовать точно так же, как и полные.
---
## Статусы файлов
* Статусом **untracked** помечается файл, о существовании которого Git знает, но не следит за изменениями в нём. Этот статус — противоположность **tracked**, в который попадают все файлы, отслеживаемые Git.
* Файл переходит в статус **staged** после выполнения **git add**.
* Статус **modified** означает, что файл был изменён.
* Большинство файлов в проектах «шагает» по следующему циклу: «изменён» → «добавлен в список на коммит» → «закоммичен» → «изменён» → и так далее.
---
## Оформление сообщений к коммитам
* Сообщение не должно превышать 72 символов
* Сообщение должно быть информативным и чётким
* Сообщение должно соответсвовать одному из общепринятых стилей написания коммитов
---
## Откат файлов и коммитов
* Команда **git restore --staged <file>** переведёт файл из staged обратно в modified или untracked.
* Команда **git reset --hard <commit hash>** «откатит» историю до коммита с хешем <hash>. Более поздние коммиты потеряются!
* Команда **git restore <file>** «откатит» изменения в файле до последней сохранённой (в коммите или в staging) версии.
---
## Просмотр изменений в коммите
* Команда **git diff** сравнит последнюю закоммиченную версию файла с той, что находится в состоянии modified.
* Команда **git diff --staged** покажет изменения в staged-файлах относительно последних закоммиченных версий.
---
## .gitignore
* Игнорировать файл: filename
* Игнорировать папку: folder/
* Игнорировать все файлы типа: *.extension
* Исключить файл из игнорирования: !filename
* Игнорировать файлы в подкаталогах: **/*.extension
* Комментарии: # comment
## Радуемся!
