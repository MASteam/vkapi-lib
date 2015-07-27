# VKapi-lib
**VKapi-lib** -- это библиотека, написанная на Java для работы с ВКонтакте API.

## Документация

### Установка
Для использования библиотеки нужно скомпилировать ее в .jar и включить в проект в вашей IDE.
### Использование
Для методов, требующих **access_token** нужно его установить:
```java
Vk.token = "YOUR_TOKEN";
```
Также вы можете установить кодировку (по-умолчанию **windows-1251**) или версию используемого API (по-умолчанию **5.35**):
```java
Vk.encoding = "UTF-8";
Vk.version = 5.34;
```
Работа с API заключается в использовании классов, соответствующих названию методов. Пример использования метода **users.get:**
```java
String user_info = Users.get("user_ids=1&fields=city,sex,country&name_case=nom");
```

## Лицензия
[The MIT License](http://opensource.org/licenses/MIT)
