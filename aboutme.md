# Анкета

#### FE:
* Если необходимые данные не заполнены - выводится окно оповещения о заполнении анкеты
* При изменении анкеты выоводится окно ошибки, если информация поля "О себе" не заполнена.

#### BE:

* После успешном изменении анкеты используется метод [`POST/profile/info`](https://leoka-estetica-dev.ru.net/swagger/index.html)
* При переходе на страницу "Анкета", сервер возвращает данные анкеты, используя методы:
[`GET/profile/menu`](https://leoka-estetica-dev.ru.net/swagger/index.html)
[`GET/profile/skills`](https://leoka-estetica-dev.ru.net/swagger/index.html)
[`GET/profile/intents`](https://leoka-estetica-dev.ru.net/swagger/index.html)
[`GET/profile/remarks`](https://leoka-estetica-dev.ru.net/swagger/index.html)
[`GET/profile/info`](https://leoka-estetica-dev.ru.net/swagger/index.html)
[`GET/profile/selected-intents`](https://leoka-estetica-dev.ru.net/swagger/index.html)
[`GET/profile/selected-skills`](https://leoka-estetica-dev.ru.net/swagger/index.html)
* POST/profile/select-menu
