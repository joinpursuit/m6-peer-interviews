# This is the List of All Trivia Questions and where they are being used

|                                                      Question                                                      |  Associated Lesson   |
| :----------------------------------------------------------------------------------------------------------------: | :------------------: |
|                           What is the difference between an parameter and and argument?                            |     Control Flow     |
|                              What is the difference between `var`, `const`, and `let`                              |     Control Flow     |
|                   Within a function, what is the difference between `return` and `console.log()`                   |     Control Flow     |
|                                What is the difference between `=`, `==`, and `===`                                 |         Math         |
|                                                   What is `NaN`?                                                   |         Math         |
|                                        Is `NaN == NaN` true or false, why?                                         |         Math         |
|                          Is `'McDonalds' > 'Burger King' - true, false or an error? Why?                           |   Strings & RegEx    |
|             What are the differences between a single quote, double quote, smart quote, and backtick?              |   Strings & RegEx    |
|                              What is the difference between a and 'a' in JavaScript?                               |   Strings & Regex    |
|                  What is the difference between a function declaration and a function expression?                  |        Errors        |
|                    What is one difference between an arrow function and a function declaration?                    |        Errors        |
|                                Can a function expression be an anonymous function?                                 |        Errors        |
|                                Can a function declaration be an anonymous function?                                |        Errors        |
|                        Is an arrow function a function declaration or function expression?                         |        Errors        |
|                                What is the first index position of an array in JS?                                 |  Arrays & Callbacks  |
|                                           What is a primitive data type?                                           |  Arrays & Callbacks  |
|                                         Is an array a primitive data type?                                         |  Arrays & Callbacks  |
|            What is the difference between: `for (let i = 0; i < 5; i++)` and `for (i = 0; i < 5; i++ )`            |  Arrays & Callbacks  |
|                                          What is a higher order function?                                          | Working with Objects |
|                                            What is a callback function?                                            | Working with Objects |
|                              What is the spread/rest `...` operator? What does it do?                              |        Big O         |
|                                 What is the difference between `1000` and `1_000`?                                 |      Recursion       |
|                                             What does `parseInt()` do?                                             |      Recursion       |
|                                            What does `parseFloat()` do?                                            |      Recursion       |
|                                              What does `Number()` do?                                              |      Recursion       |
|                                              What does `isNaN()` do?                                               |      Recursion       |
| In JavaScript `.?` is the symbol for optional chaining. What is optional chaining and where/when would you use it? |         OOP          |
|                         In JavaScript, what does the keyword static inside of a class do?                          |        OOP 2         |
|                          Why would we use the keyword static? What problem does it solve?                          |        OOP 2         |
|                                                                                                                    |                      |
|                                                                                                                    |                      |

## Evaluate Code Block:

### Control Flow

Do these code blocks return the same thing? What is different about them?

```js
const findFirstEvenNum = (arr) => {
  let num = 0;
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] % 2 === 0) {
      num = arr[i];
      break;
    }
  }
  return num;
};
```

```js
const findFirstEvenNum = (arr) => {
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] % 2 === 0) {
      return arr[i];
    }
  }
};
```

### Big O

Look at the following output

```js
const numbers = [1, 2, 3, 4, 5];
const printItems = (arr) => {
  for (let item in arr) {
    console.log(item);
  }
};

console.log(printItems(numbers));
```

The output is

```
0
1
2
3
4
undefined
```

Why is the last item `undefined`?
Insert Dash

### OOP

What is wrong with the following code?

```js
const delete = (item) => {
  console.log('item was deleted')
}
```
