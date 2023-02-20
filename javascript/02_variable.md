## Javascript
# 2. Variable

### 1. var  
The var statement declares a function-scoped or globally-scoped variable, optionally initializing it to a value.  
If var is declared outside the function, it becomes globally-scoped variable. Conversely, if declared in a function, it becomes function-scoped variable.

```
var i = 0

function functionA () {
    console.log(i)
    i = 1
    var j = 3
}

functionA(i)
console.log(i)
// console.log(j) // ReferenceError: j is not defined
```

var can be declared again. It is also possible to update only the value.

```
var a = "This is A"
console.log(a)

var a = "This is a"
console.log(a)

a = "Aa"
console.log(a)

// output : 
// This is A
// This is a
// Aa
```

Hosting in Javascript is a mechanism by which variable and function declarations are moved to the top. Therefore, the two codes below are the same.
```
console.log(hoistingTest)
var hoistingTest = "Hello hoisting!"
```
```
var hoistingTest
console.log(hoistingTest)
hoistingTest = "Hello hoisting!"
```
When var is declared, the value is initialized to 'undefined'. Therefore, the above code will output 'undefined' as a result.

### 2. let  
The let declaration declares a block-scoped local variable, optionally initializing it to a value.
```
let i = 0

function functionA () {
    console.log(i)
    i = 1
    let j = 3
}

{
    let k = 5;
}

functionA(i)
console.log(i)
// console.log(j) // ReferenceError: j is not defined
console.log(k) // ReferenceError: k is not defined
```

Unlike var, let cannot be declared again. value can be updated.

```
let a = "This is A"
console.log(a)
// let a = "This is a" // SyntaxError: Identifier 'a' has already been declared
// console.log(a)
a = "Aa"
console.log(a)
```
However, if you declare in a different scope, no error will occur.
```
let a = "This is A"
console.log(a)
// let a = "This is a" // SyntaxError: Identifier 'a' has already been declared
// console.log(a)

{
    let a = "This is a"
    console.log(a)
}

a = "Aa"
console.log(a)
```

Let does not initialize to 'undefined' when declared differently from var.

```
console.log(hoistingTest)
let hoistingTest = "Hello hoisting!"
```

Therefore, a ReferenceError will occur as a result of the above code.
    
### 3. const  
The const declaration creates block-scoped constants, much like variables declared using the let keyword. The value of a constant can't be changed through reassignment (i.e. by using the assignment operator), and it can't be redeclared (i.e. through a variable declaration). However, if a constant is an object or array its properties or items can be updated or removed.

<!-- ### 2. hoisting -->

***
#### Keywords
- hoisting : JavaScript Hoisting refers to the process whereby the interpreter appears to move the declaration of functions, variables or classes to the top of their scope, prior to execution of the code.

#### Reference
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/var
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const
- https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/