## Особенности и нюансы языка JavaScript

> **НАХОДИТЕ ПОДОБНЫЕ ШТУКИ И ДОБАВЛЯЙТЕ СЮДА**

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






