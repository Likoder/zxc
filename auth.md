# Авторизация/Регистрация

## Авторизация через email и password

#### FE:
* При авторизации пользователю необходимо заполнить форму:

|Name|Type|Description|
|-|--------|---|
|email|string|Электронная почта пользователя|
|password|string|Пароль|

* Пользователь может скрыть или открыть пароль при заполнении формы авторизации
* Всплывающее окно ошибки выводится при:
  1. Если email не существует в базе данных.
  2. Если пароль для конкретного email некорректен.

#### BE:

* Для авторизации авторизации используется метод [`GET/user/signin`](https://leoka-estetica-dev.ru.net/swagger/index.html)
* При успешной авторизации пользователь попадает на страницу "Профиль", сервер возвращает данные профиля, используя методы:
[`GET/profile/menu`](https://leoka-estetica-dev.ru.net/swagger/index.html)
[`GET/profile/skills`](https://leoka-estetica-dev.ru.net/swagger/index.html)
[`GET/profile/intents`](https://leoka-estetica-dev.ru.net/swagger/index.html)
[`GET/profile/remarks`](https://leoka-estetica-dev.ru.net/swagger/index.html)
[`GET/profile/info`](https://leoka-estetica-dev.ru.net/swagger/index.html)

## Регистрация 

#### FE:
* При регистрации пользователю необходимо заполнить форму:

|Name|Type|Validation|Description|
|-|--------|------|---|
|componentRoles|enum||Роль пользователя на платформе:<br>  1 - Соискатель <br>2 - Основатель<br>3 - Кадровое или аутстаффинговое агентство|
|email|string||Электронная почта пользователя|
|password|string||Пароль|

* Всплывающее окно ошибки выводится при:
  1. Если пользователь не выбрал роль на платформе
  2. Если пользователь не указал email.
  3. Если пароль не прошел валидацию.
  4. Если пользователь не принял согласие с условиями платформы.

#### BE:

* Для регистрации используется метод [`GET/user/signup`](https://leoka-estetica-dev.ru.net/swagger/index.html)
* При нажатии пользователем на ссылку "Правила использования платформы" , вызывается метод [`GET/press/offer`](https://leoka-estetica-dev.ru.net/swagger/index.html)
* При успешной регистрации пользователь попадает на страницу "Профиль".

## Авторизация через Google



## Авторизация через VK


## Logout
* 
