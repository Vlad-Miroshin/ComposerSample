# Модуль 57. Контейнеры и Docker. Практические задачи (HW-04)
Модуль 57. Практические задачи (HW-04) <a href="https://skillfactory.ru/">Skillfactory</a><br> 
Выполнил студент <a href="https://github.com/Vlad-Miroshin">Владислав Мирошин</a> поток PHPPRO_22 

## Формулировка задания

Соберите площадку для разработки на базе Docker. Площадка должна иметь отдельные контейнеры под Nginx, PHP-FPM и MySQL. 

## Реализованные требования

- Сайт отвечает на имя application.local, его можно вызвать из браузера.
- При вызове сайт выводит на экран приветствие на ваше усмотрение.
- Контейнеры должны быть сконфигурированы при помощи docker-compos и отдельных Dockerfile.
- Настроен проброс директорий с кодом.
- Реализована возможность передавать в контейнер пользовательский php.ini. Например, если потребуется включить показ ошибок. 
- Конфигурация переписана так, чтобы можно было передавать кастомный my.cnf при сборке.

## Дополнително

- В сборку добавлен phpMyAdmin с переназначением портов, чтобы не конфликтовать с nginx (доступен по адресу http://application.local:8181)
- К решению прилагаются скриншоты страницы phpinfo, подключения к mysql снаружи (dbeaver), и изнутри (phpMyAdmin)

## Как запустить

- убедиться, что на хосте свободны порты 80, 443, 3306, 8181
- выполнить команду:

```
docker compose up --build
```
