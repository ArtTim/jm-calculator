<details>
<summary>Задача: “Калькулятор”</summary>

### Описание:
Создайте консольное приложение “Калькулятор”. Приложение должно читать из консоли введенные пользователем арифметические операции и выводить в консоль результат их выполнения.

### Требования:
1. Калькулятор умеет выполнять операции сложения, вычитания, умножения и деления с двумя числами: a + b, a - b, a * b, a / b. Данные передаются в одну строку (смотрите пример)! Решения, в которых каждое число и арифмитеческая операция передаются с новой строки считаются неверными.
2. Калькулятор умеет работать как с арабскими (1,2,3,4,5…), так и с римскими (I,II,III,IV,V…) числами.
3. Калькулятор должен принимать на вход числа от 1 до 10 включительно, не более. На выходе числа не ограничиваются по величине и могут быть любыми.
4. Калькулятор умеет работать только с целыми числами.
5. Калькулятор умеет работать только с арабскими или римскими цифрами одновременно, при вводе пользователем строки вроде 3 + II калькулятор должен выбросить исключение и прекратить свою работу.
6. При вводе римских чисел, ответ должен быть выведен римскими цифрами, соответственно, при вводе арабских - ответ ожидается арабскими.
7. При вводе пользователем неподходящих чисел приложение выбрасывает исключение и завершает свою работу.
8. При вводе пользователем строки, не соответствующей одной из вышеописанных арифметических операций, приложение выбрасывает исключение и завершает свою работу.
#### Пример работы программы:
```
Input:
1 + 2
Output:
3
Input:
VI / III
Output:
II
```

</details>

### Описание структуры проекта
Проект разбит на три пакета:
1. main. Здесь находится основной класс main
2. calc. Здесь происходят математические операции с введённой строкой
3. treatment. Здесь всё что связано с обработкой строки:
    - Request. Ввод строки и её разбор на переменные;
    - CheckNum. Проверка строки на соответствие требованиям ТЗ (арабские или римские числа, больше 0 и меньше 11);
    - Convertation. Перевод римских чисел в арабские и обратно.