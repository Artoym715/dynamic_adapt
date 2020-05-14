# Динамический адаптив (Dynamic Adapt)
JS функция для комфортной адаптивной верстки. Позволяет "перебрасывать" объекты DOM в зависимости от потребностей.

## Применение.
Для перещаемого объекта пишем HTML атрибут - `data-da` и указываем параметры 

## Параметры

`data-da="куда,какой,когда"`

Название | Значение по-умолчанию | Описание
------------- | ------------- | ------------- 
`куда (имя класса)` | _\[обязательный\]_ | Класс блока, в который нужно будет "перебросить" текущий объект. Если класс не уникален, объек перебросится в первый элемент с этим классом.
`какой` | last | Позиция на которую нужно переместить объект внутри родителя `куда`. Кроме цифр можно указать слова first (в начало блока) или last (в конец блока)
`когда` | 767 | Брейкпоинт при котором перемещать объект.

## Примеры

```html
<div data-da="content__column_garden" class="content__block">Я Коля
<div data-da="content__column_garden,2" class="content__block">Я Коля
<div data-da="content__column_garden,2,992" class="content__block">Я Коля
```

## Подробнее
https://www.youtube.com/watch?v=QKuMr575vlQ

## Спасибо за идеи и предложения
last и first - идея Mark.
Параметры по умолчанию - идея mubat (https://github.com/mubat)
