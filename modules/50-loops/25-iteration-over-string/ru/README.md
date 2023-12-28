
С помощью циклов не только обрабатывают числа, но работают и со строками. Например, можно получить конкретный символ по его индексу, а также формировать строки в циклах.

Ниже пример кода, который печатает буквы каждого слова на отдельной строке:

```python
def print_name_by_symbol(name):
    i = 0
    # Такая проверка будет выполняться до конца строки,
    # включая последний символ. Его индекс `length - 1`.
    while i < len(name):
        # Обращаемся к символу по индексу
        print(name[i])
        i = i + 1

name = 'Arya'
print_name_by_symbol(name)
# => 'A'
# => 'r'
# => 'y'
# => 'a'
```

https://replit.com/@hexlet/python-basics-loops-iteration-over-string

Главное в этом коде — поставить правильное условие в `while`. Это можно сделать двумя способами: `i < len(name)` или `i <= len(name) - 1` — они приведут к одному результату.