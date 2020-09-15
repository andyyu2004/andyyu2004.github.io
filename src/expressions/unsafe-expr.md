# Unsafe Expressions

> **Syntax**
>
> <*unsafe-expr*> ::= `unsafe` <*[block-expr]*>
>
>

Unsafe blocks allow you to take references to arbitrary values by the `&` operator. This is
considered unsafe as there is nothing stopping you from dereferencing a dangling pointer that points
onto a stack frame that has been dropped.



[block-expr]: ./block-expr.md
