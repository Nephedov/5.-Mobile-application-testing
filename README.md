# «Снифферинг. Настройка и возможности»

## Решения
### Задание 1
* Throttle:
  * <a href="https://drive.google.com/file/d/1vbiv4LvxTBWC_GJ_gljAXN3hZUI9-HW6/view?usp=sharing"> Скриншот</a> Throttle настроек, с нулевой скоростью соединения.
  * <a href="https://drive.google.com/file/d/1iVqNdGf3OjvVkirkD4cOG0JYst06SHGc/view?usp=sharing">Скриншот</a> состояния GET запроса с настройками Throttle.
  * <a href="https://drive.google.com/file/d/14ZvSNy6H8Rn14TO9ZNFV7pQPW_7XZxnk/view?usp=sharing">Скриншот</a> состояния приложения при ошибке загрузки данных.
* Rewrite:
  * <a href="https://drive.google.com/file/d/1emFASg6HTVOz5gvgxRgwxz1AeGSBDway/view?usp=sharing">Скриншот</a> Rewrite настроек с подменой кода ответа сервера.
  * <a href="https://drive.google.com/file/d/1NoFNlaGWSpnbdlWqWoWv4KJgvKFmU4aw/view?usp=sharing">Скриншот</a> состояния GET запроса с настройками Rewrite.
  * <a href="https://drive.google.com/file/d/14aUR9OX-bC3aITyJo5REfRZZx08mg9TS/view?usp=sharing">Скриншот</a> состояния приложения при ошибке загрузки данных.
## Что было сделано
* Установлен и настроен [Charles](https://www.charlesproxy.com/).   
* Настроено android-устройство для отслеживания запросов в Charles.
* Установлено тестовое приложение **Гороскопы Mail.ru**-[Гороскопы в GooglePlay](https://play.google.com/store/apps/details?id=ru.mail.horo.android) на android-устройство.
  ### Задание 1
  * Созданы условия моделирования ошибки загрузки данных двумя способами:
      * Способ с использованием Throttle - конфигурация состояния сети:
        * Заданы настройки Throttle c нулевой скоростью загрузки\отдачи - <a href="https://drive.google.com/file/d/1vbiv4LvxTBWC_GJ_gljAXN3hZUI9-HW6/view?usp=sharing"> Скриншот</a> настроек.
        * Найдет GET запрос, от приложения, не имеющий ответа - <a href="https://drive.google.com/file/d/1iVqNdGf3OjvVkirkD4cOG0JYst06SHGc/view?usp=sharing">Скриншот</a> состояния GET запроса.
        * Зафиксировано отображение состояния приложения при ошибке загрузки данных - <a href="https://drive.google.com/file/d/14ZvSNy6H8Rn14TO9ZNFV7pQPW_7XZxnk/view?usp=sharing">Скриншот</a> приложения при ошибке.
  * Созданы условия моделирования ошибки загрузки данных двумя способами:
      * Способ с использованием Rewrite - подмена значения кода ответа:
        * Заданы настройки Rewrite c заменой кода ответа "200" на "500" - <a href="https://drive.google.com/file/d/1emFASg6HTVOz5gvgxRgwxz1AeGSBDway/view?usp=sharing">Скриншот</a> настроек.
        * Найдет GET запрос, от приложения с кодом ответа "500" - <a href="https://drive.google.com/file/d/1NoFNlaGWSpnbdlWqWoWv4KJgvKFmU4aw/view?usp=sharing">Скриншот</a> состояния GET запроса.
        * Зафиксировано отображение состояния приложения при ошибке загрузки данных - <a href="https://drive.google.com/file/d/14aUR9OX-bC3aITyJo5REfRZZx08mg9TS/view?usp=sharing">Скриншот</a> приложения при ошибке.

---
---



## Описание Задания 1 

Вам необходимо убедиться, что разработчики предусмотрели обработку ошибки загрузки данных на странице гороскопа на сегодняшний день и у любого из зодиаков.
Смоделируйте показ ошибки загрузки данных на странице.

**Результат выполнения задания:**

1. Скриншот необходимых для данной проверки настроек в Charles.
2. Скриншот данной ошибки в приложении.

