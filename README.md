![](https://raw.githubusercontent.com/khalid586/khalid586/main/assets/banner%20gif.gif)

## [<img align = "center" alt="Coding" width="54px" height = "36px" src="https://cdn.dribbble.com/users/1138721/screenshots/10809828/media/478d32b2e65c8c3194b7f2154e179231.gif">]() Overview
> **javascript is one of the most widely used programming languages in the world right now.In this repository you will get to know about javascript from the very basics and later on we will build projects as well.**

<br>


# Datatypes

📌 **Q: Why do we use `let` instead of `var`?**

- variables can be assigned without using `const` and `let` but it is not advised to do.

**Ans**: **`Var`** was previously used. The problem was var was not capable enough to deal with block and function scope. So when ever any developer used a variable multiple times js wasn’t able to detect which variable is being mentioned so it would change both of the variables. **`let`** fixed this issue.

- Any variable without value assigned to it will be assigned with value **`undefined`**
</aside>

---

We are going to look at some datatypes.

 `number`
 > 12 , 34 , 3,4

`bigint`
> 432434254423423432

`string`
> "My name is Khan"

`boolean`
> false , true


**`null`** 

- this is an **object**
- This is a standalone **value** this means the variable doesn’t hold any kind value.
- Example: Supposed we tried to fetch temperature from frontend and we didn’t get any temperature it will return us **null**.

`undefined` 
- it is a **datatype**
- Means datatype has not been defined yet.

`symbol`
- we use **symbol** for uniqueness (of `components`).

`Object`
- Holds values as `key:value`
  > Will deep dive into this later.

<br>

---


📌 **`NaN`** means not a number. when we want to convert something  to a number but it isn’t convertible to a number then we will get the value as `NaN` which means **Not a Number**.

```jsx
let score = "12b"
let scoreInt = Number(score)

console.log(typeof scoreInt) // This will tell you that it is a number
console.log(scoreInt) // This wil give you NaN(Not a Number)

// Number("33") -> 33
// Number("22ab") -> NaN
// Number(true) -> 1
```

📌 Empty string means `false`. Otherwise it means `true`

```jsx
let a = "khalid"
let b = Boolean(a)
console.log(b) // this will result in true

a = ""
b = Boolean(a)
console.log(b) // this will result in false 
```

---

📌 If a string is found somewhere the statement the following literals(string/numbers) will be treated as string

```jsx
console.log("1"+2) // 12
console.log(1+"2") // 12
console.log("1"+2+2) // 122
console.log(1+2+"2") // 32 [1 and 2 are numbers that is why they are added the moment we add them to "2" , 3 (1+2) also becomes a string. ]
```

📌 The **comparison** operator and **equality check** operator in JavaScript work differently.


📌 
**===** means strict equal. This checks both **value** and **datatype**.

```jsx
console.log(2 == "2") // true
console.log(2 === "2") // false
```

📌 Avoid following conversions

```jsx
console.log(null > 0)
console.log(undefined < 0)
```


📌 Datatypes

1. **Primitive** (call by **value**)
    - String
    - Number
    - Boolean
    - Null
    - Undefined
    - Symbol
    - BigInt
2. **Non Primitive** (call by **reference**)[These all are objects]
    - Array
    - Object
    - Function
</aside>

<aside>
📌 Symbol returns a unique value which helps us identify whether the value is unique or not.

```jsx
// Example

const a = Symbol("123")
const b = Symbol("123")

console.log(a == b) // false
```

📌 use `n` after end of a numeric literal. It will be converted to `BigInt`.

```jsx
let a = 234324343243243243243434324n
console.log(typeof a) // bigint
```

</aside>

<aside>
📌 Objects hold value as {key : value} format.

```jsx
let myObj = {
	name: "khalid",
	age : 23
}
```

📌 All the non primitive datatypes are `Objects`.









<!-- Things I need to include
1. Repositories 
2. preli result 
3. update all the 2x with 3x
4. Correct "About me" & "connect me" section 

testing new branch
 -->
