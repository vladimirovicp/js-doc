```
/**
 * Returns the result of concatenation of two strings.
 * Получи результат объединения двух строк
 *
 * @param {string} value1
 * @param {string} value2
 * @return {string}
 *
 * @example
 *   'aa', 'bb' => 'aabb'
 *   'aa',''    => 'aa'
 *   '',  'bb'  => 'bb'
 */
```

```javascript
function concatenateStrings(value1, value2) {
  throw new Error("Not implemented");
}
```

```javascript
return value1 + value2;
```

```javascript
return `${value1}${value2}`;
```

```javascript
return value1.concat(value2);
```

```
/**
 * Возвращает длину заданной строки.
 * Вывести длину заданной строки.
 *
 * @param {string} value
 * @return {number}
 *
 * @example
 *   'aaaaa' => 5
 *   'b'     => 1
 *   ''      => 0
 */
```

```javascript
function getStringLength(value) {}
```

```javascript
return value.length;
```

```
/**
 * Returns the result of string template and given parameters firstName and lastName.
 * Возвращает результат шаблона строки и заданных параметров firstName и lastName.
 * Please do not use concatenation, use template string :
 * Пожалуйста, не используйте конкатенацию, используйте шаблонные строки
 * https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/template_strings
 *
 * @param {string} firstName
 * @param {string} lastName
 * @return {string}
 *
 * @example
 *   'John','Doe'      => 'Hello, John Doe!'
 *   'Chuck','Norris'  => 'Hello, Chuck Norris!'
 */
```

```javascript
function getStringFromTemplate(firstName, lastName) {}
```

```javascript
return `Hello, ${firstName} ${lastName}!`;
```

```
/**
 * Extracts a name from template string 'Hello, First_Name Last_Name!'.
 * Извлеките имя из строки шаблона 'Hello, First_Name Last_Name!'.
 *
 * @param {string} value
 * @return {string}
 *
 * @example
 *   'Hello, John Doe!' => 'John Doe'
 *   'Hello, Chuck Norris!' => 'Chuck Norris'
 */
```

```javascript
function extractNameFromTemplate(value) {}
```

```javascript
return value.slice(7, -1);
```

```javascript
return value.replace(/Hello, /g, "").replace("!", "");
```

```
/**
 * Returns a first char of the given string.
 * Возвращает первый символ заданной строки.
 *
 * @param {string} value
 * @return {string}
 *
 * @example
 *   'John Doe'  => 'J'
 *   'cat'       => 'c'
 */
```

```javascript
function getFirstChar(value) {}
```

```javascript
return value[0];
```

```
/**
 * Removes a leading and trailing whitespace characters from string.
 *
 * @param {string} value
 * @return {string}
 *
 * @example
 *   '  Abracadabra'    => 'Abracadabra'
 *   'cat'              => 'cat'
 *   '\tHello, World! ' => 'Hello, World!'
 */
```

```javascript
function removeLeadingAndTrailingWhitespaces(value) {}
```

```javascript
return value.trim();
```

```
/**
 * Returns a string that repeated the specified number of times.
 *
 * @param {string} value
 * @param {string} count
 * @return {string}
 *
 * @example
 *   'A', 5  => 'AAAAA'
 *   'cat', 3 => 'catcatcat'
 */
```

```javascript
function repeatString(value, count) {}
```

```javascript
return value.repeat(count);
```

```
/**
 * Remove the first occurrence of string inside another string
 *
 * @param {string} str
 * @param {string} value
 * @return {string}
 *
 * @example
 *   'To be or not to be', 'not'  => 'To be or  to be'
 *   'I like legends', 'end' => 'I like legs',
 *   'ABABAB','BA' => 'ABAB'
 */
```

```javascript
function removeFirstOccurrences(str, value) {
  return str.replace(value, "");
}
```

```
/**
 * Remove the first and last angle brackets from tag string
 *
 * @param {string} str
 * @return {string}
 *
 * @example
 *   '<div>' => 'div'
 *   '<span>' => 'span'
 *   '<a>' => 'a'
 */
```

```javascript
function unbracketTag(str) {}
```

```javascript
return str.match(/<(.*?)>/)[1];
```

```javascript
return str.replace(/[<>]/g, "");
```

```javascript
return str.substring(1, str.length - 1);
```

```
/**
 * Converts all characters of the specified string into the upper case
 *
 * @param {string} str
 * @return {string}
 *
 * @example
 *   'Thunderstruck' => 'THUNDERSTRUCK'
 *  'abcdefghijklmnopqrstuvwxyz' => 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
 */
```

```javascript
function convertToUpperCase(str) {
  return str.toUpperCase();
}
```

```
/**
 * Extracts e-mails from single string with e-mails list delimeted by semicolons
 *
 * @param {string} str
 * @return {array}
 *
 * @example
 *   'angus.young@gmail.com;brian.johnson@hotmail.com;bon.scott@yahoo.com'
 *   => [
 *      'angus.young@gmail.com',
 *      'brian.johnson@hotmail.com',
 *      'bon.scott@yahoo.com'
 *   ],
 *   'info@gmail.com' => ['info@gmail.com']
 */
```

```javascript
function extractEmails(str) {}
```

```javascript
return str.split(";");
```

```
/**
 * Returns the string representation of rectangle with specified width and height
 * using pseudograhic chars
 *
 * @param {number} width
 * @param {number} height
 * @return {string}
 *
 * @example
 *
 *            '┌────┐\n'+
 *  (6,4) =>  '│    │\n'+
 *            '│    │\n'+
 *            '└────┘\n'
 *
 *  (2,2) =>  '┌┐\n'+
 *            '└┘\n'
 *
 *             '┌──────────┐\n'+
 *  (12,3) =>  '│          │\n'+
 *             '└──────────┘\n'
 *
 */
```

```javascript
function getRectangleString(width, height) {}
```

```javascript
const el = ["┌", "─", "┐", "│", "└", "┘"];
const top = `${el[0] + el[1].repeat(width - 2) + el[2]}\n`;
const centerLine = `${el[3] + " ".repeat(width - 2) + el[3]}\n`;
const center = centerLine.repeat(height - 2);
const bottom = `${el[4] + el[1].repeat(width - 2) + el[5]}\n`;
return top + center + bottom;
```

```javascript
const head = `┌${"─".repeat(width - 2)}┐\n`;
const middle = `│${" ".repeat(width - 2)}│\n`;
const foot = `└${"─".repeat(width - 2)}┘\n`;
return head + middle.repeat(height - 2) + foot;
```

```
/**
 * Encode specified string with ROT13 cipher
 * See details:  https://en.wikipedia.org/wiki/ROT13
 *
 * @param {string} str
 * @return {string}
 *
 * @example
 *
 *   'hello' => 'uryyb'
 *   'Why did the chicken cross the road?' => 'Jul qvq gur puvpxra pebff gur ebnq?'
 *   'Gb trg gb gur bgure fvqr!' => 'To get to the other side!'
 *   'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz'
 *    => 'NOPQRSTUVWXYZABCDEFGHIJKLMnopqrstuvwxyzabcdefghijklm'
 *
 */
```

```javascript
function encodeToRot13(str) {
  const input = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz";
  const output = "NOPQRSTUVWXYZABCDEFGHIJKLMnopqrstuvwxyzabcdefghijklm";
  const arr = str.split("");
  const result = arr.map((char) => {
    const index = input.indexOf(char);
    return index > -1 ? output[index] : char;
  });
  return result.join("");
}
```

```
/**
 * Returns true if the value is string; otherwise false.
 * @param {string} value
 * @return {boolean}
 *
 * @example
 *   isString() => false
 *   isString(null) => false
 *   isString([]) => false
 *   isString({}) => false
 *   isString('test') => true
 *   isString(new String('test')) => true
 */
```

```javascript
function isString(value) {
  return typeof value === "string" || value instanceof String;
}
```

```
/**
 * Returns playid card id.
 *
 * Playing cards inittial deck inclides the cards in the following order:
 * Игральные карты начальная колода раскладывает карты в следующем порядке:
 *
 *  'A♣','2♣','3♣','4♣','5♣','6♣','7♣','8♣','9♣','10♣','J♣','Q♣','K♣',
 *  'A♦','2♦','3♦','4♦','5♦','6♦','7♦','8♦','9♦','10♦','J♦','Q♦','K♦',
 *  'A♥','2♥','3♥','4♥','5♥','6♥','7♥','8♥','9♥','10♥','J♥','Q♥','K♥',
 *  'A♠','2♠','3♠','4♠','5♠','6♠','7♠','8♠','9♠','10♠','J♠','Q♠','K♠'
 *
 * (see https://en.wikipedia.org/wiki/Standard_52-card_deck)
 * Function returns the zero-based index of specified card in the initial deck above.
 * Функция возвращает основанный на нуле индекс указанной карты в исходной колоде выше.
 *
 * @param {string} value
 * @return {number}
 *
 * @example
 *   'A♣' => 0
 *   '2♣' => 1
 *   '3♣' => 2
 *     ...
 *   'Q♠' => 50
 *   'K♠' => 51
 */
```

```javascript
function getCardId(value) {
  const arr = [
    "A♣",
    "2♣",
    "3♣",
    "4♣",
    "5♣",
    "6♣",
    "7♣",
    "8♣",
    "9♣",
    "10♣",
    "J♣",
    "Q♣",
    "K♣",
    "A♦",
    "2♦",
    "3♦",
    "4♦",
    "5♦",
    "6♦",
    "7♦",
    "8♦",
    "9♦",
    "10♦",
    "J♦",
    "Q♦",
    "K♦",
    "A♥",
    "2♥",
    "3♥",
    "4♥",
    "5♥",
    "6♥",
    "7♥",
    "8♥",
    "9♥",
    "10♥",
    "J♥",
    "Q♥",
    "K♥",
    "A♠",
    "2♠",
    "3♠",
    "4♠",
    "5♠",
    "6♠",
    "7♠",
    "8♠",
    "9♠",
    "10♠",
    "J♠",
    "Q♠",
    "K♠",
  ];
  return arr.indexOf(value);
}
```
