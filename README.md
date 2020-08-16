# 1. Фигурные скобки #

- Плохой код

😠 Никогда не разделяйте строки без фигурных скобок, можно ненароком сделать ошибку при добавлении строк:

`if (n < 0)`

`alert('Степень' + ' ' + n + 'не поддерживается');`

- Хороший код

😃 При разделении строк использовать фигурные строки

`if (n < 0) {`  

  `alert('Степень' + ' ' + n + 'не поддерживается');}`

# 2. Длина строки #

- Плохой код

😠 Не пишите длинные горизонтальные строки кода

- Хороший код

😃 Разделяйте горизонтальные строки кода

`let str =  
'Рабочая группа TC39 организации Ecma International -   
это группа JavaScript-разработчиков, теоретиков и авторов движков JavaScript,    
которые вместе с сообществом занимаются поддержкой и развитием языка JavaScript.'`

# 3. Создание объекта #

-Плохой код

😠 Не создавайте объекты через конструктор new Object.

`let item = new Object();`

-Хороший код

😃 Для создания объекта используйте фигурные скобки.

`let item = {};`

# 4. Создание массивы #

-Плохой код

😠 Не создавайте массивы через конструктор new Array.

`let items = new Array();`

-Хороший код

😃 Для создания массива используйте квадратные скобки.

`let items = [];`

# 5. Создание строки #

-Плохой код

😠 Двойные кавычки расходуют большее количество памяти

`let name = "Боб Дилан"`

-Хороший код

😃  Используйте одинарные кавычки для строк

`let name = 'Боб Дилан'`

# 6. Объявления функций #

-Плохой код

😠 Никогда не объявляйте функцию внутри блока кода - например в if, else, while и так далее.

Единственное исключение - блок функции.

`if  (currentUser) {
  function test() {
    console.log('Плохой мальчик.');
  }
}`

- Хороший код

😃 Вместо этого присваивайте функцию уже объявленной через let переменной.

Условное объявление функций работает, но в различных браузерах работает по-разному.

`let test;`

`if (currentUser) {
  test = function test() {
    console.log('Молодец.');
  };
}`

# 7. Использование аргументов в функции #

- Плохой код

😠 Никогда не используйте аргумент функции arguments, он будет более приоритетным над объектом arguments, который доступен без объявления для каждой функции.

`function nope(name, options, arguments) {`

  `// ...код...`

`}`

- Хороший код

😃

`function yup(name, options, args) {`

  `// ...код...`

`}`

# 8. Доступ к свойствам и методам #

- Плохой код

😠

`let isJedi = luke['jedi'];`

-Хороший код

😃 Используйте точечную нотацию для доступа к свойствам и методам.

`let isJedi = luke.jedi;`

# 9. Объявление переменных #

- Плохой код

😠

`let i, len, dragonball,
    items = getItems(),
    goSportsTeam = true;`

-Хороший код

😃 Объявляйте переменные, которым не присваивается значение, в конце, а также каждую переменную с новой строки.

Это удобно, когда вам необходимо задать значение одной из этих переменных на базе уже присвоенных значений.

`let items = getItems(),
    goSportsTeam = true,
    dragonball,
    length,
    i;`

# 10. Условные выражения и равенства #

- Плохой код

😠

`if (name !== '') {`

  `// ...код...`

`}`

-Хороший код

😃Используйте короткий синтаксис.

`if (name) {`

  `// ...код...`

`}`
