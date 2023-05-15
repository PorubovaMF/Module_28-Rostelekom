Проводилось тестирование пользовательского интерфейса c с элементами позитивного и негативного функциогального тестирования c помощью программной библиотеки Selenium . Список тест-кейсов, чек-лист и баги представлены по ссылке: https://docs.google.com/spreadsheets/d/1pzW-KgoIREkmPhcVIBgWqsg7L6afFNad/edit?usp=sharing&ouid=115355369804812515946&rtpof=true&sd=true

В файлах: test_authorization_by_code_page_rt.py, test_authorization_page_rt.py, test_registration_page_rt.py написана реализация тест-кейсов

В файле conftest.py реализована логика запуска браузера и добавлен обработчик, который считывает из командной строки параметр browser_name, а так же language (если сайт поддерживает разные языки) Браузер объявлется в фикстуре browser и передается в тест как параметр. Tест запускается с параметром browser_name следующей командой: pytest -m pytest -v --browser_name chrome .\test_authorization_page_rt.py
