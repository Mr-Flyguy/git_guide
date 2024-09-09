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
## Радуемся!
