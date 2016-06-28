# Day 2

## Reading
* You Don't Know JS: Up & Going
  * Chapter 1: Into Programming
    * [Operators](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20&%20going/ch1.md#operators)

## Concepts

### Operators
An **operator** usually represents a simple action that's performed upon values. It usually takes the following form:

> [left-hand-side-value] [operator] [right-hand-side-value]

For example, in the multiplication operation `a * 2`, the LHS value is `a`, the RHS value is `2`, and the operator is `*`.

### Declarations
This is a more advanced concept that we'll revisit later. For now, all we need to know is that `a = 2;` and `var a = 2;` can achieve the same thing in our simple program. Adding that extra `var`, however, lets the compiler know "`a` is here!" more explicitly, makes your program more robust, and is a good practice to follow from now on.

### The `=` Operator
`a = 2` does **not** mean "`a` equals `2`" - it means "let `a` be `2`".

### The `+=` / `-=` / `*=` / `/=` Operators
It's a shorthand: if you find yourself writing something like `a = a + 2`, you can shorten it by writing `a += 2` instead; they do exactly the same thing. Beware though that it's `+=`, not `=+`.

### The `++` / `--` Operators
It's a shorthand: if you find yourself writing something like `a = a + 1`, you can shorten it by writing `a++` instead. **There are some important caveats** which we'll cover later, so it's recommended that you don't use `++` (and `--`) in your code for the time being.

### The `.` Operator
`.` locates a **property** of an **object**. For example, `console.log` locates the `log` property of the `console` object. An alternative syntax is `console['log']` - they do exactly the same thing, but is more verbose, so we usually don't use it.

### The `===` / `!==` Operators
`b === a` means "is `b` equal to `a`?" Usually, the answer will be either "yes" or "no"; in the world of programming languages, we use the words `true` and `false` instead. So for example:

* `console.log(2 === 2)` will result in `true`
* `console.log(2 === 1)` will result in `false`

In JavaScript, `!` indicates negation, so `!==` means "**not** equal", and `b !== a` means "is `b` not equal to `a`?"

* `console.log(2 !== 2)` will result in `false`
* `console.log(2 !== 1)` will result in `true`

### The `&&` / `||` Operators
These are your logical *AND* and *OR*. For example:

* `console.log(true && false)` will result in `false`
* `console.log(true || false)` will result in `true`

### (Extra) The `**` / `%` Operators
These two operators were not mentioned inside today's reading material, but are needed to complete our exercises:

* `**`: the exponentiation operator
  * `2 * 2 * 2 * 2` is exactly the same with `2 ** 4`
  * `3 * 3 * 3` is exactly the same with `3 ** 3`

* `%`: the remainder operator
  * `console.log(2 % 3)` will result in `2`
  * `console.log(3 % 3)` will result in `0`
  * `console.log(4 % 3)` will result in `1`
  * `console.log(5 % 3)` will result in `2`

## Exercises
1. Explain the following code; what does it do?

  (Hint: run the code and see how it works)

  ```javascript
  var x = prompt();
  
  console.log(x *= x *= x);
  ```

2. Rewrite the code in Ex. 1 using the `**` operator; the output should not be affected.

3. Write a program that:

  * Prompt the user to input a number `x`
  * Test if `x` is even
  * Output the result to the console; the output should be `true` when x is even or `false` when `x` is odd
