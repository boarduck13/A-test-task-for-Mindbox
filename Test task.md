Для решения задачи мы можем использовать две техники: граничные значения и классы эквивалентности.

### 1. Граничные значения

Граничные значения — это значения, которые находятся на границах допустимого диапазона, а также значения, которые находятся сразу за пределами этого диапазона. В данном случае диапазон значений от 0 до 115 включает в себя:

- Минимальное значение: 0
- Максимальное значение: 115
- Значения ниже минимума: -1
- Значения выше максимума: 116

Таким образом, граничные значения будут следующими:

| Входное значение | Ожидаемый результат       |
|——————|—————————|
| -1               | Ошибка                    |
| 0                | Можно оформить            |
| 1                | Можно оформить            |
| 114              | Можно оформить            |
| 115              | Можно оформить            |
| 116              | Ошибка                    |

### 2. Классы эквивалентности

Классы эквивалентности — это группы значений, которые обрабатываются одинаково. В данном случае можно выделить следующие классы:

1. Класс значений ниже допустимого диапазона: значения < 0.
   - Пример: -1
   - Результат: Ошибка

2. Класс значений в пределах допустимого диапазона: значения от 0 до 115.
   - Пример: 0 (можно оформить), 1 (можно оформить), 50 (можно оформить), 115 (можно оформить)
   - Результат: Можно оформить

3. Класс значений выше допустимого диапазона: значения > 115.
   - Пример: 116
   - Результат: Ошибка

Таким образом, примеры входных значений и результаты для каждого класса эквивалентности:

| Класс эквивалентности               | Пример входного значения | Ожидаемый результат       |
|————————————-|————————–|—————————|
| Значения < 0                        | -1                       | Ошибка                    |
| Значения от 0 до 115                | 0                        | Можно оформить            |
|                                     | 1                        | Можно оформить            |
|                                     | 50                       | Можно оформить            |
|                                     | 115                      | Можно оформить            |
| Значения > 115                      | 116                      | Ошибка                    |

