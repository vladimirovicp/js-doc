# js-doc

## Методы примитивов
## Number()
Объект Number является объектом-обёрткой, позволяющей вам работать с числовыми значениями. Объект Number создаётся через конструктор Number().
```js
let num = Number("123"); // превращает строку в число

new Number(value);
var a = new Number('123'); // a === 123 is false
var b = Number('123'); // b === 123 is true
a instanceof Number; // is true
b instanceof Number; // is false

Number("123"); // 123
Number(""); // 0
Number("0x11"); // 17
Number("0b11"); // 3
Number("0o11"); // 9
Number("foo"); // NaN
Number("100a"); // NaN
```

## toString()
Метод toString() возвращает строковое представление указанного объекта Number.
```js
var count = 10;

console.log(count.toString()); // Выведет '10'
console.log((17).toString()); // Выведет '17'

var x = 6;

console.log(x.toString(2)); // Выведет '110'
console.log((254).toString(16)); // Выведет 'fe'

console.log((-10).toString(2)); // Выведет '-1010'
console.log((-0xff).toString(2)); // Выведет '-11111111'
```


###  Math.max
возвращает наибольшее число из списка
```js
alert( Math.max(3, 5, 1) ); // 5

```
```js
let arr = [3, 5, 1];
alert( Math.max(arr) ); // NaN
```

```js
let arr = [3, 5, 1];
alert( Math.max(...arr) ); // 5 (оператор "раскрывает" массив в список аргументов)
```




## String

### splice

### split
Метод split() разбивает объект String на массив строк путём разделения строки указанной подстрокой.
```js
let str = "тест";
alert( str.split('') ); // т,е,с,т
```

### slice
Метод slice() извлекает часть строки и возвращает новую строку без изменения оригинальной строки.

```js
let str1 = "Приближается утро.";
let str2 = str1.slice(1, 8);
console.log(str2); // ВЫВОД: риближа
let str3 = str1.slice(4, -2);
console.log(str3); // ВЫВОД: лижается утр
let str4 = str1.slice(12);
console.log(str4); // ВЫВОД:  утро.
let str5 = str1.slice(30);
console.log(str5); // ВЫВОД: ""
```

### concat

### includes()
Метод includes() проверяет, содержит ли строка заданную подстроку, и возвращает, соответственно true или false.

```js
let str = "Быть или не быть вот в чём вопрос.";

console.log(str.includes("Быть")); // true
console.log(str.includes("вопрос")); // true
console.log(str.includes("несуществующий")); // false
console.log(str.includes("Быть", 1)); // false
console.log(str.includes("БЫТЬ")); // false
```

### replace()
Метод replace() возвращает новую строку с некоторыми или всеми сопоставлениями с шаблоном, заменёнными на заменитель. Шаблон может быть строкой или регулярным выражением, а заменитель может быть строкой или функцией, вызываемой при каждом сопоставлении.
```js
let re = /яблоки/gi;
let str = "Яблоки круглые и яблоки сочные.";
let newstr = str.replace(re, "апельсины");
console.log(newstr); // апельсины круглые и апельсины сочные.
```
```js

let s1 = 'aabcc';
s1 = s1.replace('a','');
console.log(s1); // abcc
s1 = s1.replace('a','1');
console.log(s1); // 1bcc


```



## Array

### push
добавляет элемент в конец.

### shift
удаляет элемент в начале, сдвигая очередь, так что второй элемент становится первым.
Удаляет из массива первый элемент и возвращает его.
```js
let fruits = ["Яблоко", "Апельсин", "Груша"];
alert( fruits.shift() ); // удаляем Яблоко и выводим его
alert( fruits ); // Апельсин, Груша
```

### unshift
Добавляет элемент в начало массива
```js
let fruits = ["Апельсин", "Груша"];
fruits.unshift('Яблоко');
alert( fruits ); // Яблоко, Апельсин, Груша
```


### pop
Удаляет последний элемент из массива и возвращает его
```js
let fruits = ["Яблоко", "Апельсин", "Груша"];
alert( fruits.pop() ); // удаляем "Груша" и выводим его
alert( fruits ); // Яблоко, Апельсин
```

### push
Добавляет элемент в конец массива:
```js
let fruits = ["Яблоко", "Апельсин"];
fruits.push("Груша");
alert( fruits ); // Яблоко, Апельсин, Груша
```





### join
```js
let arr = ['Вася', 'Петя', 'Маша'];
let str = arr.join(';'); // объединить массив в строку через ;
alert( str ); // Вася;Петя;Маша
```




