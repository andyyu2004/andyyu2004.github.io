# Box Expressions

> **Syntax**
>
> <_box-expr_> ::= `box` <_[expr]_>


Box expressions are the way to achieve heap allocation in *L*. The
memory is managed by a garbage collector. Box expressions return a
pointer.

`t: T => box t: &T`

[expr]: ../expressions.md
