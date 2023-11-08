## Содержимое файла composer.json
```
{
    "name": "sancho/lrv-49",
    "description": "Домашнее задание по Composer",
    "type": "project",
    "require-dev": {
        "psr/log": "^3.0"
    },
    "license": "proprietary",
    "authors": [
        {
            "name": "Sancho Rodriges",
            "email": "softilla@ya.ru"
        }
    ],
    "minimum-stability": "stable",
    "require": {}
}
```

## Вопросы

### В чем разница между файлами composer.json и composer.lock ?

composer.json - это основной файл composer, в нём указывается информация о пакете и требуемые зависимости.
composer.lock содержит версии зависимостей, которые установлены на данный момент.

### В чем разница между директивами require-dev и require внутри файла composer.json?

в require указываются зависимости для проекта в продакшн версии, а в require-dev - зависимости, требуемые только на этапе разработки

### В чем разница между запуском команды composer install и composer update?

composer install установит конкретные версии библиотек, указанные в файле composer.lock
composer update будет обновлять библиотеки в проекте на самые последние версии, соответствующие требованиям в composer.json
