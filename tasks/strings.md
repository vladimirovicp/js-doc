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
function getStringLength(value) {
  throw new Error("Not implemented");
}
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
