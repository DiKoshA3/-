<!-- PROJECT LOGO -->
<br />
<div id="header" align="center">
  <img src="https://s14.stc.yc.kpcdn.net/share/i/12/13143964/wr-960.webp" "Optional title"/>
</div>
  <h3 align="center">Дипломный проект: реальный кейс компании "Ростелеком Информационные технологии"</h3>


<!-- ABOUT THE PROJECT -->
## О проекте


Тестирование сайта Ростелекома: <br />
1) Авторизация по логину и паролю: <br />
-по логину и паролю;<br />
-по номеру телефона, кнопка "Номер";<br />
-по номеру телефона, кнопка "Email"; <br />
-по номеру телефона, кнопка "Войти";<br />
-по номеру телефона, кнопка "Личный кабинет".<br />
2) Авторизация по тайм-коду.<br />
3) Восстановление пароля:<br />
-тип восстановления пароля;<br />
-восстановить пароль клиента по номеру телефона, кнопка "По номеру телефона";<br />
-восстановить пароль клиента по номеру телефона, нажав кнопку "По электронной почте".<br />
4) Регистрация:<br />
-основные шаги;<br />
-с помощью настройки (Блокировать/отключать cookies).<br />
Автоматическое тестирование сайта https://b2c.passport.rt.ru 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

При тестировании сайта использовались следующие методы разработки тестов:

* анализ граничных значений;
* разделение на классы эквивалентности;
* Тестирование состояний и переходов.


Библиотеки PyCharm, использованные при тестировании:

* __pageobject__ <br />
Это шаблон проектирования, который используется при написании автоматизированных тестов.
* __pytest__ <br />
Стандартный фреймворк pytest позволяет легко создавать небольшие, интуитивно понятные тесты и шкалы для поддержки комплексного функционального тестирования приложений и библиотек.
* __selenium__ <br />
Эта библиотека позволяет писать автоматизированные тесты, поддерживает все основные браузеры, а тесты могут быть написаны на многих языках программирования, а также запускаться на разных платформах.
* __faker__ <br />
Это библиотека, которая позволяет генерировать случайные данные. Ее можно использовать для заполнения таблиц в базе данных, создания корректных XML-документов и генерации ответов в формате JSON для REST.

Чтобы начать тестирование, вам нужно нажать через __Open Folder__ загрузить свой проект, далее открыть терминал через вкладку __Terminal__ и нажать __New Terminal__, необходимо загрузить библиотеки, если они отсутствуют, с помощью команды __pip install *библиотека*__.
Для создания временного адреса электронной почты использовался веб-сайт. www.1secmail.com

Проект содержит файлы:

* base_page.py - находится конструктор webdriver и общие для всех тестируемых страниц методы;

* auth_page.py - содержит методы проверок формы авторизации;

* change_pass_page.py - содержит методы проверок формы восстановления пароля;;

* reg_page.py - содержит методы проверок формы регистрации;

* test_auth_page.py - запуск тестов формы авторизации;

* test_change_pass_page.py - запуск тестов формы восстановления пароля;

*  test_reg_page.py - запуск тестов формы регистрации;

* locators.py - находятся все локаторы;

* conftest.py - находится фикстура с функцией открытия и закрытия браузера;

* settings.py - находятся методы и переменные для параметризации тестов;

* pytest.ini - зарегистрированы метки маркировок тестов.


Тестовые примеры, отчеты об ошибках и контрольный список доступны на Google Диске https://drive.google.com/drive/folders/1BbX-KV39YtDE2c98BynPZShf7zAqvLKq?usp=drive_link
