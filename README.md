# Projects_3
Тестовые сценарии проверяют кликабельность кнопок, равенство карточек товара и картинок/цен/и т.д. к ним. Постаралась сделать названия
тестов читаемыми, чтоб было понятно, что именно происходит.
Проверяется также присутствие элементов на странице.
Также добавила функцию формирования HTML отчета.
Для запуска теста необходимо знать путь до файла chromedriver.exe. Для этого в PyCharm в левой колонке находим файл chromedriver.exe,
кликает по нему правой клавишей мыши, выбираем Copy Path --> Absolute Path.
В моем случаем получился путь C:\Users\Татьяна\PycharmProjects\Projects_3\chromedriver.exe. Дописываем путь до файла с тестами Tests\login.py.
python -m pytest -v --html=.\Reports\report.html --driver Chrome --driver-path - показываем с помощью каких инструментов
будет работать тест и в каком браузере. --html=.\Reports\report.html - формирует отчет в HTML. Полная команда для запуска теста получилась такая:
python -m pytest -v --html=.\Reports\report.html --driver Chrome --driver-path C:\Users\Татьяна\PycharmProjects\Projects_3\chromedriver.exe Tests\login.py
