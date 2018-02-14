# SIMPLELANG

A simple programming language.

Made for JUST FOR STUDYING using lark-parser and parsing itself.

## Description

SIMPLELANG has below feature.

- Only support number. There is no string, list, object, and so on.
- Basic arithmetic operations (addition, subtraction, multiplication, division)
- Declaring and using variables.
- Declaring functions.
- Calling functions with local environments.

#### Basic arithmetic operations

You can use `+, -, *, /, ()`.

#### Declaring variables

You can declare new variables with `variable_name = <expression>`.

No need to type keyword like `var`, `val`, `let`, `const`.

And you can use overwrite value of variables by simply assign value again.

To refer the value of variables, simply call its name.

```
a = 1;
a; => 1

b = a + 2;
b; => 3
```

#### Declaring functions

The keyword to declare function is `def`. And `def` followed with name of function, and parameters(surrounded with parenthesis), and its content (surrounded with braces)

Like below.

```
def foo ( a, b, c ) {
  return a + b + c;
}
```

#### Calling functions

You can call declared function with its name. and you can pass arguments with brackets.

```
d = foo [ 1, 2, 3 ]
```

#### Return

Return statement returns value. And following statements or expressions are ignored.

```
return 2;

// below lines are meaningless
a = 1;
b = 3;
...

```

### Conclusion

An example of SIMPLELANG program.

```
a = 5;

def func ( b , c ) {
  a = 4;
  return a + b * c;
}

c =  func [ 2 , 4 ];

return c;
```

This returns 12.0.
