# Компонент "Выгрузка пользователей в Excel"

## Описание
Компонент позволяет выгружать данные пользователей из таблицы `b_user` Bitrix в Excel-файл (.xlsx). Пользователь может фильтровать данные по дате регистрации и по наличию заполненного телефона.

## Требования
- Bitrix с поддержкой D7 (Data Management Layer)
- PHP с установленными расширениями: xml, gd, phar.
- Composer с установленной библиотекой PhpSpreadsheet

## Установка
1. Скопируйте компонент в директорию `/local/`, созданную в корне сайта.
2. Убедитесь, что в корне сайта есть файл `composer.json` с зависимостью:
    ```json
    {
        "require": {
            "phpoffice/phpspreadsheet": "^1.23"
        }
    }
    ```
3. В корневой директории с файлом composer.json выполните:
    
    ```bash
    composer install
    ```
4. Установка библиотек для работы с excel
     ```bash
    composer require phpoffice/phpspreadsheet
    ```

## Использование
Перейдите на страницу: http://your-site/local/admin/export_users.php
Заполните фильтры, нажмите "Выгрузить в Excel" и скачайте файл.# bitrix-weather-widget
