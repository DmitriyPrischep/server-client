### Задание 1.4
# Скользящий максимум

Дан массив целых чисел A[0..n), n не превосходит 100 000. Так же задан размер некотрого окна (последовательно расположенных элементов массива) в этом массиве k, k<=n. Требуется для каждого положения окна (от 0 и до n-k) вывести значение максимума в окне. Скорость работы O(n log n), память O(n).

## Формат ввода
Вначале вводится n - количество элементов массива. Затем вводится n строк со значением каждого элемента. Затем вводится k - размер окна.

## Формат вывода
Разделенные пробелом значения максимумов для каждого положения окна.

| Ввод  | Вывод |
| :---: | :-:   |
|  3    |   3   |
| 1 2 3 |       |
|  3    |       |