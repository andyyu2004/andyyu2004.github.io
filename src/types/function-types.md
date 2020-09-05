# Function Types

> **Syntax**
>
> <*function-type*> ::= `fn(` <*types*><sup>?</sup> `)` <*return-type*><sup>?</sup>
>
> <*types*> ::= <*[type]*> ( `,` <*[type]*>)
>
> <*return-type*> ::= `->` <*[type]*>

### Examples

```
let f: fn();
let g: fn(bool) -> bool;
let h: fn(num) -> fn(bool, bool) -> bool;
```

[type]: ../types.md
