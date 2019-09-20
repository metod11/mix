## Тестирование NiederreiterBaseTwo генератора (t,m,s)-сетки

Для сборки проекта необходимо выполнить команду:

    make
    
Для запуска необходимо выполнить команду:

    main

Результаты теста будут выведены в консоль. Виды тестов:
* Покомпонентная уникальность 

| Название генератора | Успешное прохождение теста на размерностях |
|-------------------- | ------------------------------------------ |
| Генератор последовательностей Соболя | 2 - 24 |
| Генератор сеток Нидеррайтера по основанию b = 2 | 2 - 24 |

* Линейный коэффициент корреляции Пирсона - протестировано от 2 до 24 размерности

| Название генератора | Успешное прохождение теста на размерностях |
|-------------------- | ------------------------------------------ |
| Генератор последовательностей Соболя | 2 - 24 |
| Генератор сеток Нидеррайтера по основанию b = 2 | 2 - 24 |

* Тестирование сеток на дефект(значения в таблицах соответствует тройке (t, m, s)):

Генератор последовательностей Соболя

| m\s | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  0  | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
|  1  | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
|  2  | 0 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 |
|  3  | 0 | 0 | 1 | 2 | 2 | 2 | 2 | 2 | 2 | 2 |
|  4  | 0 | 0 | 1 | 2 | 2 | 3 | 3 | 3 | 3 | 3 |
|  5  | 0 | 0 | 1 | 2 | 2 | 2 | 2 | 3 | 3 | 3 |
|  6  | 0 | 0 | 1 | 2 | 3 | 3 | 3 | 4 | 4 | 4 |
|  7  | 0 | 0 | 1 | 2 | 3 | 3 | 3 | 4 | 4 | 4 |
|  8  | 0 | 0 | 1 | 2 | 3 | 4 | 4 | 4 | 5 | 5 |
|  9  | 0 | 0 | 1 | 2 | 3 | 4 | 5 | 5 | 5 | 6 |
|  10 | 0 | 0 | 1 | 2 | 3 | 4 | 5 | 5 | 6 | 6 |

Генератор сеток Нидеррайтера по основанию b = 2

| m\s | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  0  | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
|  1  | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
|  2  | 0 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 |
|  3  | 0 | 0 | 1 | 2 | 2 | 2 | 2 | 2 | 2 | 2 |
|  4  | 0 | 0 | 1 | 1 | 3 | 3 | 3 | 3 | 3 | 3 |
|  5  | 0 | 0 | 1 | 2 | 2 | 3 | 4 | 4 | 4 | 4 |
|  6  | 0 | 0 | 1 | 3 | 3 | 3 | 4 | 4 | 5 | 5 |
|  7  | 0 | 0 | 1 | 3 | 3 | 3 | 4 | 4 | 6 | 6 |
|  8  | 0 | 0 | 1 | 2 | 3 | 4 | 5 | 5 | 7 | 7 |
|  9  | 0 | 0 | 1 | 3 | 3 | 3 | 5 | 6 | 6 | 6 |
|  10 | 0 | 0 | 1 | 2 | 4 | 4 | 6 | 7 | 7 | 7 |