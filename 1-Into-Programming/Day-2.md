# Day 2

## Reading
* You Don't Know JS: Up & Going
  * [Chapter 1: Into Programming](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20&%20going/ch1.md)
    * Operators

## Concepts

### Operators
An **operator** usually represents a simple action that's performed upon values. It usually takes the following form:

> [left-hand-side-value] [operator] [right-hand-side-value]

For example, in the multiplication operation `a * 2`, the LHS value is `a`, the RHS value is `2`, and the operator is `*`.

All the operations in JavaScript read from left to right.

### Declarations
This is a more advanced concept that we'll revisit later. For now, all we need to know is that `a = 2;` and `var a = 2;` can achieve the same thing in our simple program. Adding that extra `var`, however, lets the compiler know "`a` is here!" more explicitly, makes your program more robust, and is a good practice to follow from now on.

### The `=` Operator
`a = 2` does **not** mean "`a` equals `2`" - it means "let `a` be `2`".

### The `+=` / `-=` / `*=` / `/=` Operator
It's a shorthand: if you find yourself writing something like `a = a + 2`, you can shorten it by writing `a += 2` instead; they do exactly the same thing. Beware though that it's `+=`, not `=+`.

### The `++` / `--` Operator
It's a shorthand: if you find yourself writing something like `a = a + 1`, you can shorten it by writing `a++` instead. **There are some important caveats** which we'll cover later, so it's recommended that you don't use `++` (and `--`) in your code for the time being.

### The `.` Operator
`.` locates a **property** of an **object**. For example, `console.log` locates the `log` property of the `console` object. An alternative syntax is `console['log']` - they do exactly the same thing, but is more verbose, so we usually don't use it.

### The `===` / `!==` Operator
`b === a` means "is `b` equal to `a`?" Usually, the answer will be either "yes" or "no"; in the world of programming languages, we use the words `true` and `false` instead. So for example:

* `console.log(2 === 2)` will result in `true`
* `console.log(2 === 1)` will result in `false`

In JavaScript, `!` indicates negation, so `!==` means "**not** equal", and `b !== a` means "is `b` not equal to `a`?"





