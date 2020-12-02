# CMPSC 201 Final Exam

## Your Name

1\. In Java, an object may be considered to be of more than one type; for instance, an instance of a subclass named `Kong` can also be considered as an instance of the parent class `Gorilla`. What is the term for the ability of a variable to be simultaneously considered as two different types?

2\. Explain short-circuit evaluation with a simple example involving the logical "or" operator "||".

3\. Each of these three composite types - "array," "set," and "record" - can contain several values at once (e.g., an array could have three elements, a set could contain three elements, a record could contain three elements). What makes them different? Explain the differences between an array type, a set type, and a record type.

4\. Which of the following Java functions correctly finds the sum of the digits in a nonnegative integer named `eeek`? For instance, `sum(354) = 3+5+4=12` and `sum(10223) = 1+0+2+2+3 = 8`. Explain why your chosen answer is correct and why each of the other methods is incorrect.

```
  (a)
```

```
int sum(int eeek) {
  int r = eeek % 10;
  int q = eeek / 10;
  return r + sum(q);
}
```

```

  (b)
```

```
int sum(int eeek) {
  if (eeek == 1)
    return 1;
  else
    return 1 + sum(eeek/10);
}
```

```

  (c)
```

```
int sum(int eeek) {
  if (eeek < 10)
    return eeek;
  else
    return sum(eeek/10);
}
```

```

  (d)
```

```
int sum(int eeek) {
  if (eeek == 0)
    return 0;
  else
    return  eeek % 10 + sum(eeek/10);
}
```

5\. In Fortran, arrays are stored in column-major order; in C and Java they are stored in row-major order. Does it make any difference to the programmer which method is used? Explain.

6\. If you have tried to track down precise definitions of the terms "strongly typed" and "weakly typed" you have probably come away frustrated. Our textbook defines a "strongly typed language" as one that "prohibits ... the application of any operation to any object that is not intended to support that operation." Give an example of such an operation and such an object, using only standard primitive types.

7\. Here are some C declarations and statements:

```
  double x = 10;
  double y = 20;
  double temp;
  double *p;
  double *q;
  p = &x;
  q = &y;
  *p = *p + *q;
  temp = 1 + *q;
  q = &temp;
```

(a) What is the final value of `*p`?

(b) What is the final value of `*q`?

(c) What is the final value of `x`?

(d) What is the final value of `y`?

8\. The following statements are entered into the Haskell interactive environment:

```
  Prelude> let f x y = take x y
  Prelude> let s = "barbarian"
  Prelude> let p = f 3 s
  Prelude> let g = f 2
```

(a) What is the value of `f 2 ['a','b','c']`?

(b) What is the value of `head s : tail s`?

(c) What is the value of `p`?

(d) What is the value of `g [1,2,3,4,5]`?

9\. What are virtual functions? Describe a circumstance in which virtual functions would be appropriate.

10\. True or false

(a) Java supports multiple inheritance.

Put "X" inside brackets [ ] of the correct answer.

- [ ] True.
- [ ] False.

(b) C++ uses static binding by default.

Put "X" inside brackets [ ] of the correct answer.

- [ ] True.
- [ ] False.

(c) In C++ we can overload symbolic operators, such as *.

Put "X" inside brackets [ ] of the correct answer.

- [ ] True.
- [ ] False.

(d) In lazy evaluation the parameters are evaluated exactly once.

Put "X" inside brackets [ ] of the correct answer.

- [ ] True.
- [ ] False.

11\. What does a language-based security entail? Describe what it is, provide at least one problem that may arise in a language-based security and how it can be solved.

12\. Suppose you want to (or have to) write a new programming language. List all of the necessary steps (things to consider/decide on and things to develop) to accomplish this task.
