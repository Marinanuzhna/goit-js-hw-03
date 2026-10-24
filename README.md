# goit-js-hw-03
Задача 1. Генератор slug

Виконуй це завдання у файлі task-1.js


Перш ніж розв'язувати задачу, розберемось із новим терміном.



Slug — це зрозумілий людині унікальний ідентифікатор, який використовується у веброзробці для створення читабельних URL-адрес.



Наприклад, замість того, щоб користувач побачив в адресному рядку mysite.com/posts/1q8fh74tx, можна зробити slug із назви статті: mysite.com/posts/arrays-for-beginners.



Slug — це завжди рядок у нижньому регістрі, слова якого розділені тире.



Оголоси функцію slugify, яка очікує один параметр title — заголовок статті. Функція повертає slug, створений із цього рядка.

Значенням параметра title будуть рядки, слова яких розділені лише пробілами.
Усі символи slug повинні бути в нижньому регістрі.
Усі слова slug повинні бути розділені тире.


Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її роботи.

console.log(slugify("Arrays for beginners")); // "arrays-for-beginners"
console.log(slugify("English for developer")); // "english-for-developer"
console.log(slugify("Ten secrets of JavaScript")); // "ten-secrets-of-javascript"
console.log(slugify("How to become a JUNIOR developer in TWO WEEKS")); // "how-to-become-a-junior-developer-in-two-weeks"

Залиш цей код для перевірки ментором.



Вимоги

Оголошено функцію slugify(title).
Виклик slugify("Arrays for beginners") повертає "arrays-for-beginners".
Виклик slugify("English for developer") повертає "english-for-developer".
Виклик slugify("Ten secrets of JavaScript") повертає "ten-secrets-of-javascript".
Виклик slugify("How to become a JUNIOR developer in TWO WEEKS") повертає "how-to-become-a-junior-developer-in-two-weeks".
Виклик з будь-якими валідними аргументами повертає правильне значення.
Результати всіх викликів виведено в консоль.


Задача 2. Композиція масивів

Виконуй це завдання у файлі task-2.js


Оголоси функцію makeArray, яка очікує три параметри:

firstArray — масив
secondArray — масив
maxLength — максимальна довжина результату


Функція створює новий масив, який містить спочатку всі елементи з firstArray, а потім усі елементи з secondArray.

Якщо кількість елементів у новому масиві перевищує maxLength, функція повертає копію масиву довжиною maxLength елементів.
В іншому випадку функція повертає весь новий масив.


Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її роботи.

console.log(makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3)); // ["Mango", "Poly", "Ajax"]
console.log(makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4)); // ["Mango", "Poly", "Houston", "Ajax"]
console.log(makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3)); // ["Mango", "Ajax", "Chelsea"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2)); // ["Earth", "Jupiter"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4)); // ["Earth", "Jupiter", "Neptune", "Uranus"]
console.log(makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0)); // []

Залиш цей код для перевірки ментором.



Вимоги

Оголошено функцію makeArray(firstArray, secondArray, maxLength).
Виклик makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3) повертає ["Mango", "Poly", "Ajax"].
Виклик makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4) повертає ["Mango", "Poly", "Houston", "Ajax"].
Виклик makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3) повертає ["Mango", "Ajax", "Chelsea"].
Виклик makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2) повертає ["Earth", "Jupiter"].
Виклик makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4) повертає ["Earth", "Jupiter", "Neptune", "Uranus"].
Виклик makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0) повертає [].
Виклик з будь-якими валідними аргументами повертає правильний масив.
Результати всіх викликів виведено в консоль.


Задача 3. Фільтрація масиву чисел

Виконуй це завдання у файлі task-3.js


Оголоси функцію filterArray, яка очікує два параметри:

numbers — масив чисел
value — порогове значення
Функція повертає новий масив, що містить лише ті числа з numbers, які більші за value.



Усередині функції:

Створи порожній масив, у який будеш додавати підходящі числа.
Використай цикл для ітерації кожного елемента масиву numbers.
Використай умовний оператор if усередині циклу для перевірки кожного елемента і додавання до свого масиву.
Поверни свій новий масив з підходящими числами як результат.


Візьми код нижче і встав після оголошення своєї функції для перевірки коректності її роботи. У консоль будуть виведені результати її роботи.

console.log(filterArray([1, 2, 3, 4, 5], 3)); // [4, 5]
console.log(filterArray([1, 2, 3, 4, 5], 4)); // [5]
console.log(filterArray([1, 2, 3, 4, 5], 5)); // []
console.log(filterArray([12, 24, 8, 41, 76], 38)); // [41, 76]
console.log(filterArray([12, 24, 8, 41, 76], 20)); // [24, 41, 76]



Залиш цей код для перевірки ментором.



Вимоги

Оголошено функцію filterArray(numbers, value).
Виклик filterArray([1, 2, 3, 4, 5], 3) повертає [4, 5].
Виклик filterArray([1, 2, 3, 4, 5], 4) повертає [5].
Виклик filterArray([1, 2, 3, 4, 5], 5) повертає [].
Виклик filterArray([12, 24, 8, 41, 76], 38) повертає [41, 76].
Виклик filterArray([12, 24, 8, 41, 76], 20) повертає [24, 41, 76].
Виклик з будь-якими валідними аргументами повертає правильний масив.
Результати всіх викликів виведено в консоль.