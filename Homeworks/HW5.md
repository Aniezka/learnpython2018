## Поисковая система для корпуса

В этом задании вам нужно будет написать свой "Яндекс", который будет искать информацию в ранее собранном вами корпусе газеты из [третьго ДЗ](https://github.com/ancatmara/learnpython2018/blob/master/Homeworks/Project.ipynb).

Для этого вам потребуется:

1. Придумать структуру базы данных и добавить в нее названия статей, их тексты, очищенные от тегов и прочего мусора (те, что лежат у вас в папке `plain` в третьем ДЗ) и ссылки на эти статьи на сайте вашей газеты. По желанию можно добавить в базу и другие метаданные: дату, автора и т.д.
2. Создать веб-сервис, в котором можно будет вбить произвольную фразу и получить ссылки на материалы, где она встречается, и кусочек страницы с ней. Т.е. на странице результатов поиска должен выводиться список всех статей, в тексте которых нашлось заданное слово / фраза. Каждый элемент списка -- это ссылка на эту статью на сайте и кусочек текста статьи (того, что лежит в вашей базе данных), содержащий запрос. Размер выводимого кусочка статьи -- на ваше усмотрение, рекомендуемая длина -- 250-500 символов. 

Результаты поиска желательно выводить на главной странице. Если для них создана отдельная страница, то поле для ввода поискового запроса должно быть и там. 

В качестве СУБД рекомендуем использовать SQLite.

### Критерии

|Балл|Критерий|
|----|--------|
|2|Программа запускается и оформлена по PEP8. Соответствие PEP8 можно проверить с помощью команды `pycodestyle my_script_name.py` в командной строке.|
|2|Создана база данных, в которой есть тексты статей, их названия и ссылки на эти статьи на сайте газеты|
|1|Создано фласк-приложение с формой поиска на главной странице|
|2|При отправке запроса через форму поиска формируется корректный sql-запрос|
|1|Sql-запрос возвращает нужные данные из базы|
|2|Данные отображаются на странице согласно требованиям|
|1|**Бонусный балл** за оформление сайта с помощью bootstrap|

**NB!** Это задание, как и предыдущее, лучше сдавать в виде обычного .py скрипта (а не тетрадки).

**NB!** Если Вы не сделали задание 3, то создайте базу данных с нуля.