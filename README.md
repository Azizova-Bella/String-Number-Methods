# String-Number-Methods

# Методы String и Number в JavaScript
![Watch this video](https://youtu.be/nQ5Ms1WqNa4?si=aVRZS4hGoQVhDEYV)

## Методы String
**String** — это объект, представляющий текст. JavaScript предоставляет множество методов для работы со строками. ✍️
(![image](https://github.com/user-attachments/assets/e284445b-5826-41a0-a6d2-177d18d0375e)
)

### Методы для манипуляции строками
1. **`concat(string)`**: Соединяет строки. ➕
   ```javascript
   const text1 = "Привет";
   const text2 = "мир";
   console.log(text1.concat(", ", text2)); // Привет, мир
   ```
### Свойства строк
2.- **`length`**: Возвращает длину строки. 🧮
  ```javascript
  const text = "Привет, мир!";
  console.log(text.length); // 12
  ```

3. **`charAt(index)`**: Возвращает символ по указанному индексу. 🅰️
   ```javascript
   const text = "Hello";
   console.log(text.charAt(1)); //for finding letter in index
   ```

4. **`at(index)`**: Возвращает символ по указанному индексу б работает как charAt но с минусом(-). 🅰️
   ```javascript
   const text = "Hello";
   console.log(text.charAt(1)); //for finding letter in index
   ```

### Методы для удаления пробелов
5.- **`trim()`**: Удаляет пробелы в начале и конце строки. ✂️
  ```javascript
  const text = "   Привет   ";
  console.log(text.trim()); // Привет
  ```

### Методы для работы с содержимым строки
6. **`split(delimiter)`**: Разделяет строку на массив по заданному разделителю  считается как search (🔍). 📚
   ```javascript
   const text = "seb, shaftollu, banan";
   console.log(text.split(", ")); // ["seb", "shaftollu", "banan"]
   ```

7. **`replace(kuhna, nav)`**: Заменяет указанную подстроку на новую. 🔄
   ```javascript
   const text = "Привет, JavaScript!";
   console.log(text.replace("JavaScript", "Мир")); 
   ```
8. **`replaceAll(kuhna, nav)`**: Заменяет указанную подстроку на новую,ту у которых одинаковое имя то всеи изменяет. 🔄
   ```javascript
   const text = "Привет, JavaScript!";
   console.log(text.replace("JavaScript", "Мир")); 
   ```

9. **`includes(substring)`**: Проверяет, содержит ли строка указанную подстроку. 🔍
   ```javascript
   const text = "Привет, мир!";
   console.log(text.includes("мир")); // true
   ```

10. **`substring(sarshavi, tamomshavi)`**: Возвращает подстроку с указанными индексами. ✂️
   ```javascript
   const text = "JavaScript";
   console.log(text.substring(0, 4));
   ```
11. **`slice (sarshavi, tamomshavi)`**: Возвращает подстроку с указанными индексами , но плюс в том что принимает и минусавые значение. ✂️
   ```javascript
   const text = "JavaScript";
   console.log(text.substring(0, 4));
   ```

12. **`toLowerCase()`**: Преобразует строку в нижний регистр. 🔡
   ```javascript
   const text = "Привет, Мир!";
   console.log(text.toLowerCase()); // привет, мир!
   ```

13. **`toUpperCase()`**: Преобразует строку в верхний регистр. 🔠
   ```javascript
   const text = "Привет, Мир!";
   console.log(text.toUpperCase()); // ПРИВЕТ, МИР!
   ```

14. **`indexOf(substring)`**: Возвращает индекс первого вхождения подстроки. Если подстрока не найдена, возвращает -1. 🔢
   ```javascript
   const text = "JavaScript";
   console.log(text.indexOf("Script")); // 4
   ```

15. **`lastIndexOf(substring)`**: Возвращает индекс последнего вхождения подстроки. 🔙
   ```javascript
   const text = "JavaScript is great. I love JavaScript!";
   console.log(text.lastIndexOf("JavaScript")); // 26
   ```

16. **`repeat(count)`**: Повторяет строку указанное количество раз. 🔁
   ```javascript
   const text = "ha";
   console.log(text.repeat(3)); // hahaha
   ```

---

## Методы Number

**Number** — это объект для работы с числами. JavaScript предоставляет методы для обработки чисел. 🔢


![image](https://github.com/user-attachments/assets/037204b2-ccec-4ac0-a862-2d8f4de2026b)



### Свойства и преобразования чисел

### Проверка чисел
1. **`isNaN(value)`**: Проверяет, является ли значение NaN (не числом). ❓
   ```javascript
   console.log(isNaN("abc")); // true
   ```
2. **`Number.isInteger(value)`**: Проверяет, является ли значение целым числом. ✔️
   ```javascript
   console.log(Number.isInteger(10)); // true
   console.log(Number.isInteger(10.5)); // false  // booling znacheniya meta auto 
   ```

### Математические операции
3. **`Math.round(number)`**: Округляет число до ближайшего целого. 🔘
   ```javascript
   console.log(Math.round(4.5)); // 5
   ```

4. **`Math.floor(number)`**: Округляет число вниз. ⬇️
   ```javascript
   console.log(Math.floor(4.7)); // 4
   ```

5. **`Math.ceil(number)`**: Округляет число вверх. ⬆️
   ```javascript
   console.log(Math.ceil(4.1)); // 5
   ```

6. **`Math.abs(number)`**: Возвращает модуль числа. ➕
   ```javascript
   console.log(Math.abs(-5)); // 5
   ```

7. **`Math.sqrt(number)`**: Возвращает квадратный корень числа. ✖️
   ```javascript
   console.log(Math.sqrt(16)); // 4
   ```

8. **`Math.pow(base, exponent)`**: Возводит число в степень. 🔺
   ```javascript
   console.log(Math.pow(2, 3)); // 8
   ```

9. **`Math.random()`**: Возвращает случайное число от 0 до 1. 🎲
   ```javascript
   console.log(Math.random()); // Например, 0.8374
   ```

10. **`Math.max(a, b, ...)`**: Возвращает наибольшее число. ⬆️
   ```javascript
   console.log(Math.max(1, 5, 10)); // 10
   ```

11. **`Math.min(a, b, ...)`**: Возвращает наименьшее число. ⬇️
   ```javascript
   console.log(Math.min(1, 5, 10)); // 1
   ```


