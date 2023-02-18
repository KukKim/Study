# Typescript


### Typescript
In wiki, typescript is defined as follows:

>TypeScript is is a strict syntactical superset of JavaScript and adds optional static typing to the language.

This means that while typescript provides the functions of javascript, it also provides additional functions of typescipt.  
It is also compiled into a javascript file when you compile a file in typescript.

### Differences from Javascript
JavaScript is not class-based languages (like Java or C++). it is dynamic and does not have static types.  
1. Defining types  
    TypeScript supports an extension of the JavaScript language, which offers places for you to tell TypeScript what the types should be.  
    For example, to create an object with an inferred type which includes name: string and id: number, you can write:
    ```
        const user = {
            name: "Hayes",
            id: 0,
        };
    ```
    You can explicitly describe this object’s shape using an interface declaration:
    ```
        interface User {
            name: string;
            id: number;
        }
    ```

***
#### Keywords
- Duck typings

#### Reference
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain
- https://en.wikipedia.org/wiki/TypeScript
- https://www.typescriptlang.org/ko/docs/handbook/typescript-in-5-minutes.html