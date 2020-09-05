# Block Expressions

> **Syntax**
>
> <*block-expr*> ::= `{` \
> &nbsp; &nbsp; &nbsp; <_[stmt]_> <sup>*</sup> \
> &nbsp; &nbsp; &nbsp; <_[expr]_> <sup>?</sup> \
>`}`

A block expression is a control flow construct for sequencing multiple
statements with an optional final expression. A block also introduces a
new lexical scope where variable declarations are visible only from
after the [let statement] that declares it until the end of the block.

Each statement is executed sequentially and the type of the entire block
is the type of the final expression, or `()` if the expression is omitted.

Note how the differentiating factor between an expression statement and
an expression is the trailing semicolon.


```
let x: int = { 5 };

let x: () = { 5; };

```


[stmt]: ../statements.md
[expr]: ../expressions.md
[let statement]: ../statements/let-stmts.md

