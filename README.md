# Инструкция по развертыванию проекта.

1. `python3 -m venv venv_name` - создание виртуального окружения.
2. `source venv_name/bin/activate` - активация виртуального окружения.
3. `pip install -r requirements.txt` - подключить все библиотеки проекта.
4. `python manage.py migrate` - создать базу данных.
5. `python manage.py runserver` - запустить сервер.
6. `pip install freeze > requirements.txt` - обновить список библиотек по окончанию проекта.

## Запуск терминала в контексте django
`python manage.py shell_plus --ipython`

---

# Список всех заданий:

## Задания
### Выполнять после: Модуль-1
1. [x] Создайте новый проект DjangoCountries. 
Создайте новое виртуальное окружение(venv), установите в него Django.
Рекомендация: выполните все действия используя терминал Linux.
2. [x] Главная страница должна быть доступна по корневому url’у.
На ней разместите произвольное приветствие c минимальным HTML оформлением.
3. [x] Запустите проект и проверьте отображение главной страницы.
4. [x] Загрузите ваш проект на GitHub
Важно: не забудьте в проект добавить .gitignore. Виртуальное окружение и настройки вашей IDE не должны быть частью репозитория.

### Выполнять после: Модуль-2
1. [x] Оформите главную страницу в виде полноценного html-документа
2. [x] Список с данными для стран возьмите тут.
Примечание: пока мы работаем без БД, скопируйте данные о странах в файл (разместите файл в корне проекта).
 Для получение информации из файла используйте работу с файлами в Python, работа с json-1 и работа с json-2.
3. [x] По url: /countries-list/ отобразите нумерованный список всех стран, отобразив в списке только названия стран.
4. [x] Название каждой страны сделайте гиперссылкой, которая ведет на персональную страницу данной страны. 
На персональной странице страны отобразите ее название(в виде заголовка) и список всех языков, на которых говорят в данной стране.

### Выполнять после: Модуль-3
1. [x] Создайте модель-класс Country.
2. [x] Перенесите все страны из исходного json файла в базу данных(БД).
3. [x] Измените работу вашего приложения на работу с БД
4. [x] Выгрузите данные из БД в фикстуру(fixture) countries.json

### Выполнять после: Модуль-4
1. [x] Используя информацию с занятия, измените структуру БД, реализовав связь “многие-ко-многом” для стран и языков.
Не забудьте: выгрузить обновленные данные из БД fixture: countries.json
2. [x] Добавьте в проект файл requirements.txt
3. [x] Добавьте в проект файл README.md, добавив в него:
1. [x] * Информацию о запуске проекта после клонирования
2. [x] * Список всех заданий, пометив выполненные
### Выполнять после: Модуль-5
Примечание: Модуль-5 “работа с формами”, в рамках проекта “Django Countries” мы не будем использовать формы, поэтому задания с формами не связаны.

1. [x] 
2. [x] На главной странице добавьте еще одну ссылку “Языки”. По ссылке отобразите страницу со списком всех языков на котором говорят во всех странах.
3. [x] Все языки в списке сделайте гиперссылками, каждая ведет на отдельную страницу, на которой отображаются страны, которые говорят на выбранном языке.
### Выполнять после: Модуль-7 (финальные задания)
* На верху страницы со списком стран добавьте алфавит, каждая буква которого является гиперссылкой. Каждая гиперссылка(на букве) ведет на страницу на которой отображаются только страны на выбранную букву. См. аналогию тут.
* Внизу страницы со списком стран реализуйте пагинацию. На каждой странице отобразите 10 стран.