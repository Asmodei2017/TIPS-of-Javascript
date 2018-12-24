## Особенности и нюансы языка JavaScript

> **НАХОДИТЕ ПОДОБНЫЕ ШТУКИ И ДОБАВЛЯЙТЕ СЮДА**

#### Типы данных 

#####  Стандарт ECMAScript определяет 7 типов данных

- 6 типов данных являются ПРИМИТИВАМИ:
  - `Number` (Число)
  
  - `String` (Строка)
  
  - `Boolean `(Булев, Логический тип TRUE/FALSE)
 
  - `Null` (Null, ссылка на пустое, не существующее )
 
  - `Undefined` (значение НЕ ОПРЕДЕЛЕНО)
 
  - `Symbol` (ES6 читаем)[http://haa.su/EUG/]

- 7  `Object` (Объекы/Массивы/Функции/JSON) 

#### При сравнении, JS приводит типы к логическому значению

###### список того, что приведется к `false`
 - `Nan`
 - `null`
 - `undefined`
 - `false`
 - `" " пустая стока`
 - `0 `

#### При преобразовании к числу методом унарного оператора +

- `строка` при преобразовании к числу `+строка` вернет `NaN`

- ` true ` при преобразовании к числу `+true` вернет `число 1`

-  ` undefined ` при преобразовании к числу `+undefined` вернет `NaN`

-  ` NaN ` при преобразовании к числу `+NaN` вернет `NaN`

-  ` Null ` при преобразовании к числу `+Null` вернет  `число 0`

#### Приоритет операторов и порядок их выполнения

 | Приор  |  Тип оператора |  Порядок   вып. |Оператор   |
| ------------ | ------------ | ------------ | ------------ |
| 20  |Группировка   |  не определено |  …  |
|  19 |  Доступ к свойствам |  слева направо | . |
|   |  Доступ к свойствам с возможностью вычисления | слева направо |  [ … ] |
|   | new (со списком аргументов)  | неопределено  |  new … ( … ) |
|   | Вызов функции  | слева направо  |  ( … ) |
|  18 |	new (без списка аргументов)   | справа налево  | new …  |
| 17  | Постфиксный инкремент  |   | ... ++  |
|   |  Постфиксный декремент |   |  ... - -  |
|  16 | Логическое отрицание  | справа налево  |  ! |
|   | Побитовое отрицание  |   |  ~ |
|   |Унарный плюс   |   |  + |
|   | Унарный минус  |   |  - |
|   | Префиксный инкремент  |   | ++ ...  |
|   | Префиксный декремент  |   |  - - ...   |
|   |  typeof|   | typeof …  |
|   | void  |   | void …  |
|   |  delete |   |  delete … |
|   |   await|   | await …  |
| 15  | Возведение в степень  | справа налево  |   * *  |
|  14 | Умножение  |   | *  | 
|   | Деление  |   | /  |
|   | Остаток  |   |  % |
| 13  |  Сложение |  слева направо | +  |
|   |  Вычитание |   |  - |
| 12  | Побитовый сдвиг влево  |   | <<  |
|   | Побитовый сдвиг вправо  |   | >>  |
|   |  Сдвиг вправо с заполнением нулей |   |  >>> |
|   |   |   |   |
|   |   |   |   |





#### Нюансы JAVASCRIPT

- При сложении со строкой будет всегда строка. EX: ` 5 + '7' = '57'`
 
- строки сравниваются по номеру индекса `UNICODа`

- Оператор `&&` выполняется слева направо и должены быть ВСЕ` true` , если хоть один будет `false` то вернет `false`

- Оператор `||` вернет `true` если хотябы одно из условий будет `true`

- Одинаковые массивы НЕ БУДУТ `===`равны друг другу так как они хранятся в разных ячейках памяти

- часть строки нельзя изменить, можно поменять на новую

- `НАСТОЯЩИЕ ЧИСЛА` - это `целое` и `дробное` число (0-9, 2.5) и `infinity`

- `0.1 + 0.2 == 0.3`  ВЕРНЕТ `FALSE`  пояснение (https://is.gd/Lpz4vq) 

- `typeof null ` вернет `Object`



#### Необъяснимо НО факт 

- `typeOf NaN` -=> `"number"`

- `9999999999999999` -=> `10000000000000000`

- `9 + "1"` -=> `"91"`

- `91 - "1"` -=> `90`

- `0.5 + 0.1 == 0.6` -=> `true`

- `0.1 + 0.2 == 0.3` -=> `false`

- `Math.max()` -=> `-Infinity`

- `Math.min()` -=> `Infinity`

- `[] == 0` -=> `true`

- `[] == []` -=> `false`

- `[] + []` -=> `" "`

- `[] + {}` -=> `" [object Object] "`

- `{} + []` -=> `0`

- `true + true + true === 3` -=> `true`

- `true-true` -=> `0`

- `true == 1` -=> `true`

- `true === 1` -=> `false`

- `(!+[]+[]+![]).length` -=> `9`

## Стрелочные функции
- объявляются и назначаются ТОЛЬКО переменным FunctionExpression
- если параметр 1, то можно передавать без скобок
- если в блоке кода одна команда, то можно писать без фигурных скобок
- если параметров нет, то обязательно должны быть пустые круглые скобки
- нет локальной переменной arguments содержащей все аргументы
- если необходимо собрать все аргументы в коллекцию используйте опертор rest.
- this в использовании внутри тела функции ВСЕГДА будет обращаться к глобальному контексту (ducument)






