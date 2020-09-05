# Functions

> Syntax:
>
> &lt;_fn_&gt; ::= `fn` &lt;_[ident]_&gt;
> &lt;_[generics]_&gt;<sup>?</sup> (&lt;_params_&gt;<sup>?</sup>)
> _&lt;return-type&gt;_
> _&lt;[block-expr]&gt;_
>
> &lt;_params_&gt; ::= &lt;_param_&gt; (`,` &lt;_param_&gt;)<sup>*</sup>
>
> <_param_> ::= &lt;_[expr]_&gt; `:` &lt;_[type]_&gt;
>
> <_return-type_> ::= `->` <_[type]_>

<!-- interesting, <_something_> seems to work as I wish -->

### Examples
```
fn identity<T>(t: T) -> T {
    t
}
```

```
fn naive_fib(n: number) -> number {
    if n < 2 { n } else { naive_fib(n-1) + naive_fib(n-2) }
}
```

[ident]: identifiers.md
[generics]: type-parameters.md
[type]: types.md
[expr]: expressions.md
[block-expr]: expressions/block-expr.md
