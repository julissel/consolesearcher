# consolesearcher
**Задание №1 "Консольная программа поисковик" для курса OTUS "Web-разработчик на Python".**


**Цель:**

Создать программу поисковик (консольную)
Пользователь вводит текст запроса, поисковую систему (google.com, yandex.ru, ...), количество результатов, рекурсивный поиск или нет, формат вывода (в консоль, в файл json, в csv).
Программа находит в интернете начиная от стартовой точки все ссылки на веб-странице в заданном количестве (название ссылки и саму ссылку).
Если поиск не рекурсивный, то берем ссылки только из поисковика, если рекурсивный, то берем первую ссылку, переходим, находим там ссылки, переходим, ...
В зависимости от выбранного формата вывода сохраняем результат (текст ссылки: ссылка) либо в консоль либо в файл выбранного формата.

**Реализована возможность выбора:**
- поисковой системы (Google.com, Duckduckgo.com),
- количества результатов,
- вариант вывода (консоль, json, xml, csv).

*Для поиска в Duckduckgo.com предварельно нужно установить Firefox и Geckodriver (sudo apt-get install firefox-geckodriver).*


**Установка**
 - Для установки нужно создать корневой репозиторий:
   
   *consolesearcher*
   
 - перейти в корневой репозиторий и склонировать проект: 
   
   *git clone https://github.com/julissel/consolesearcher.git*

 - создать виртуальное окружение:
   
   *python3 -m venv myenv*

 - активировать окружение:

   *source myenv/bin/activate*
 
 - установить зависимости:

   *pip install -r requirements.txt*

 - запустить:

   *python3 -m consolesearcher*

 - после взаимодействия с приложением выйти из виртуального окружения:
   
   *deactivate*


**Сборка пакета**

Для сборки пакета нужно перейи в корневую директорию проекта - consolesearcher. 

Далее выполнить следующую команду:

*python3 setup.py sdist bdist_wheel* 
