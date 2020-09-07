# Operator Expressions


> **Syntax**
>
> <*operator-expr*> ::= \
> &nbsp; &nbsp; &nbsp; | <*[assignment-expr]*> \
>

## Assignment Expressions


> **Syntax**
>
> <*assignment-expr*> ::= <*[expr]*> `=` <*[expr]*>
>

The expression on the left of the `=` must be an *[lvalue]*. Following
in the style of
[*C*](https://en.wikipedia.org/wiki/C_(programming_language)), the
result of an assignment expression is the rhs.

```
// assigns `x` to 5
// main also evaluates to 5
fn main() -> int {
    let x = 0;
    x = 5
}
```

[expr]: ../expressions.md
[lvalue]: ../lvalues-and-rvalues.md#lvalues
[rvalue]: ../lvalues-and-rvalues.md#rvalues
[assignment-expr]: #assignment-expressions
