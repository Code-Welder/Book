## 2.1. Значение, идентификатор, переменная и константа, литерал, присвоение

> Значение (Value) — величина, записанная в определенное место памяти в определенном формате и представляющая данные, которым может манипулировать программа.

> Идентификатор (Identifier) — имена переменных, констант, функций, методов, аргументов, классов, как внутренние, так и импортированные из других модулей и глобальные.

```js
const INTERVAL = 500;
let counter = 0;
const MAX_VALUE = 10;
let timer = null;

const event = () => {
  if (counter === MAX_VALUE) {
    console.log('The end');
    clearInterval(timer);
    return;
  }
  console.dir({ counter, date: new Date() });
  counter++;
};

console.log('Begin');
timer = setInterval(event, INTERVAL);
```

> Переменная (Variable) — именованная область памяти (идентификатор), имеющая тип данных, адрес и значение.

Мы можем менять значение переменной в отличие от константы (а для некоторых языков и тип):

```js
let cityName = 'Beijing';
```

> Константа (Constant) — идентификатор, с которым связано неизменяемое значение и тип

```js
const WATCH_TIMEOUT = 5000;
```

```js
// Constants

const SALUTATION = 'Ave';

const COLORS = [
  /* 0 */ 'black',
  /* 1 */ 'red',
  /* 2 */ 'green',
  /* 3 */ 'yellow',
  /* 4 */ 'blue',
  /* 5 */ 'magenta',
  /* 6 */ 'cyan',
  /* 7 */ 'white',
];
```

> Литерал (Literal) — запись значения в коде программы.

Например: литералы чисел, логических значений, null и undefined, строк, массивов, объектов, функций. Литералы могут иметь различный синтаксис, от очень простого, для записи чисел, до сложных синтаксических конструкций, для записи объектов.

> Присвоение (Assignment) — связывания значения и идентификатора (например переменной).

Операция присвоения во многих языках возвращает присваиваемое значение (имеет поведение выражения).
